# Week 2 copy-paste prompts

Paste these into **agent chat**, not the terminal. Use **one prompt at a time**. Codex is primary; Claude Code can use the same plain-language prompts with its own MCP connect UI.

**No Gmail. No secrets. Local Sticky Notes only.**

## 1 — Brief

```text
I am not a developer. Help me design a tiny local MCP server called "sticky-notes".
Tools: list_notes, add_note(text), search_notes(query).
Store notes in notes.json in this project. No accounts, no cloud APIs.
Explain each file you will create in one plain sentence before writing code.
Stop after the plan; wait for my yes.
```

## 2 — Build

```text
Build the sticky-notes MCP from the approved plan.
Include clear run/connect instructions for Codex on my machine.
After building, tell me exactly what to click/type to connect it, then stop.
```

## 3 — Prove

```text
Call add_note with "buy oat milk", then list_notes, then search_notes for "milk".
Show me the tool results and the path to notes.json. Do not claim success without those.
```

## 4 — Break/fix (after a tool was renamed or notes.json was emptied/removed)

```text
Expected: list_notes returns my notes. Actual: [paste error or empty result].
Find the smallest fix. Do not rebuild from scratch. Then re-run list_notes.
```

## Optional — Stretch tool

```text
Add one more tool: count_notes (returns how many notes exist) OR delete_note(query_or_id).
Keep storage in notes.json. Explain the change in one sentence, then implement and show me how to test it.
```
