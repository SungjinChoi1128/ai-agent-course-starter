# Validation record

Checked on 2026-09-07.

## Completed checks

- All eight week folders contain README, instructor notes, exercises/homework and prompts.
- All eight agendas total exactly 90 minutes.
- Local Markdown links checked for existing targets.
- Markdown code fences checked for closure.
- All six JSON fixtures parse; the primary dataset has four actions, three open.
- Official upstream source and skill path verified at commit 304fb3b4825c4132c273732b14d2d5e86b54f8e3.
- Pinned sparse checkout executed on macOS with Git 2.50.1.
- Skill copied into an isolated temporary destination; installed SKILL.md and upstream license compared byte-for-byte with source.
- Setup and first-lesson instructions manually walked through for scope, sequencing and fallback paths.

## Not claimed

- Git was already installed on this machine; missing-Git installation paths were checked against documentation, not executed on fresh operating systems.
- Windows/PowerShell and Linux installation procedures have not been executed here.
- Native skill discovery and an interactive interview have not been tested in a fresh learner Codex or Claude Code session. Complete the one-question smoke check before relying on discovery.
- The classroom prompt explicitly adapts unavailable OMX runtime behavior; full OMX compatibility is not claimed.
- There is no bundled learner application to build or run. Learners create one during the exercises.
- The local optional JSON language server was unavailable; JSON was validated with the installed Node runtime instead.

Before a new cohort, repeat setup on the learners' actual agent versions and record the results here.
