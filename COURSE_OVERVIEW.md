# Course overview

## Audience and destination

Three adults who can use files and a browser but have not developed software. Codex is the primary teaching surface; the Claude Code learner uses equivalent natural-language prompts and a separate skill-discovery path.

By the end, each learner can define a small problem, direct a coding agent, inspect its files and output, test important behavior, recover from one error, and explain what remains uncertain. Reading every line of generated code is not a completion requirement. Knowing what the result should do is.

## Learning design

Each week introduces one new responsibility for the human. Use the same small project repeatedly so that new tools do not hide the lesson. Introduce a technical term only when the learner needs it to continue.

| Week | Human responsibility | Main artifact | Evidence of learning |
| --- | --- | --- | --- |
| 1 | Decide what matters | Interview brief and first build | Explain one decision the interview changed |
| 2 | Make intent inspectable | Context pack and success criteria | Another person can judge three criteria |
| 3 | Know where work lives | Workspace map and restart instructions | Restart from a closed terminal |
| 4 | Give precise feedback | Before/after inspection log | Show two changes and a regression check |
| 5 | Separate observation from explanation | Bug report and fix evidence | Reproduce before, pass after |
| 6 | Define repeatable inputs and outputs | Draft automation and contract | Run twice without duplicates; handle bad data |
| 7 | Decide what to trust | Verification and release decision | Identify one risk the tests do not cover |
| 8 | Own the outcome | Capstone and handover | A peer can use it with the author silent |

## Scope across the eight sessions

Week 1: agent mental model, skill as a reusable workflow, OMO/OMX naming, guided interview, first build, inspection, light safety.

Week 2: relevant context, a user and goal, constraints and non-goals, examples, three measurable success criteria, handling ambiguity.

Week 3: folders and files, paths, terminal and current directory, repository and local history, dependencies and lockfiles, local versus remote, restart instructions.

Week 4: small changes, observable feedback, preserving working behavior, feedback triage, user checks and iteration logs.

Week 5: expected versus actual, reproduction, exact sanitized errors, three hypotheses, a discriminating check, minimal fix and regression verification.

Week 6: structured data, a schema, API request/response, local fixtures before optional live reads, validation, a repeatable task, dry run, duplicate prevention and stop controls.

Week 7: trust boundaries, diffs, tests versus proof, secrets, untrusted instructions in data, least necessary permissions, deletion and publication decisions.

Week 8: select a bounded capstone, accept the brief, build or finish, peer-test, correct, demonstrate and hand over.

## Session rhythm and group size

Follow each week's minute-by-minute agenda; every agenda totals 90 minutes. Protect at least 35 minutes for learner action and at least 10 minutes for inspection and sharing.

During peer checks, rotate driver, user and observer. Each learner owns their own project. Rotate the three roles every five minutes in the scheduled peer-check block so all three practise judging output. During solo work, circulate in short visits instead of solving one person's project for them.

The Claude Code learner is not expected to copy the Codex screen. Ask everyone for the same artifact and behavioral evidence.

## Assessment without code quizzes

Use a simple 0–2 scale on five dimensions:

| Dimension | 0: not yet | 1: with help | 2: independently |
| --- | --- | --- | --- |
| Intent | Cannot describe the user/outcome | Names user and outcome | Gives a concrete example and boundary |
| Direction | Vague request only | Supplies some context | Supplies constraints and testable criteria |
| Inspection | Accepts agent's claim | Checks the happy path | Checks happy path and a useful edge case |
| Recovery | Repeats “fix it” | Records an error | Uses evidence to compare hypotheses |
| Ownership | Cannot explain the result | Can demonstrate it | Can restart, hand over, and state limitations |

Use the scale for coaching after W1, W4 and W8. Capstone readiness means no zero in inspection or ownership; a polished interface is not a substitute. Learners may submit screenshots, a short recording, or a live demonstration with an inspection log.

## Homework and recovery

Homework takes 20–30 minutes and asks for one small change or evidence artifact. If access or installation fails, accept a completed paper brief and annotated expected behavior. Begin the next class by pairing the learner with the instructor to restore access.

Missing a week: read that week's README, complete the minimum exercise, and bring the exit artifact. Keep stretch tasks optional. Never require a new subscription to complete the course.
