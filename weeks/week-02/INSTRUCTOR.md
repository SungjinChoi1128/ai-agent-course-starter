# Week 2 instructor notes

## Preparation (≈20 min before class)

- Rehearse once on a clean Codex project: create Sticky Notes MCP → connect → call `add_note` then `list_notes` → open `notes.json` → break one thing → fix.
- Preferred live build: local Sticky Notes with `list_notes`, `add_note(text)`, `search_notes(query)` → `notes.json`. **No accounts, no cloud APIs, no Gmail.**
- Fallback: demo on your machine; learners write brief + success checks on paper; finish connect as homework.
- Whiteboard line: **Skill = reusable instructions. MCP = live tool plug. Today we build the plug.**

## Open (≤2 min)

“Last time we used *skills* — written instructions the agent reuses. Today we add *MCP*: a plug that lets the agent use a live tool outside the chat. We’ll build one with Codex, connect it, and prove it works.”

## Plain-language talking points (8–18)

- **MCP (plain):** a **plug** that lets the coding agent use a tool or data source outside the chat.
- **Name once:** MCP = Model Context Protocol (learners do not need the full name to use it).
- **Skill:** saved recipe of written steps. Good for interviews and briefs.
- **MCP:** live capability. Good when the agent must **do** something or read changing data.
- **Rule of thumb:** If the answer can live in a markdown file, start with a skill. If the agent must act on live data or another system, you need a plug.
- **Safety out loud:** Do not connect personal work email or client data today. Read every permission request. “The agent said it worked” is not proof — open the file.

## Demo idea (18–28)

Drive Codex yourself. Build Sticky Notes MCP. Approve installs. Call `add_note` with a harmless phrase, then `list_notes`. Have learners predict which file changes, then open `notes.json` together.

## Facilitation

- **28–40:** Hand out the three success checks from the README. Each learner picks a theme (work tasks / meal ideas / lesson ideas).
- **40–70:** Circulate; unblock install/config only; do not hijack keyboards. Point them at [PROMPTS.md](PROMPTS.md) one prompt at a time.
- **70–82:** Deliberately break one thing (rename a tool or empty/delete `notes.json`). Learners reproduce, write expected vs actual, ask for a minimal fix, recheck.
- **82–90:** Two learners show one successful tool call. Collect exit sentences.

## What to watch for

- Learners paste API keys or connect personal Gmail → stop; local Sticky Notes only.
- Agent “finishes” without a file change → insist they open `notes.json`.
- Wrong MCP path / not restarted → restart Codex after connect.
- Early finisher → observer role or stretch `delete_note` / `count_notes`.
- Claude Code learner → same artifact and checks; different connect UI is fine.

## Debrief

Ask: “What did MCP give you that a skill alone could not? What did you observe? What remains uncertain?” Collect working MCP (or paper brief), tool-call evidence, and the one-sentence why.
