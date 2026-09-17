# Course overview

## Audience and destination

Four non-technical professionals who can use files and a browser but have not developed software. **Codex is the primary teaching surface**; a Claude Code learner (if present) uses equivalent natural-language prompts.

By the end, each learner can define a small problem, connect a live tool through MCP, ship a personal utility, inspect and fix with evidence, combine skills with MCP, connect a real service with least access, automate a weekly job with a stop switch, and hand a working demo to a peer. Reading every line of generated code is not a completion requirement. Knowing what the result should do is.

## Learning design

Each week is one end-to-end build with Codex. Introduce a technical term only when the learner needs it to finish the build.

| Week | Theme | Leave with |
| --- | --- | --- |
| 1 (done) | Agents, skills, Deep Interview, GitHub | Brief + first build |
| 2 (today) | MCP end-to-end — Sticky Notes with Codex | Working local MCP + proof it was called |
| 3 | Ship a small app (interview → build → GitHub) | One personal utility from a deep-interview brief, in GitHub |
| 4 | Make it trustworthy | Same app with 3 manual checks + one fix from a failed check |
| 5 | Skill + MCP workflow | Short workflow: skill gathers intent, MCP does the live action |
| 6 | Talk to a real service safely | One read-only connection with least access |
| 7 | Automate a weekly job | Repeatable run with a stop switch (no duplicate mess) |
| 8 | Capstone demo day | Working demo peers can run with author silent |

## Scope across the eight sessions

Week 1 (historical): agent mental model, skill as a reusable workflow, guided interview, first build, inspection, light safety, GitHub basics.

Week 2: plain-language MCP vs skill; build Sticky Notes MCP (`list_notes`, `add_note`, `search_notes` → `notes.json`); connect in Codex; prove a tool call; break and fix.

Week 3: deep-interview a personal utility, build the smallest version, open the result, put it on GitHub (or document what blocked the push).

Week 4: run three manual checks on the Week 3 app; turn one failure into a verified fix.

Week 5: write a short skill that gathers intent, then call the Sticky Notes (or similar) MCP to do the live action.

Week 6: one read-only connection to a real service (calendar / email / drive / local folder) with least access; no write or delete in class.

Week 7: schedule or batch a weekly job (digest, cleanup, reminder) with a stop switch; run twice without duplicates.

Week 8: bounded capstone demo and peer handover with the author silent.

## Session rhythm and group size

Follow each week's minute-by-minute agenda; every agenda totals 90 minutes. Protect at least 35 minutes for learner action and at least 10 minutes for inspection and sharing.

During peer checks, rotate driver, user and observer. Each learner owns their own project. During solo work, circulate in short visits instead of solving one person's project for them.

Ask everyone for the same artifact and behavioral evidence, even if one learner uses Claude Code instead of Codex.

## Assessment without code quizzes

Use a simple 0–2 scale on five dimensions:

| Dimension | 0: not yet | 1: with help | 2: independently |
| --- | --- | --- | --- |
| Intent | Cannot describe the user/outcome | Names user and outcome | Gives a concrete example and boundary |
| Direction | Vague request only | Supplies some context | Supplies constraints and testable criteria |
| Inspection | Accepts agent's claim | Checks the happy path | Checks happy path and a useful edge case |
| Recovery | Repeats “fix it” | Records an error | Uses evidence to compare hypotheses |
| Ownership | Cannot explain the result | Can demonstrate it | Can restart, hand over, and state limitations |

Use the scale for coaching after W1, W4 and W8. Capstone readiness means no zero in inspection or ownership. Learners may submit screenshots, a short recording, or a live demonstration with an inspection log.

## Homework and recovery

Homework takes 20–30 minutes and asks for one small change or evidence artifact. If access or installation fails, accept a completed paper brief and annotated expected behavior. Begin the next class by pairing the learner with the instructor to restore access.

Missing a week: read that week's README, complete the minimum exercise, and bring the exit artifact. Keep stretch tasks optional. Never require a new paid subscription to complete the course. Prefer local/fake data over risky real logins (especially in Weeks 2–5).
