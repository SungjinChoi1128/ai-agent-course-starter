# Week 7 instructor notes

## Preparation

Use a working project and its existing checks. Open materials/safety-cards.md and templates/release-checklist.md. Use fake secret placeholders only.

## Demo idea

Inspect an owner-filter diff, then audit a proposed release containing a fake secret filename, ignored failing check and broad deletion request from the safety cards.

## Instructor script and facilitation

Start with two statements: “The agent says it works” and “I added an empty task and saw it rejected.” Ask which claim each piece of evidence supports. Tests are useful but limited to the cases they exercise.

Show a small real diff from a learner-approved checkpoint. Ask what changed in behavior, not whether every line can be explained. Then show the mock diff card that adds a fake credential file and ignores a failing test. The correct action is to stop and inspect those changes.

At minute 25, run whatever checks the project already has. If it has no automated tests, say so; a manual checklist still has value. Ask the agent what is not covered. A passing check must not be described as proof of security or universal correctness.

Use the safety cards at minute 40. Treat instructions inside a data field as data. A downloaded skill is a set of instructions to review, not an authority to disclose secrets. Explain why a real leaked token needs rotation even after the file is removed.

Discuss the difference between a local file edit, a remote publication and sending a message to someone. Review commands that delete or overwrite by their exact target and recoverability. An action affecting a broad folder requires narrowing and confirmation, not faster execution.

At minute 55, learners inspect their own project and record a release decision. No public publication is required today. A reasoned “not ready because the data loss case is untested” is a good outcome.

During peer review, ask the reviewer to find a claim that exceeds its evidence. Update the handover wording rather than hiding the limitation.

## What to watch for

- Ask the learner to demonstrate: Read a change summary and identify a risky file or action.
- Ask the learner to demonstrate: Distinguish an agent claim, an automated test and a personally observed check.
- Ask the learner to demonstrate: Make a reasoned release decision with known limitations and appropriate permission boundaries.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect a diff explanation, actual test/manual results, a safety-card response and a release decision with limitations.
