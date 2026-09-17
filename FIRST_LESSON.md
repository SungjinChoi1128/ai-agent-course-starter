# Start today's lesson

## Which week is “today”?

- **Week 1** is historical completed content (agents, skills, Deep Interview, first build, GitHub).
- **After Week 1, open the current week.** For this cohort, **today = Week 2: NotebookLM research power session via MCP.**
- Coach pointer: [`CURRENT_WEEK.md`](CURRENT_WEEK.md) → [`AGENTS.md`](AGENTS.md). Learners may say **start lesson** or **continue lesson**.

If you are replaying the first session for a new learner, use the Week 1 path below. Otherwise skip straight to Week 2.

## Instructor: next five minutes (Week 2 — today)

1. Open [Week 2 instructor notes](weeks/week-02/INSTRUCTOR.md).
2. Put [Week 2 agenda](weeks/week-02/README.md) on screen.
3. Confirm each learner can open Codex and has a Google account for NotebookLM.
4. Confirm NotebookLM MCP: `codex mcp add notebooklm npx notebooklm-mcp@latest` (then auth). Have a **demo notebook with 20+ sources** ready.
5. Say the caps: **15–25 sources, ≥4 types.** Fallback: add sources in NotebookLM UI from Codex’s gathered list.

## Say this (Week 2)

“Last time we used *skills* — written instructions the agent reuses. Today we add *MCP*: a plug into NotebookLM. You’ll pick a topic you care about, gather quite a lot of mixed sources, fill a notebook, and keep only **cited** insights.”

Whiteboard line: **Skill = reusable instructions. MCP = live tool plug. Today: NotebookLM — volume + citations.**

## The teaching sequence (Week 2)

- Hook with your pre-built dense notebook; MCP one-liner; auth/connect.
- Topic pick → research plan → **long gather** (biggest block) → trim.
- Create/fill NotebookLM notebook via MCP → 5–8 cited Qs → human check → one-page brief.
- Share one surprising citation. Optional Audio Overview in the UI if time.
- Prompts: [Week 2 PROMPTS.md](weeks/week-02/PROMPTS.md) — one step at a time.

## If you need Week 1 again (new learner catch-up)

1. Open [Week 1 instructor notes](weeks/week-01/INSTRUCTOR.md).
2. Put [Week 1 agenda](weeks/week-01/README.md) on screen.
3. Send learners [Setup](SETUP.md) and [the bootstrap prompt](prompts/00-bootstrap.md).
4. If setup is incomplete, pair on the instructor's machine and use the [fallback interview](prompts/01-deep-interview.md#fallback-without-the-skill).
5. Keep [the sample brief](materials/demo-brief.md) ready if the interview or network stalls.

Say: “Today we'll start with a vague idea, let the agent interview us, build a small version, try it ourselves, and make one improvement.”
