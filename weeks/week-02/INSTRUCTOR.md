# Week 2 instructor notes

## Preparation

Bring the Week 1 project and inspection log. Have materials/demo-brief.md and templates/project-brief.md open.

## Demo idea

Add an owner filter to the tracker. Example: Alex owns two open tasks and Sam owns one; filtering Alex shows two; clearing the filter shows all three.

## Instructor script and facilitation

Open with: “What did the agent have to guess last week?” Collect one guess from each learner. Explain that useful context is the information that would change a decision.

Demo the request “Make the tracker smarter.” Ask the group to predict three different interpretations. Then show a goal for a coordinator who needs to see incomplete tasks for one owner. The constraint is local fake data; the non-goal is notifications.

Read one example input and its expected output. Say: “An example lets us see whether we mean the same thing.” Show the difference between “fast” and “the open count updates after I tick one task.”

At minute 20, let learners choose at most three relevant files to mention. Ask why each matters. A transcript of every previous chat is not a useful default context pack.

At minute 35, write a criterion in action/result form: “Given two open tasks for Alex and one for Sam, selecting Alex shows two tasks.” Have a peer try to find an interpretation that would make the criterion misleading.

During implementation, stop scope growth by referring to the explicit non-goals. At peer review, keep the author silent until the user has attempted the check. Revise the brief if the check itself was ambiguous.

## What to watch for

- Ask the learner to demonstrate: Select relevant files and examples without dumping an entire private workspace.
- Ask the learner to demonstrate: Write a user-centered goal, constraints and non-goals.
- Ask the learner to demonstrate: Create three success criteria that another learner can test.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect an updated brief, a three-file-or-fewer context index and a peer acceptance record.
