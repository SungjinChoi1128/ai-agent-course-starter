# Teaching guide

## Prepare before the first class

Allow 30–45 minutes of setup support outside the 90-minute lesson. Confirm each learner's device, operating system, working Codex login (primary), and ability to open a local folder. Keep account setup separate from the Git/skill bootstrap.

Rehearse [SETUP.md](SETUP.md) on one Codex machine. Confirm that the interview file is discoverable and that the first question can be asked. Download a local copy of this repository and keep [the sample brief](materials/demo-brief.md) available if the network fails.

Use a clean teaching workspace with no client files, personal browser profiles on screen, or real credentials. Before Week 2, rehearse Sticky Notes MCP end-to-end: Codex builds it, you connect it, you call `add_note` / `list_notes` / `search_notes`, you open `notes.json`. Save a known-working copy as a fallback. **Do not demo Gmail or secrets in Week 2.**

## What to say at the start

“Today you will direct an AI that can work on files and try things. Your job is to make the goal clear and check the result. It can make mistakes. We will learn how to notice them.”

From Week 2, add: “Skills are reusable instructions. MCP is a live tool plug. Today we build the plug.”

Then show an actual file or tool result created by a small request. Avoid a tour of every button. Explain only the next action the learners need.

## Facilitation for four learners

Use names in a private attendance sheet, not in this public repository. At the start, each learner reports: what I tried, what I observed, what is unclear. Keep it to one minute each.

During solo work, give each learner a three-minute check-in. Ask “Show me the result” before reading their entire chat. During peer review, assign a driver who controls the computer, a user who attempts a task, and an observer who records confusion. Rotate so the strongest computer user does not take over.

Ask any Claude Code learner to share the same result as the Codex users. Do not equate slash commands, dollar-name skill references, chat prompts, and shell commands. [The invocation guide](SETUP.md#codex-and-claude-code) gives the current distinctions.

## Week themes (practical arc)

| Week | Focus in class |
| --- | --- |
| 1 | Agents, skills, Deep Interview, first build, GitHub (historical) |
| 2 | Sticky Notes MCP end-to-end with Codex (no Gmail/secrets) |
| 3 | Ship a small personal app from interview to GitHub |
| 4 | Three manual checks + one verified fix |
| 5 | Skill gathers intent; MCP does the live action |
| 6 | Real service, read-only, least access |
| 7 | Weekly job with stop switch; run twice cleanly |
| 8 | Capstone demo + peer handover |

## Teaching skills vs MCP (Week 2+)

- **Skill:** a saved recipe (written steps) the agent can follow again. Good for “how we do deep interviews” or “how we write a brief”.
- **MCP:** a live connection to a capability. Good when the agent must **do** something in another system or read live data — not only follow text instructions.
- **Rule of thumb:** If the answer can live in a markdown file, start with a skill. If the agent must press a button in another app or read changing data, you need a plug (MCP).
- Prefer local Sticky Notes in Weeks 2–5. Treat real email/calendar logins as Week 6 only, read-only, with explicit consent and least permissions.

## Demo discipline

Use one visible goal and one visible success check. Announce the file or folder in scope. Read proposed install commands in plain language, then use the app's normal approval control. Do not teach students to disable safeguards to make the demo faster.

For MCP demos: show the config entry (or Settings → MCP servers), restart/reload if needed, then ask Codex to call one named tool and show the returned data. Insist learners open `notes.json` themselves.

Narrate waiting productively: have learners predict what will appear and write down how they will test it. If a tool runs longer than five minutes, switch to the saved example while it finishes. If usage limits stop the agent, move to paper inspection or peer testing and finish the build later.

## Handling common moments

| Moment | Instructor response |
| --- | --- |
| “The AI says it is done.” | “Show us one check you performed yourself.” |
| “I don't know what to ask.” | “Describe the last time the problem happened.” |
| Student pastes real client material or tries Gmail in W2 | Stop; use local Sticky Notes only. |
| Agent requests a big installation | Ask what needs it and whether the accepted goal can be met with the existing tools. |
| Output looks impressive but is wrong | Record expected versus actual before asking for a change. |
| One learner finishes early | Observer role or stretch (`delete_note` / `count_notes`). |
| MCP will not connect | Check path, command, restart Codex; use instructor fallback MCP. |
| Agent wants OMX commands that do not exist | Use the documented course compatibility prompt; do not install the full framework mid-class. |

## Weekly prep and completion

Read the week's INSTRUCTOR file, rehearse the demo, and prepare its fixtures. At the start of W3 onward, ask a learner to show last week's exit artifact. At the end, collect only sanitized evidence: a brief, tool-call screenshot, inspection record, or a demo link the learner chose to share.

Homework feedback should name one useful decision and one next check. Avoid grading vocabulary or the amount of code generated.

## Maintenance before a new cohort

Check [Sources](materials/SOURCES.md), the official skill paths, the pinned upstream revision, and each agent's current help or MCP settings. Run the bootstrap in a temporary workspace. Record actual platform coverage in [Validation](VALIDATION.md). Updating documentation is appropriate; installing all of OMX is a separate course design decision.

Keep a version or commit of the course used for each cohort. If you improve prompts during a lesson, record the change afterwards and keep the learner-facing instructions consistent.
