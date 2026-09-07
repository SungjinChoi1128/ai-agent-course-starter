# AI Coding-Agent Course Starter

Eight practical, 90-minute sessions for three non-developers: two using Codex and one using Claude Code. No programming background required.

**Course promise:** turn a real, small problem into something useful, inspect what the agent did, and improve it with evidence.

> Vague idea → interview → build → inspect → improve

## Start here

**Teaching today? Open [Start today's lesson](FIRST_LESSON.md).**

1. Instructor: read [Teaching Guide](TEACHING_GUIDE.md) and complete the setup rehearsal before class.
2. Everyone: follow [Setup](SETUP.md). If Git is missing, start with the [bootstrap prompt](prompts/00-bootstrap.md) in your already-installed coding agent.
3. Open [Week 1](weeks/week-01/README.md). Copy one prompt at a time and answer the interview yourself.
4. Keep your work in `workspace/projects/` and your reflections in `workspace/notes/`. These are ignored by Git in this teaching repository.
5. Come back next week with one thing that worked and one thing you could not yet verify.

Git is the local version-history tool. GitHub is the website for sharing repositories. A GitHub account is optional for the first lesson; your coding-agent account and access must already work.

## Eight weeks

| Week | Practice | Leave with |
| --- | --- | --- |
| [1](weeks/week-01/README.md) | Agents, skills, Deep Interview | A brief and a first working version |
| [2](weeks/week-02/README.md) | Context, goals, constraints, success criteria | A clear, testable project brief |
| [3](weeks/week-03/README.md) | Workspaces, files, terminal, repos, dependencies | A project you can locate and restart |
| [4](weeks/week-04/README.md) | Build–inspect–improve | Two evidenced improvements |
| [5](weeks/week-05/README.md) | Errors and hypotheses | A reproduced, explained, verified fix |
| [6](weeks/week-06/README.md) | Data, APIs, automation | A repeatable, safe draft-report workflow |
| [7](weeks/week-07/README.md) | Trust, diffs, tests, secrets, destructive actions | A release decision supported by evidence |
| [8](weeks/week-08/README.md) | Capstone | A working demo and usable handover |

See [Course Overview](COURSE_OVERVIEW.md) for progression and assessment.

## Repository map

- `weeks/week-01/` … `weeks/week-08/`: agenda and outcomes in `README.md`, instructor scripts in `INSTRUCTOR.md`, exercises and homework in `EXERCISES.md`, copy-paste prompts in `PROMPTS.md`.
- `prompts/`: bootstrap, interview compatibility instructions, and everyday reusable prompts.
- `materials/`: synthetic meeting notes, data and API fixtures, demo brief, troubleshooting cards, safety cards, capstone ideas, and source notes.
- `templates/`: blank briefs, inspection logs, bug reports, automation contracts, and handovers.
- `workspace/`: a local practice area, with guidance for creating separate project repositories.

The running example is a meeting-action tracker. Students may choose a packing checklist or reading tracker with the same small scope.

## Reuse or teach the course

Use GitHub's **Use this template** option for your own teaching copy, or download the ZIP from the Code menu. Cloning this public repository is also fine:

```sh
git clone https://github.com/SungjinChoi1128/ai-agent-course-starter.git
```

Run that command only after Git works. Open the resulting folder in your coding agent. A clone still points to this instructor repository; do not push student work there. The bootstrap explains how to keep work local or use a separately owned repository.

Default workload: 90 minutes in class plus 20–30 minutes of homework. All required exercises use fake data and can remain local. No paid API, public deployment, or full OMO/OMX installation is required.

## Deep Interview provenance

The requested “OMO Deep Interview” is sourced from the official [oh-my-codex (OMX) repository](https://github.com/Yeachan-Heo/oh-my-codex), specifically `skills/deep-interview/`. OMO and OMX are different projects; this course uses the requested **oh-my-codex** source.

The bootstrap downloads only that skill into the chosen skill location, with its license and provenance. It does not install the entire toolkit. Current upstream instructions contain OMX runtime dependencies; [the course compatibility prompt](prompts/01-deep-interview.md) explicitly adapts those parts for a standalone classroom interview. This is not a claim that the full OMX runtime works in Claude Code or Codex Desktop.

Setup guidance checked on 2026-09-07. [Sources and maintenance notes](materials/SOURCES.md) explain the pinned revision and what instructors should recheck. Original course content is available under [MIT](LICENSE).
