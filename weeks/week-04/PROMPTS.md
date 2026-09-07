# Week 4 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Prepare an inspection

```text
Read [BRIEF PATH] and the current project. Suggest three short user tasks that would reveal whether it works. Include an empty or unusual state. Give actions and expected results, not a claim that they already pass.
```

## Triage observations

```text
Here are user observations: [NOTES]. Separate likely defects, preferences and future features. For each, explain the consequence. Help me choose one small change with a concrete success check; do not implement yet.
```

## Make a bounded improvement

```text
Observation: [ACTUAL]. Expected: [WANTED]. Change only [BEHAVIOR]. Preserve [BASELINE FEATURES]. Implement the smallest useful correction, then check [OLD CHECK] and [NEW CHECK]. Report what you observed and what still needs my inspection.
```

## Compare before and after

```text
Compare these observations: before [EVIDENCE], after [EVIDENCE]. Did the stated success check improve? Identify regressions or missing evidence. Do not infer success from appearance or from an agent's earlier completion message.
```
