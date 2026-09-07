# Setup

Budget 30–45 minutes before Week 1. Setup is complete only after Git works, the course folder opens, the skill file is present, and a one-question interview smoke check succeeds.

## Before the bootstrap

You need a browser and an already-working local coding agent: Codex Desktop/CLI or Claude Code. Sign in through the product's own interface. The bootstrap does not install or purchase a coding-agent subscription.

Open an empty folder you control in your agent. If Git is not yet installed, view [the bootstrap prompt](prompts/00-bootstrap.md) on GitHub, copy its full fenced text, and paste it into the agent chat. The agent can install Git first, then fetch this course. Alternatively, download this repository as a ZIP and open the extracted folder.

A browser-only chat that cannot run local commands cannot install software on your laptop. In that case, follow the official Git installer with instructor support, then resume in the local agent.

## Recommended path

1. Read the [bootstrap prompt](prompts/00-bootstrap.md), including its boundaries.
2. Paste it into your local coding agent. Tell it which agent you use if it cannot detect this.
3. Review the proposed installation source, commands, destination folders, and any administrator request.
4. Let it verify Git, download the course, extract the one upstream skill, and prepare the workspace.
5. Open the actual course folder as your project and refresh skill discovery if needed.
6. Paste [the classroom interview prompt](prompts/01-deep-interview.md) with a harmless idea. Answer one question, then say “Stop the smoke check.”
7. Read the setup report. A file existing does not prove the agent discovered it.

## Git installation by platform

The agent must detect the environment before choosing a command. Check `git --version` and the resolved executable, not just the presence of a file named git.

| Platform | Appropriate route when Git is absent | Watch for |
| --- | --- | --- |
| macOS | Official Git macOS instructions; use existing Homebrew with `brew install git`, or Apple's Command Line Tools installer when appropriate | Do not install Homebrew merely to avoid discussing options. A macOS git shim can exist before developer tools are installed. |
| Windows PowerShell | Official Git for Windows installer, or existing WinGet using `winget install --id Git.Git -e --source winget` after reviewing the package | Reopen terminal after installation to refresh PATH. PowerShell syntax differs from Bash. |
| Linux | Identify distribution and package manager first; install that distribution's Git package | If system installation needs administrator rights, explain the exact command and use the normal permission flow. Do not blindly prepend sudo. |
| WSL | Treat the WSL shell as Linux | Keep agent, Git, course folder and skill destination in the same environment. Windows and WSL home folders differ. |
| Managed device | Use the organisation's approved installer or ask IT | Do not work around policy or repeatedly retry denied installations. |

Source: [official Git installation guide](https://git-scm.com/install/). Install methods change; verify the current platform page before running one.

## Codex and Claude Code

These paths describe current local discovery, checked 2026-09-07. Installed versions and managed policies may differ.

| Surface | Recommended course-local skill file | Invocation |
| --- | --- | --- |
| Codex | `.agents/skills/deep-interview/SKILL.md` at course root | Select the installed skill in the available skill interface, or use a verified `$deep-interview` reference in agent chat |
| Claude Code | `.claude/skills/deep-interview/SKILL.md` at course root | Check the command list for the installed skill; `/deep-interview` is the documented pattern for a discovered skill |
| Either, discovery unavailable | Ask the agent to read the verified local file by its exact path | Paste the classroom compatibility prompt and call this direct-file use, not native skill discovery |

These are **chat/skill references, not terminal commands**. Do not type dollar-name or slash-name invocations into your shell. Do not invent `codex skills install`, `claude skills add`, or other unsupported commands.

For Codex, current user-scope guidance uses `~/.agents/skills/`. Some installer versions still default to `~/.codex/skills/`; verify the installed client's supported location and explicitly set the destination when using a helper. For Claude Code, the user location is `~/.claude/skills/`. Prefer project scope for this class so installation affects only the teaching workspace. Avoid duplicate names across scopes.

Codex and Claude Code can load an instruction file without implementing each other's tools. The extracted upstream skill calls OMX state commands and other skills that are deliberately not installed here. [The compatibility prompt](prompts/01-deep-interview.md) keeps a human-paced interview and local brief, explicitly omits unavailable orchestration, and requires a separate build request.

Official sources: [Codex skills](https://learn.chatgpt.com/docs/build-skills), [Claude Code skills](https://code.claude.com/docs/en/skills). Reopen the session if the new skill does not appear, and check the current product help before assuming a feature exists.

## Workspace and version history

The course folder is the teaching reference. The bootstrap creates `workspace/projects/my-first-agent-project/` and `workspace/notes/` without replacing existing work. The practice folders are ignored by the course repository.

If you cloned the course, it already has Git history. If you downloaded a ZIP, the bootstrap can initialise Git in that folder after confirming it is not inside another repository. Reuse an existing Git identity. If missing, request the learner's chosen name and email before a commit; use local configuration only. A private GitHub noreply address is suitable when chosen by the learner. Never invent an identity or change global settings.

GitHub publication is optional for students. A local commit does not upload anything. Do not push a clone back to the instructor. In W3, learners can make their project its own local repository; in W8, they may publish to a repository they own after review.

## If setup stalls

- No admin permission: use the approved installer route or the paper fallback; don't disable restrictions.
- Cannot access GitHub: use the downloaded course and [fallback interview](prompts/01-deep-interview.md#fallback-without-the-skill). Resume extraction when access returns.
- Skill directory already exists: compare source and contents; reuse an identical copy, otherwise stop before replacing it.
- OMX command missing: use the compatibility prompt. Installing the full toolkit is not part of the course bootstrap.
- Wrong folder opened: locate `COURSE_OVERVIEW.md`, then open that containing folder in the agent.
- Git author missing: set a learner-approved identity locally, or defer commits and continue the lesson.
- Skill is installed but not shown: refresh/reopen, verify scope and conflicts, then use explicit-file reading if necessary.
- Repository name already exists: choose a new local destination; do not delete the old folder.

## Light safety

Review downloaded instructions and scripts before allowing execution. A familiar repository name does not make every command appropriate for your machine. Use the synthetic examples in this course. Never paste tokens, passwords, keys, real customer data, or private meeting transcripts into chat or commits. If a real credential is disclosed, revoke or rotate it; deleting the visible text alone does not undo exposure.
