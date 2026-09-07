# Week 1 instructor notes

## Preparation

Complete SETUP.md before class. Open the sample meeting notes and demo brief. Have one prepared local tracker available if the live build stalls.

## Demo idea

Meeting-action tracker with manual task entry, optional owner, a completed checkbox and an open-task count. Keep saving behavior explicit. Use fake names from materials/meeting-notes.md; no login, AI API or email.

## Instructor script and facilitation

Opening: “An agent can act on files and try the result. We decide the outcome and check whether it happened.” Ask a learner to point to the file that changed. Do not introduce model architecture, context windows or terminal internals today.

At minute 10: “A skill packages a way of working. It can tell the agent to interview us before building.” Open the installed skill, point to its name and description, and explain that we are using the course's explicit standalone adaptation. Show that we installed one skill, not a new agent.

At minute 20, say only: “I want help with meeting notes.” Use the classroom interview prompt. Give concrete answers: a volunteer coordinator, manual action entry, three fake tasks, no accounts, no sending messages. Let a learner decide whether data must survive refresh. That choice materially affects the build.

At minute 35, ask students to name the user and one out-of-scope feature. If their interview is unfinished, request a summary with open questions and explicitly choose whether to clarify or accept a small brief. Do not silently let the agent guess.

At minute 45, send the build prompt in a new message. While it runs, students write the actions they will perform to judge it. Read a permission request in ordinary language: what will run and where it will write.

At minute 65: “Let's use it as someone who did not watch it being built.” Add a task, mark it complete and try a blank task. Record observations before asking for improvements. If everyone is successful, use the mistake card about refresh behavior and explain that this may be a requirement mismatch rather than a coding defect.

## What to watch for

- Ask the learner to demonstrate: Explain that an agent can inspect files, make changes, run work and check results within its available permissions.
- Ask the learner to demonstrate: Describe a skill as a reusable set of workflow instructions, sometimes with supporting files.
- Ask the learner to demonstrate: Turn one vague idea into an approved brief, a first version and one inspected improvement.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect brief.md, a working local artifact, run/open instructions and one completed inspection-log entry.
