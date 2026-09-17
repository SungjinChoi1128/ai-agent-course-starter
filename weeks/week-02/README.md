# Week 2: MCP end-to-end — Sticky Notes

Build a live tool plug with Codex. 90 minutes, four learners. **No Gmail. No secrets.**

## Expected outcomes

- Explain MCP vs a skill in plain words (Skill = reusable instructions; MCP = live tool plug).
- Build a local Sticky Notes MCP with `list_notes`, `add_note`, `search_notes` storing data in `notes.json`.
- Connect it in Codex, call a tool, and prove it with a file or tool result you opened yourself.

## Before class

Bring Week 1 recall (skill, AGENTS.md, first build). Instructor rehearses Sticky Notes MCP once on a clean Codex project. Have a working fallback MCP ready if install stalls.

## 90-minute agenda

| Time | Minutes | Activity | What learners do |
| --- | --- | --- | --- |
| 0–8 | 8 | Recall + hook | Name one thing they built or tried after Week 1; see skill vs MCP side-by-side |
| 8–18 | 10 | Plain model | Write “Skill is ___ / MCP is ___” in their own words |
| 18–28 | 10 | Live demo (instructor drives) | Predict what file will change; watch approvals for Sticky Notes MCP |
| 28–40 | 12 | Brief before build | Pick a notes theme; fill three success checks |
| 40–70 | 30 | Build-along | With Codex: create MCP → connect → call tools → open `notes.json` |
| 70–82 | 12 | Break + fix | Reproduce → expected vs actual → minimal fix → recheck |
| 82–90 | 8 | Share + homework | Show one successful tool call; name what MCP gave that a skill alone could not |

## Three success checks (pass at least 2)

1. Codex lists the MCP tools without you typing the tool names from memory.
2. `add_note` creates or updates a real `notes.json` you can open in the editor.
3. `search_notes` returns a note you added earlier (or clearly says none found).

## Use this lesson

1. Instructor: read [Instructor notes](INSTRUCTOR.md).
2. Learners: open [Exercises and homework](EXERCISES.md).
3. Copy one prompt at a time from [Prompts](PROMPTS.md).
4. Keep evidence using the [templates](../../templates/README.md).

## Exit artifact

- Working Sticky Notes MCP (or instructor-demo + paper brief if blocked)
- Screenshot or short note of one successful tool call
- One sentence: “I needed MCP instead of a skill because ___.”

[Course overview](../../COURSE_OVERVIEW.md) · [Setup](../../SETUP.md)
