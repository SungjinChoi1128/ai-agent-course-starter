# Week 6 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Inspect the data

```text
Read materials/data/README.md and the JSON fixtures. Explain the fields and expected results. Identify duplicates, missing required fields, invalid values and any assumptions. Keep source files unchanged. Use only synthetic data.
```

## Explain API behavior

```text
Use materials/api/README.md and its local JSON fixtures to explain a request, a successful response, an empty response and an unavailable source. These are simulations, not live calls. Describe what the report should do in each case and what must not be assumed.
```

## Build a draft workflow

```text
In [PROJECT PATH], build a manually triggered local report using [INPUT PATH] and the approved automation contract. Write a draft only; no email, uploads, real API writes or scheduler. Validate inputs, preserve source data, report rejected records and prevent duplicate entries on repeated runs. Document how to start and stop it. Test normal, empty, duplicate and missing-input cases.
```

## Review repeatability

```text
Run or guide me through two executions with the same input. Compare outputs and check for duplicates or unintended writes. Then simulate an unavailable source. Report actual observations, partial results and what a scheduled version would still need. Do not enable a schedule.
```
