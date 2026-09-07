# Manual skill extraction reference

For instructors or an agent carrying out the bootstrap. This downloads data; it does not run upstream installers. Read the commands and confirm their destinations first. Use only the recipe for your actual shell.

Pinned source: [Deep Interview at the course revision](https://github.com/Yeachan-Heo/oh-my-codex/tree/304fb3b4825c4132c273732b14d2d5e86b54f8e3/skills/deep-interview).

## macOS/Linux/WSL: Bash or Zsh

Run from a directory where temporary downloads are permitted. Stop on any failed step; do not continue to copying after a failed fetch.

```sh
task_skill_source=$(mktemp -d)
git clone --filter=blob:none --no-checkout --depth 1 https://github.com/Yeachan-Heo/oh-my-codex.git "$task_skill_source"
git -C "$task_skill_source" fetch --depth 1 origin 304fb3b4825c4132c273732b14d2d5e86b54f8e3
git -C "$task_skill_source" sparse-checkout set --no-cone /skills/deep-interview/ /LICENSE
git -C "$task_skill_source" checkout --detach FETCH_HEAD
git -C "$task_skill_source" rev-parse HEAD
git -C "$task_skill_source" ls-tree -r --name-only HEAD -- skills/deep-interview
```

The printed revision must equal the pin. Inspect the complete skill file and license. At this revision there is one source file, `skills/deep-interview/SKILL.md`. It references external OMX tools; do not fetch or install those as part of this recipe.

Choose the verified course-root destination from SETUP. Create its parent directory if absent. If the `deep-interview` destination exists, compare it and stop before any conflicting overwrite. Copy the directory and the license using the shell's normal file-copy operation, quoting actual paths. Compare each relative file and hash using `shasum -a 256` on macOS or `sha256sum` on Linux.

## Windows: PowerShell

Use the Windows agent's local environment, not this recipe inside WSL. Commands are intentionally separate so failures can be seen.

```powershell
$taskSkillSource = Join-Path ([System.IO.Path]::GetTempPath()) ("course-skill-" + [guid]::NewGuid().ToString("N"))
git clone --filter=blob:none --no-checkout --depth 1 https://github.com/Yeachan-Heo/oh-my-codex.git $taskSkillSource
if ($LASTEXITCODE -ne 0) { throw "Clone failed; stop." }
git -C $taskSkillSource fetch --depth 1 origin 304fb3b4825c4132c273732b14d2d5e86b54f8e3
if ($LASTEXITCODE -ne 0) { throw "Fetch failed; stop." }
git -C $taskSkillSource sparse-checkout set --no-cone /skills/deep-interview/ /LICENSE
if ($LASTEXITCODE -ne 0) { throw "Sparse checkout failed; stop." }
git -C $taskSkillSource checkout --detach FETCH_HEAD
if ($LASTEXITCODE -ne 0) { throw "Checkout failed; stop." }
git -C $taskSkillSource rev-parse HEAD
git -C $taskSkillSource ls-tree -r --name-only HEAD -- skills/deep-interview
```

Inspect hidden files too with `Get-ChildItem -Force -Recurse`. Use `Get-FileHash -Algorithm SHA256` to compare source and destination files. Use literal, resolved paths when copying. Do not translate Bash variables or flags blindly into PowerShell.

## Verification contract

1. Exact source commit matches the pin.
2. Frontmatter has the expected name and description.
3. Full skill directory is inspected; no escaping paths or unexpected symlinks.
4. Only that directory and its license are installed.
5. Every source skill file matches the installed relative file and SHA-256 hash.
6. Provenance records date, source, pin, destination, file list and hash result.
7. Skill discovery is observed or explicitly recorded as unverified.
8. The standalone interview prompt produces one relevant question and stops when asked.

If Git sparse checkout is not supported, an instructor may download an archive of the **same pinned commit**, inspect its paths, and extract only this directory and LICENSE. Do not replace the pin with a different branch silently.

A pinned revision improves reproducibility, not security by itself. Review its contents. Recheck official product skill locations before a new cohort.
