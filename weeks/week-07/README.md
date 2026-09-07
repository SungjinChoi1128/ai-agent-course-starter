# Week 7: Decide what to trust

Verification, diffs, tests, secrets and destructive actions. 90 minutes, three learners.

## Expected outcomes

- Read a change summary and identify a risky file or action.
- Distinguish an agent claim, an automated test and a personally observed check.
- Make a reasoned release decision with known limitations and appropriate permission boundaries.

## Before class

Use a working project and its existing checks. Open materials/safety-cards.md and templates/release-checklist.md. Use fake secret placeholders only.

## 90-minute agenda

| Time | Minutes | Activity | What learners do |
| --- | --- | --- | --- |
| 0–10 | 10 | Claim versus evidence | Compare 'all done' with a recorded check and its actual output. |
| 10–25 | 15 | Read a diff | Inspect a real small change and name its effect and risk. |
| 25–40 | 15 | Tests and gaps | Run existing checks and identify a behavior they do not cover. |
| 40–55 | 15 | Safety scenarios | Discuss fake secrets, malicious input instructions and broad deletion requests. |
| 55–75 | 20 | Audit your project | Inspect files, outputs, permissions and failure behavior before release. |
| 75–85 | 10 | Peer decision | Give a go/no-go decision supported by evidence and known limitations. |
| 85–90 | 5 | Exit | Name one action that needs explicit approval and one check still missing. |

## Use this lesson

1. Instructor: read [Instructor notes](INSTRUCTOR.md).
2. Learners: open [Exercises and homework](EXERCISES.md).
3. Copy one prompt at a time from [Prompts](PROMPTS.md).
4. Keep evidence using the [templates](../../templates/README.md).

## Exit artifact

A diff explanation, actual test/manual results, a safety-card response and a release decision with limitations.

[Course overview](../../COURSE_OVERVIEW.md) · [Setup](../../SETUP.md)
