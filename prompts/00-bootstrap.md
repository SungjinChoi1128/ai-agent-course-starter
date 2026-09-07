# First-week bootstrap prompt

Copy the complete block into an **already-installed local coding agent**, not a terminal. It installs Git only if needed, downloads the course if needed, installs only the Deep Interview skill, and prepares a local practice workspace.

The instructor can replace the course URL with their own template copy. The pinned skill revision is recorded in [Sources](../materials/SOURCES.md). There is no need to install GitHub CLI for learners.

```text
Help me set up this eight-week AI coding-agent course on this computer.
I am a non-developer. Explain each phase briefly and carry out the setup
using your available local tools and normal approval controls.

Course URL:
https://github.com/SungjinChoi1128/ai-agent-course-starter.git

Official skill source:
https://github.com/Yeachan-Heo/oh-my-codex.git
Skill directory: skills/deep-interview
Pinned revision: 304fb3b4825c4132c273732b14d2d5e86b54f8e3

Scope and safety:
- Install Git if missing and ONE upstream skill, not all of OMO/OMX.
- Do not install oh-my-codex packages, hooks, MCP servers, tmux, other skills,
  or a new agent runtime. Do not run omx setup or upstream setup scripts.
- Review install commands with me: source, purpose, files affected and
  administrator needs. Use normal approvals. Never blindly use sudo,
  disable safeguards, pipe a downloaded script into a shell, or execute
  code from a downloaded skill during installation.
- Do not read or print secret values, credential stores or full environment
  dumps. Do not request tokens in chat. Use existing authentication or
  the official interactive sign-in flow only if actually needed.
- Preserve existing folders, Git history, settings, skills and identities.
  No deletions, force pushes, automatic publication or overwrites.
- This is local setup. Do not create a remote repository or push anything.

1. Detect and report the environment.
Identify OS, shell, whether this is WSL/container/remote rather than my laptop,
current folder, agent surface/version if observable, and normal skill discovery
locations. Avoid assuming that Codex Desktop implies the codex CLI is installed.
If you cannot execute locally, explain that limitation and give the matching
manual step; never claim an installation happened.

2. Verify or install Git FIRST.
Run git --version and resolve its executable using the actual shell.
On macOS, a git shim alone is not sufficient; the version check must succeed.
If Git works, keep it. If missing, consult https://git-scm.com/install/
and choose the detected platform's official route:
- macOS: use existing Homebrew when suitable, or the official/Apple developer
  tools route. Explain any GUI step; do not install a package manager silently.
- Windows: use the official Git for Windows installer, or existing WinGet
  with the exact Git.Git package after source review. Refresh the terminal
  environment afterwards.
- Linux/WSL: inspect the distribution and available package manager.
  Show the distribution-appropriate Git package command. If installation
  requires admin privileges, request them through the normal approval
  mechanism or give the manual step. Do not guess a sudo command.
Stop this phase until git --version succeeds. Report the version and path.

3. Locate or obtain the course and prepare its workspace.
If this course is already open, reuse its actual root after checking for
README.md and COURSE_OVERVIEW.md. Otherwise choose a new course folder under
the current writable location and clone the course URL there. If the intended
folder exists, inspect it and reuse only when it is the correct course;
choose a new folder or ask before a conflict. ZIP extraction is acceptable
if cloning is unavailable; inspect the archive paths before extracting.
Do not mistake the skill-source repository for the course workspace.

Inspect git rev-parse --show-toplevel and git status. If this is a ZIP copy
and has no repository, confirm the course root is not inside another repo,
then git init in that exact course root. Do not initialise an ancestor folder.
If cloned, preserve history and remote; explain that origin is the instructor's
repository and students should not push to it.

Create, if absent:
workspace/projects/my-first-agent-project/
workspace/notes/
Do not replace existing content. Confirm the repository ignore rules cover
practice outputs, .env files, and local skill installations. If any needed
rules are missing, append only those rules without replacing the file.

Read existing effective Git user.name and user.email without changing them.
If either is missing, ask for my chosen commit identity only when a commit
is needed. Configure it with git config --local in the exact repo after I
supply it. Do not invent values or use --global. A setup can finish with
commits deferred, clearly recorded. Do not commit automatically in this setup.

4. Extract only the Deep Interview skill from the official source.
Use the pinned revision above; do not silently substitute the latest main.
Choose the destination based on current official docs and my installed agent:
- Codex course-local default: COURSE_ROOT/.agents/skills/deep-interview/
- Claude Code course-local default: COURSE_ROOT/.claude/skills/deep-interview/
If a project-local path is unsupported, verify a supported user-local location
and explain the wider scope before writing there. Keep Windows/WSL paths in
the same environment as the agent. Do not install in both places unnecessarily.

If a trusted built-in skill-installer helper is actually available, inspect
its documented options and use the repository, exact revision, skill path
and explicit parent destination. Do not invent a helper command or path.
Otherwise perform a Git sparse checkout in a fresh temporary directory:
clone with --filter=blob:none --no-checkout --depth 1;
fetch the pinned revision with --depth 1;
sparse-checkout set --no-cone /skills/deep-interview/ /LICENSE;
checkout the fetched revision detached.
Check every command's success before continuing. See the manual recipe in
materials/skill-extraction.md for shell-specific examples.

Verify git rev-parse HEAD equals the pin. Check that the skill source directory
contains SKILL.md with name: deep-interview and a non-empty description.
Enumerate all files, including hidden files. Inspect text instructions and
relative references. Reject path traversal, unexpected symlinks, and references
that would copy files from outside the intended skill directory.

Copy the complete skills/deep-interview directory, preserving all internal
files, plus upstream LICENSE as LICENSE.upstream in the installed directory.
Do not copy the source .git directory, other skills, root AGENTS.md, configs,
hooks or packages into the course. A temporary Git checkout is acquisition,
not a full toolkit installation.

If the destination already exists, compare it. Reuse identical contents;
otherwise stop and explain the conflict without replacing anything.
Compare relative file lists and SHA-256 hashes of every installed skill file
against the source, and compare LICENSE.upstream with the fetched license.
Do not claim success from SKILL.md existence alone.

Record source URL, full revision, actual destination, file list/hashes and
inspection date in workspace/skill-provenance.md. Keep the upstream contents
unmodified. Do not automatically remove the temporary checkout; report its
path for later deliberate cleanup.

5. Explain runtime compatibility and verify discovery.
The downloaded skill includes OMX commands and references to other skills.
Those are NOT installed here. Do not claim this is a complete OMX setup.
Read prompts/01-deep-interview.md and explain its explicitly adapted
classroom mode: one question at a time, a local brief, no OMX state service,
no automatic orchestration, and a separate build request.

Use current product documentation and the actual skill selector/help to
verify invocation. Codex commonly uses a $deep-interview skill reference
in chat; Claude Code uses /deep-interview when the skill is discovered.
These are not shell commands, and neither syntax is universal.
If discovery is unavailable, explicitly read the verified local SKILL.md
and use the classroom compatibility prompt; label this direct-file use.
Reopen or refresh the agent if needed. Do not fabricate a successful
selector check when you cannot observe it.

6. Report setup status and stop.
Write workspace/setup-report.md with:
- environment and successful Git version/executable;
- course root, repository root and current branch if any;
- workspace locations and identity status (configured or commits deferred);
- source revision, skill destination and file/hash verification result;
- native discovery verified, pending user check, or direct-file fallback;
- unavailable OMX features and the compatible interview prompt to use;
- precise remaining manual steps, without secret values.
Explain Git versus GitHub in two sentences.
End by giving me the exact next action: open Week 1 and paste the classroom
interview prompt for a one-question smoke check. Do not begin building an app.
```
