# Week 1 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Start the interview

```text
Use the full prompt in ../../prompts/01-deep-interview.md. Replace the idea if needed. Confirm the loaded skill file and apply the standalone classroom instructions. Ask one question at a time; do not build.
```

## Build the approved brief

```text
The interview is complete and I approve brief.md in workspace/projects/my-first-agent-project/. Build the smallest local version that satisfies it. Work only in that project. Keep the accepted non-goals and decisions. Prefer a simple solution with no new dependencies when feasible. Explain any required install before running it. Use fake data, give me exact run/open instructions and report the checks you actually performed. Stop once I can inspect the result.
```

## Inspect together

```text
Help me inspect this result against the three checks in brief.md. Give me one action at a time and the expected result; wait for my observation. Include empty input. Do not tell me it passed until we have evidence.
```

## Improve one thing

```text
Observed: [WHAT HAPPENED]. Wanted: [WHAT SHOULD HAPPEN]. Change only [ONE BEHAVIOR]. Preserve [WHAT ALREADY WORKS]. Recheck the changed behavior and the original three checks. Summarize the change and anything you could not verify.
```
