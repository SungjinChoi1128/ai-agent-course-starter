# Week 8 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Bound my capstone

```text
My capstone idea is [IDEA] for [USER]. Inspect my existing project and help select a version I can finish during a 25-minute build block. Give one concrete outcome, non-goals, three observable checks and one edge case. Ask about unresolved decisions before I approve the brief.
```

## Finish the approved scope

```text
Implement the approved capstone brief at [PATH] in [PROJECT PATH]. Preserve the non-goals and permission boundaries. Use synthetic data. Keep me informed if the scope cannot be completed as agreed; do not silently drop a criterion. Verify the result and provide actual start/open instructions.
```

## Prepare peer testing

```text
Turn the accepted criteria into a short peer-test card. Give only the steps and expected results a new user needs. Include one failure or unusual input. Do not coach the user through the test; leave room to record observations.
```

## Write the handover

```text
Create a handover from the actual project and verification results. Include purpose, intended user, data sources, exact start/stop instructions, success checks with evidence, known limitations, recovery steps and one next improvement. Separate verified behavior from assumptions. Do not publish or claim unsupported compatibility.
```
