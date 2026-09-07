# Week 3 instructor notes

## Preparation

Use the existing project. Have the file map and restart-runbook templates ready. No new framework is required; a zero-dependency project is a valid example.

## Demo idea

Locate brief.md, the main app file, data and run instructions. Create a local checkpoint, make a small label edit, inspect the diff, and restart the project.

## Instructor script and facilitation

Start by closing the agent chat panel and asking: “Where is your work?” Learners should point to a folder, not a conversation. A workspace is the folder the agent is working in; a terminal is a place to run commands.

Show a harmless command only after predicting what it will do. Use the current shell's directory command and git status. Explain the current directory before discussing command syntax.

The course's practice directory is ignored by the outer teaching repository. Help each student initialise their own project repository only in workspace/projects/my-first-agent-project after inspecting its contents. Give it its own ignore rules before staging. Reuse their Git identity, or ask for their chosen name and email and configure locally. Do not change global settings.

Before a checkpoint, show the selected files and explain that a commit is a local snapshot. Explain that push uploads commits to a configured remote, and that today's exercise needs no remote.

At minute 40, inspect what is actually present. If there is a package manifest, explain that it lists required libraries and tasks; a lockfile records resolved versions. If there is none, explicitly say that this project may not need a dependency manager. Do not install packages just to demonstrate an install.

During restart practice, stop only the learner's known project process using its normal stop control. Do not kill every process on a port or delete dependencies to manufacture a problem. Let a peer use the runbook without rescue for two minutes before offering a hint.

## What to watch for

- Ask the learner to demonstrate: Find the project root and explain the role of its important files.
- Ask the learner to demonstrate: Distinguish local files, a local Git repository and a remote repository.
- Ask the learner to demonstrate: Restart a project from written instructions and understand why an install is needed.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect file map, restart runbook, repository location and checkpoint reference or documented deferral.
