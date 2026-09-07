# Week 5 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Diagnose before editing

```text
In [PROJECT PATH], expected [EXPECTED] but observed [ACTUAL]. Reproduction: [STEPS]. Relevant sanitized error: [ERROR]. Do not edit yet. Propose three plausible hypotheses, state what each predicts, and run safe checks that distinguish them. Report the supported cause and remaining uncertainty.
```

## Explain the error

```text
Explain this sanitized error in ordinary language: [ERROR]. Separate what it explicitly tells us from what we still need to investigate. Give one safe next check and explain why it is useful. Do not suggest reinstalling everything.
```

## Fix the supported cause

```text
The evidence supports [CAUSE] because [OBSERVATION]. Correct that cause in [PROJECT PATH] with the smallest change. Preserve unrelated behavior. Repeat [ORIGINAL REPRODUCTION] and [REGRESSION CHECK]. If an existing test setup is available, add an appropriate small regression check. Report actual results.
```

## Instructor-only bug seed

```text
In this disposable teaching copy only: [EXACT COPY PATH], introduce one reversible defect so that completing a task does not update the displayed open count. First confirm the original project is outside scope. Keep the rest runnable. Record the exact change and recovery steps in an instructor note. Verify the expected symptom. Do not publish or alter the original project.
```
