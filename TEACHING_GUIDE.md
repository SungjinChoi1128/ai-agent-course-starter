# Teaching guide

## Prepare before the first class

Allow 30–45 minutes of setup support outside the 90-minute lesson. Confirm each learner's device, operating system, working coding-agent login, and ability to open a local folder. Keep account setup separate from the Git/skill bootstrap.

Rehearse [SETUP.md](SETUP.md) on one Codex machine and the learner's Claude Code surface. Confirm that the interview file is discoverable and that the first question can be asked. Download a local copy of this repository and keep [the sample brief](materials/demo-brief.md) available if the network fails.

Use a clean teaching workspace with no client files, personal browser profiles on screen, or real credentials. Prepare a local meeting-action tracker from the demo brief before class as a fallback; the live demo can still start from an empty project. Save a known-working copy before W5.

## What to say at the start

“Today you will direct an AI that can work on files and try things. Your job is to make the goal clear and check the result. It can make mistakes. We will learn how to notice them.”

Then show an actual file created by a small request. Avoid a tour of every button. Explain only the next action the learners need.

## Facilitation for three learners

Use names in a private attendance sheet, not in this public repository. At the start, each learner reports: what I tried, what I observed, what is unclear. Keep it to one minute each.

During solo work, give each learner a three-minute check-in. Ask “Show me the result” before reading their entire chat. During peer review, assign a driver who controls the computer, a user who attempts a task, and an observer who records confusion. Rotate so the strongest computer user does not take over.

Ask the Claude Code learner to share the same result as the Codex users. Do not equate slash commands, dollar-name skill references, chat prompts, and shell commands. [The invocation guide](SETUP.md#codex-and-claude-code) gives the current distinctions.

## Teaching the interview

Let the agent ask one question, let the student answer, then pause to identify the decision that answer settles. If the student says “easy to use,” ask them to describe one action a user should complete.

If an interview runs long, explicitly request an early summary with open questions and unresolved risks. Do not portray a time limit or an ambiguity score as proof that the requirements are complete. Use the small fallback brief when needed; the student still reviews and approves it before building.

Keep interview and build as two separate messages. This helps students see that writing requirements is an action with a useful output.

## Demo discipline

Use one visible goal and one visible success check. Announce the file or folder in scope. Read proposed install commands in plain language, then use the app's normal approval control. Do not teach students to disable safeguards to make the demo faster.

Narrate waiting productively: have learners predict what will appear and write down how they will test it. If a tool runs longer than five minutes, switch to the saved example while it finishes. If usage limits stop the agent, move to paper inspection or peer testing and finish the build later.

## Handling common moments

| Moment | Instructor response |
| --- | --- |
| “The AI says it is done.” | “Show us one check you performed yourself.” |
| “I don't know what to ask.” | “Describe the last time the problem happened.” |
| Student pastes real client material | Stop sharing; replace it with synthetic data. Follow the organisation's process if disclosure occurred. |
| Agent requests a big installation | Ask what needs it and whether the accepted goal can be met with the existing tools. |
| Output looks impressive but is wrong | Record expected versus actual before asking for a change. |
| One learner finishes early | Give them the observer role or an edge-case exercise. |
| Agent wants OMX commands that do not exist | Use the documented course compatibility prompt; do not install the full framework mid-class. |

## Weekly prep and completion

Read the week's INSTRUCTOR file, rehearse the demo, and prepare its fixtures. At the start of W3 onward, ask a learner to restart their project from their own instructions. At the end, collect only sanitized evidence: a brief, one inspection record, or a demo link the learner chose to share.

Homework feedback should name one useful decision and one next check. Avoid grading vocabulary or the amount of code generated.

## Maintenance before a new cohort

Check [Sources](materials/SOURCES.md), the official skill paths, the pinned upstream revision, and each agent's current help or skill selector. Run the bootstrap in a temporary workspace. Record actual platform coverage in [Validation](VALIDATION.md). Updating documentation is appropriate; installing all of OMX is a separate course design decision.

Keep a version or commit of the course used for each cohort. If you improve prompts during a lesson, record the change afterwards and keep the learner-facing instructions consistent.
