# Week 5 instructor notes

## Preparation

Save a working checkpoint or copy. Prepare materials/debugging-cards.md. Use an actual observed problem if available; introduce a known reversible defect only in a disposable teaching copy.

## Demo idea

Wrong-folder restart for the quick example; incorrect open-task count for the deeper exercise. Use the debugging cards to distinguish environment failures from behavior defects.

## Instructor script and facilitation

Say: “An error is an observation. A cause is an explanation we have to check.” Show a failed restart from the wrong folder. Copy only the relevant error text, removing private paths if sharing outside class.

Ask the group for three possibilities: wrong current folder, a missing file, or an outdated run instruction. A directory check can distinguish them without editing code or reinstalling anything.

Then demonstrate a behavior problem: a completed task remains in the open count. In a disposable copy, use the bug-seeding prompt to introduce only that known mismatch and record what changed. The learner sees the symptom; the instructor keeps the answer key.

At minute 25, require each hypothesis to predict an observable result. “The AI made a mistake” does not tell us what to check. Encourage a small read-only check before a fix.

During investigation, preserve the original error and avoid a stream of speculative changes. If the first explanation is disproved, update the hypothesis list. If a dependency or environment is the cause, do not rewrite the application as a workaround.

At minute 60, the same steps must fail before and pass after. If the problem is in code, ask for a small regression test when an existing test setup can support it, and still perform a manual check. No need to install an entire testing framework during class.

End by having the learner explain the cause in two sentences: what happened, and which evidence supports it. “It works now” is not yet a cause.

## What to watch for

- Ask the learner to demonstrate: Write expected versus actual behavior and reproducible steps.
- Ask the learner to demonstrate: Compare three plausible explanations using evidence before changing code.
- Ask the learner to demonstrate: Verify a minimal fix and recheck a previously working behavior.

Use the same acceptance standard for Codex and Claude Code. If a tool-specific command is unavailable, use natural language and the current product's supported surface; do not invent a command.

## Debrief

Ask: “What did you decide? What did you observe? What remains uncertain?” Collect bug report, hypothesis table, cause explanation and fix verification or a precise blocker.
