# Week 3 copy-paste prompts

Paste these into agent chat, not the terminal. Replace bracketed values with your actual project paths and decisions. Use one prompt at a time. Codex and Claude Code can use the same plain-language prompts; [Setup](../../SETUP.md#codex-and-claude-code) covers skill invocation differences.

## Map my workspace

```text
Inspect [PROJECT PATH]. Show the actual project root, important files and their purpose in plain language. Explain which files I edit, which are generated, and whether dependencies are present. Do not install or modify anything.
```

## Explain a command

```text
Before running this command, explain its purpose, working directory, files it can change, network use and whether it needs extra permission: [COMMAND]. If a read-only check can confirm assumptions first, perform that check.
```

## Make a local checkpoint

```text
In [EXACT PROJECT PATH], inspect the repository root and current files. If this project has no independent repository, initialise one here and prepare ignore rules for secrets and generated files. Preserve existing content. Reuse my existing identity; ask for my chosen local identity if needed. Show the staged changes, then create a local checkpoint of this project. Do not push or change global Git settings.
```

## Write restart instructions

```text
Use the actual working project to write runbook.md with prerequisites, exact working folder, start/open steps, expected URL or file, normal stop step and one likely troubleshooting check. Verify the steps you can run and label anything untested.
```
