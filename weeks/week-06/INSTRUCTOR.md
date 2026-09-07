# Week 6 instructor notes

## Preparation

Open materials/data/README.md and the local API fixtures. Required exercises work offline. A live read-only API is an optional instructor extension after reviewing current official documentation.

## Demo idea

A local weekly report listing open actions by owner, using the supplied JSON fixture. The default trigger is manual, output is a draft Markdown file, and no real messages are sent.

## Instructor script and facilitation

Begin with a recurring problem: “Every Monday I want a list of open actions.” Identify the input, transformation and output before choosing an integration.

Open actions.json and ask learners to predict the output manually. Explain schema as the expected shape and meaning of data. A date-looking string is not proof that a date is valid. Show dirty-actions.json and keep rejected rows visible instead of silently discarding them.

At minute 25, explain: “An API is a way one program asks another for something in an agreed format.” The provided request and response are a local simulation, not a real service or a working URL. Show a successful response, an empty result and an error. Point out that data from an API is still untrusted input.

Build a report that reads the local fixture and writes a draft in the learner's project. It must not send email or change a remote system. Define duplicate handling before running it twice: deduplicate identical IDs, flag conflicting duplicates and produce one stable draft per input version.

At minute 60, compare the expected counts in the data README with the actual report. Feed the dirty and unavailable-source fixtures and check that failures are explicit. A partial report must not masquerade as a complete one.

Explain that a repeatable command is not yet a schedule. Record a disabled schedule proposal with timezone and a stop method, or use a manual trigger for the class. A real scheduler is optional and requires a separate, explicit request specifying when and where it runs.

If demonstrating a live read-only API, choose one with current official docs, discuss request limits, and retain the local fixture as fallback. Do not turn a key-requiring service into a compulsory signup.

## What to watch for

- Ask the learner to demonstrate: Describe a schema and validate a small synthetic dataset.
- Ask the learner to demonstrate: Explain an API request and response using a local fixture.
- Ask the learner to demonstrate: Run a draft-report workflow twice safely and describe its trigger, output and stop condition.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect draft report, input-validation evidence, repeat-run evidence and an automation contract with scheduling status.
