# Everyday prompts

Paste into agent chat and replace brackets.

## Resume with context

```text
Read [BRIEF], [RUNBOOK] and [LATEST INSPECTION LOG] in [PROJECT].
Summarize the current goal, working behavior and unresolved issue.
My next requested change is [ONE CHANGE]. Preserve the accepted constraints.
```

## Explain without changing

```text
Explain [FILE, COMMAND OR ERROR] in plain language using the actual project.
Separate facts from assumptions. Do not change files or run mutating commands.
```

## Ask before guessing

```text
If missing information would materially change the result, ask me one focused
question. Inspect discoverable project facts yourself. Do not invent my
preferences or silently expand the scope.
```

## Stop and hand over

```text
Stop making changes. Summarize completed work, actual checks, unfinished work
and the exact next step. Include relevant file locations without secrets.
Do not claim completion for anything you have not verified.
```

## Recover an unintended edit

```text
Inspect the unintended change in [EXACT FILE/PROJECT]. Explain its scope and
available recovery options using existing history or backups. Do not reset,
delete, overwrite or discard other work until I approve an exact recovery.
```
