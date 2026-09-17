# AI Coding-Agent Course Starter

Eight practical, 90-minute sessions for four non-technical professionals. **Codex is primary.** No programming background required.

**Course promise:** turn a real, small problem into something useful — with skills, MCP tools, inspection, and a safe handover.

> Vague idea → interview → build → connect tools (MCP) → inspect → improve → hand over

## Start here

**Teaching today? Open [Start today's lesson](FIRST_LESSON.md).** After Week 1, open the **current week** (Week 2 = Sticky Notes MCP end-to-end).

1. Instructor: read [Teaching Guide](TEACHING_GUIDE.md) and complete the setup rehearsal before class.
2. Everyone: follow [Setup](SETUP.md). If Git is missing, start with the [bootstrap prompt](prompts/00-bootstrap.md) in your already-installed coding agent.
3. Week 1 is historical completed content. For today's class, open [Week 2](weeks/week-02/README.md) (Sticky Notes MCP with Codex).
4. Keep your work in `workspace/projects/` and your reflections in `workspace/notes/`. These are ignored by Git in this teaching repository.
5. Come back next week with one thing that worked and one thing you could not yet verify.

Git is the local version-history tool. GitHub is the website for sharing repositories. A GitHub account is optional for the first lesson; your coding-agent account and access must already work.

## Eight weeks

| Week | Theme | Leave with |
| --- | --- | --- |
| [1](weeks/week-01/README.md) (done) | Agents, skills, Deep Interview, GitHub | Brief + first build |
| [2](weeks/week-02/README.md) (today) | MCP end-to-end — Sticky Notes | Working local MCP + proof it was called |
| [3](weeks/week-03/README.md) | Ship a small app (interview → GitHub) | Personal utility from a brief, in GitHub |
| [4](weeks/week-04/README.md) | Make it trustworthy | 3 manual checks + one verified fix |
| [5](weeks/week-05/README.md) | Skill + MCP workflow | Skill gathers intent; MCP does the live action |
| [6](weeks/week-06/README.md) | Real service, read-only, least access | One safe read-only connection |
| [7](weeks/week-07/README.md) | Weekly job + stop switch | Repeatable run without duplicates |
| [8](weeks/week-08/README.md) | Capstone demo + peer handover | Working demo others can run with author silent |

See [Course Overview](COURSE_OVERVIEW.md) for progression and assessment.

## Repository map

- `weeks/week-01/` … `weeks/week-08/`: agenda and outcomes in `README.md`, instructor scripts in `INSTRUCTOR.md`, exercises and homework in `EXERCISES.md`, copy-paste prompts in `PROMPTS.md`.
- `prompts/`: bootstrap, interview compatibility instructions, and everyday reusable prompts.
- `materials/`: synthetic notes, data fixtures, demo brief, troubleshooting and safety cards, capstone ideas, and source notes.
- `templates/`: blank briefs, inspection logs, bug reports, automation contracts, and handovers.
- `workspace/`: a local practice area, with guidance for creating separate project repositories.
- `sessions/`: historical class records (do not delete).

Week 1 used a meeting-action tracker as a running example. From Week 2 the focus is practical builds (Sticky Notes MCP first). Learners may still use fixtures in `materials/` as safe fake data. **No Gmail or secrets in Week 2.**

## Reuse or teach the course

Use GitHub's **Use this template** option for your own teaching copy, or download the ZIP from the Code menu. Cloning this public repository is also fine:

```sh
git clone https://github.com/SungjinChoi1128/ai-agent-course-starter.git
```

Run that command only after Git works. Open the resulting folder in your coding agent. A clone still points to this instructor repository; do not push student work there. The bootstrap explains how to keep work local or use a separately owned repository.

Default workload: 90 minutes in class plus 20–30 minutes of homework. Required early weeks use local fake data. No paid API or full OMO/OMX installation is required. Week 6's real-service step stays read-only with least access.

## Deep Interview provenance

The requested “OMO Deep Interview” is sourced from the official [oh-my-codex (OMX) repository](https://github.com/Yeachan-Heo/oh-my-codex), specifically `skills/deep-interview/`. OMO and OMX are different projects; this course uses the requested **oh-my-codex** source.

The bootstrap downloads only that skill into the chosen skill location, with its license and provenance. It does not install the entire toolkit. Current upstream instructions contain OMX runtime dependencies; [the course compatibility prompt](prompts/01-deep-interview.md) explicitly adapts those parts for a standalone classroom interview. This is not a claim that the full OMX runtime works in Claude Code or Codex Desktop.

Setup guidance checked on 2026-09-07. [Sources and maintenance notes](materials/SOURCES.md) explain the pinned revision and what instructors should recheck. Original course content is available under [MIT](LICENSE).
