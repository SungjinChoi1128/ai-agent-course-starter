# Week 8 instructor notes

## Preparation

Students arrive with a small idea, their current project and a draft brief. Use materials/capstone-ideas.md and templates/handover.md. New integrations are out of scope unless already working.

## Demo idea

Instructor shows a two-minute handover: open runbook, start the project, complete a user task, trigger an empty-input case and point to one documented limitation.

## Instructor script and facilitation

At the start, give each learner one minute: who is the user, what recurring problem do they face, and what will work today? Choose scope that can be finished in 25 minutes of build time by extending existing work.

At minute 10, ask peers whether the three checks are observable. A capstone that requires a new login system, payment service or external write should be reduced to a local draft workflow unless that integration is already safely working.

During the build block, check progress halfway. If scope is too large, explicitly agree which non-essential behavior is deferred and update the brief. Do not quietly remove an acceptance criterion after seeing it fail.

At minute 45, give the peer only the runbook and task, not a narrated tour. The author watches and records. A peer who cannot start the project has found a handover defect worth fixing.

During correction, prioritise a broken acceptance criterion over polish. Ask the learner to repeat the exact failed steps and record the new result.

Use five minutes per final demo: one minute for user/problem, two for a live workflow, one for evidence including an edge case, and one for limitations and next step. If a build is incomplete, demonstrate what actually works and identify the remaining blocker.

End with ownership: can another person find it, run it, understand its data and know what not to trust yet? Apply the course rubric consistently; code volume and tool choice are not scoring dimensions.

## What to watch for

- Ask the learner to demonstrate: Deliver one bounded project that helps a specific user.
- Ask the learner to demonstrate: Demonstrate three success checks and one failure or edge case.
- Ask the learner to demonstrate: Give a peer enough instructions to use and restart it, with honest limitations.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect capstone brief, project, inspection evidence, runbook, handover and a next-step note.
