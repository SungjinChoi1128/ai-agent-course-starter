# Week 2 instructor notes — NotebookLM research power session

## Pre-class checklist (do all)

- [ ] Every learner has a **Google account** that can open NotebookLM (browser login works).
- [ ] **NotebookLM MCP** rehearsed once on the instructor machine (learners still do **Step 1** in class):

  ```bash
  codex mcp add notebooklm npx notebooklm-mcp@latest
  ```

  Then restart/reload Codex, run the server’s auth/setup so Chrome login succeeds, and confirm tools appear (list notebooks or equivalent).
- [ ] **Demo notebook** ready with **20+ mixed sources** (YouTube + journals/articles + web + at least one PDF/report) for the opening hook.
- [ ] Fallback ready: if MCP auth fails, learners still finish the **source log** with Codex; add sources in the **NotebookLM UI** from that list after class (or mid-class if time).
- [ ] Whiteboard line: **Skill = reusable instructions. MCP = live tool plug. Today the plug is NotebookLM — volume + citations.**
- [ ] Say the caps out loud: **15–25 sources, ≥4 types. Stop at the cap.**
- [ ] Class path includes learner **Step 1 = install + auth** (not only instructor pre-class).

## Open (≤2 min)

“Last time we used *skills*. Today we use *MCP* to plug Codex into NotebookLM. First you’ll install and sign in (Step 1). Then you’ll pick a topic you care about, gather a lot of mixed sources — not five links — load a notebook, then ask sharp questions and keep only **cited** insights.”

## Hook (0–8)

Show your pre-built dense notebook. Ask: “What would change if you had 20 sources instead of 5?” One-liner: MCP lets the agent **do** something in NotebookLM, not only write advice. Learners run **Step 0 Orient** — agree to start; do **not** jump to topic yet.

## Facilitation map

| Block | Protect | Tip |
| --- | --- | --- |
| **Step 1 Install + auth** | 7 min | Confirm tools visible. If stuck >3 min → recovery “Install failed” or “MCP not connected”; keep later gathering on track |
| Topic + plan (Steps 2–3) | ~15 min | Narrow topics; reject “all of AI” |
| **Gather (Step 4)** | **~25 min** | Biggest chunk. Circulate. Enforce 15–25 and ≥4 types. No notebook yet |
| Trim (Step 5) | 7 min | Cut junk; keep type mix |
| Notebook fill (Step 6) | 13 min | MCP add; log failures; UI fallback from the same list |
| Insights + share (Steps 7–9) | 15 min | Cap at 5–8 questions; insist on citations; one surprising citation aloud |

## Timebox tips

- Install/auth stuck → paste **Install failed** recovery; continue source-log path without MCP.
- Gathering runs long → paste **Gathering is too slow** recovery (narrow to 15, still ≥4 types).
- Early finisher → Stretch prompt only (≤25 total); or help a neighbor as observer.
- Optional Audio Overview in NotebookLM UI only after insight log exists.

## Failure fallbacks

1. **Install / MCP not connected / auth fails:** Use **Install failed** or **MCP not connected** in [PROMPTS.md](PROMPTS.md). Finalize `sources/source-log.md` + draft questions. Add sources in NotebookLM UI from Codex’s list. Still require the brief and human check.
2. **Source fails to add:** Replace it; do not stop early. Record under “failed”.
3. **Topic paralysis:** Use **Learner stuck choosing a topic** recovery.
4. **Agent dumps whole pipeline:** Stop; point at `AGENTS.md` — one step, wait for learner yes. Do not skip Step 1.

## What to watch for

- Skipping Step 1 (install + auth) and jumping to topic/gather → put them back on Step 1 until tools are confirmed or recovery is chosen.
- Stopping at ~5 sources → push back to the cap/mix.
- Paywalled/pirated PDFs or client secrets → stop; public/reputable only.
- “NotebookLM worked” with no counts/citations → not done.
- Skipping trim or human check → put them back on Steps 5 and 8.

## Debrief prompts

“What did volume + mix give you that three Google results would not?”  
“Which insight has the strongest citation? Which is still uncited?”  
Collect: source-log evidence, notebook counts, insight log, one-page brief.

## Recovery prompts (pocket — full text in PROMPTS.md)

- Install failed → plain-language retry or UI path; no MCP notebook until tools visible  
- MCP not connected → finish log + manual NotebookLM path  
- Gathering too slow → 15 sources, ≥4 types, finish log now  
- Topic stuck → 5 personal options, learner picks one  
