# Week 2 prompts — NotebookLM research pipeline (MCP)

Paste **one step at a time**. Wait for the learner to say yes / show the result before the next step.
Audience: non-technical. Keep jargon only when this file already names it.

**Hard caps (say out loud):** gather **15–25 sources**, across **at least 4 types**. Stop gathering when you hit the cap — do not keep hunting forever.

**Source types (pick ≥4):**
1. YouTube (video or transcript-friendly link)
2. Online journal / academic article
3. Web article or reputable blog
4. PDF / report / white paper
5. Optional fifth: podcast episode, newsletter, or official docs

## Step 0 — Orient (coach mode)

```
You are my Week 2 lesson coach for a non-technical learner.
Read AGENTS.md and CURRENT_WEEK.md in this project if they exist.
Then read weeks/week-02/PROMPTS.md and wait.
Speak in plain language. One step at a time. Do not skip ahead.
In one or two sentences, tell me what Week 2 is about
(NotebookLM research via MCP, 15–25 mixed sources, cited insights).
Ask me if I am ready to start the lesson.
Do NOT ask for my research topic yet. Do NOT install or gather anything yet.
Stop after I say yes to starting — next is Step 1 (install + auth), not topic.
```

## Step 1 — Install + auth NotebookLM MCP

```
Before any research topic or gathering, set up NotebookLM MCP.

1) Check whether NotebookLM MCP is already connected in Codex
   (list MCP servers / tools; look for notebooklm tools).
2) If it is NOT connected, guide me to run (or run if you can):
   codex mcp add notebooklm npx notebooklm-mcp@latest
   Then restart or reload Codex if the tools do not appear yet.
3) Walk me through Google/Chrome auth in plain language for a non-technical learner:
   - Open the auth / login flow the server asks for
   - Sign in with my Google account in Chrome
   - Approve access when the browser asks
   - Come back to Codex when login finishes
4) Verify tools are visible: list notebooklm tools, or confirm out loud that
   NotebookLM MCP tools appear in Codex.
5) Stop for my yes before we pick a topic or gather sources.

If install or auth fails, use the "Install failed" recovery in this PROMPTS.md
and do not skip ahead to notebook creation.
```

## Step 2 — Topic + success picture

```
Help me pick and lock a personal research topic for this session.
Ask what I want to go deep on; narrow it to something I care about and can finish today
(not a whole career, not "all of AI"). Agree the topic in one sentence.

Then help me write:
1) Who this research is for (me, or a specific person/role)
2) What decision or output I want after the notebook (e.g. teaching notes, a brief, a plan)
3) Three questions I want the sources to help answer

Keep it short. Do not gather sources yet. Stop for my yes.
```

## Step 3 — Research plan (before any gathering)

```
Make a gathering plan for NotebookLM.
Target: 15–25 sources total, at least 4 different source types
(YouTube, journal/article, web article, PDF/report; optional: podcast/newsletter/docs).

Give me a checklist table:
| # | Type | What to look for | Why it helps my three questions |
Aim for a mix — not 20 YouTube links.
Do not search the web yet. Stop for my yes on the plan.
```

## Step 4 — High-volume gather (capped)

```
Execute the approved plan.
Gather sources until we hit 15–25 items AND at least 4 types.
For each source save:
- title
- type
- URL (or file path for a PDF I provide)
- one-line why it might matter
- date accessed

Put the list in sources/source-log.md as you go.
If a link is weak or duplicate, skip it and say why in one line.
When you hit the cap, STOP gathering and show me the count by type.
Do not create a NotebookLM notebook yet.
```

## Step 5 — Quality trim (keep the power, cut the junk)

```
Review sources/source-log.md.
Flag up to 5 weak sources (thin, off-topic, or duplicate).
Propose a final set of 15–25 that still covers ≥4 types.
Ask me which flagged ones to drop. Wait for my choices.
Then rewrite sources/source-log.md to the final list only.
```

## Step 6 — Create the NotebookLM notebook (MCP)

```
Using the NotebookLM MCP (or the connected NotebookLM tools),
create a new notebook named: [short name from my topic].
Add every source from the final sources/source-log.md.
If a source fails to add, record it under "failed" with the error in plain words
and continue with the rest.
When done, show me: notebook name/id, sources added count, failed count.
Do not ask notebook questions yet.
```

## Step 7 — Insight extraction (cited)

```
Ask NotebookLM questions that extract useful insight for my three research questions.
Rules:
- Ask 5–8 questions max this round (not dozens).
- Prefer questions that force comparison, evidence, or "what is disputed".
- For every insight, keep the citation NotebookLM gives (source title or pointer).
- If an answer has no citation, mark it "uncited — do not trust yet".

Write the results to insights/insight-log.md with this shape for each item:
### Insight
- Claim:
- Why it matters for my goal:
- Citation:
- My confidence (high/med/low):

Stop after the insight log is written. Do not build a final brief yet.
```

## Step 8 — Learner check (human in the loop)

```
Quiz me out loud (in chat):
1) Show me one insight I should verify myself.
2) Show me one disagreement or gap across sources.
3) What should I NOT conclude yet?

Wait for my answers. Then update insights/insight-log.md with a short
"human check" section capturing what I said.
```

## Step 9 — Session exit artifact

```
Create outputs/week02-brief.md with:
- Topic (one sentence)
- Source count by type
- Top 5 cited insights (claim + citation only)
- Open questions
- One next action for me this week

Keep it under one page. Then show me the file paths you created today.
```

## Stretch (only if early)

```
Add 1–3 more sources of a missing type only (stay ≤25 total),
re-run two NotebookLM questions that use the new sources,
and append any new cited insights to insights/insight-log.md.
```

## Recovery prompts (instructor pocket)

**Install failed**
```
NotebookLM MCP install or auth did not work. In plain language:
1) What we tried and where it stopped
2) Exact next clicks or commands to retry (or skip for now)
3) Confirm we will finish source-log + drafted NotebookLM questions without MCP,
   and add sources in the NotebookLM UI later
Do not create a notebook via MCP until tools are visible. Stop for my yes.
```

**MCP not connected**
```
NotebookLM MCP is not available. Help me finish everything except notebook creation:
finalize sources/source-log.md and draft the questions I will paste into NotebookLM manually.
List exact clicks I need after class to connect the MCP, in plain language.
```

**Gathering is too slow**
```
We are short on time. Narrow to 15 sources, still ≥4 types,
prefer high-signal over quantity, and finish source-log.md now.
```

**Learner stuck choosing a topic**
```
Offer me 5 personal-topic options based on what I already said in this chat.
Each option: one sentence + why NotebookLM helps. I will pick one.
```
