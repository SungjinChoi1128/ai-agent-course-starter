# Week 2 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Find relevant context

```text
I want to add [ONE FEATURE] to [PROJECT PATH]. Inspect the existing brief and relevant files. Identify up to three sources that would change your implementation decisions. Explain why each matters. Do not edit yet. Do not inspect unrelated private folders.
```

## Clarify the brief

```text
Help me complete templates/project-brief.md for [IDEA]. Use the current project as evidence. Ask only about decisions you cannot resolve from the files. Include constraints, non-goals and three checks a non-developer can perform. Mark assumptions and show the draft before implementation.
```

## Implement with boundaries

```text
Implement the approved change described in [BRIEF PATH]. Context: [RELEVANT FILES]. Goal: [USER OUTCOME]. Constraints: [LIMITS]. Non-goals: [EXCLUSIONS]. Success checks: [THREE CHECKS]. Preserve existing behavior outside this change. Show how I can verify the result.
```

## Check prompt quality

```text
Read this request and point out up to three ambiguities that could produce different results: [REQUEST]. Give a concrete example of each. Do not rewrite my intention without asking; propose clearer wording for my review.
```
