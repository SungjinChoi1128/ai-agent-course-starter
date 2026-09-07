# GitHub, Codex and Skills: First Session

**Date:** 2026-09-07 · **Duration:** 42:50 · **Speakers:** Sungjin, Philip, George, and one unidentified fourth voice
**Source:** `C:\Users\phili\Videos\2026-09-07 20-10-28.mp4`
**Pipeline:** whisper-large-v3-turbo (word timestamps) + pyannote 3.1 · talk share: Sungjin 60.7%, Philip 28.4%, George 8.3%, SPEAKER_03 2.7%

> **Speaker note.** Sungjin, Philip and George are identified from the audio itself: George is addressed by name at 14:19 and answers, and Philip identifies himself by naming skills he built. The fourth voice, 2.7% of the talk, is almost certainly Sean, but nobody says his name next to him speaking, so it is left as `SPEAKER_03` rather than guessed at. Confirm and it gets relabelled.

## Summary

The first session of Sungjin's teaching group. He walked Philip, George and the fourth participant through GitHub from scratch: what a repository is, why version control beats a Google Drive folder, commits, local versus remote, pushing, and branching off main to experiment without breaking anything.

The second half was the more interesting half. It moved to agent tooling: what a skill is, the built-in `skill-creator` command, installing and running the `deep-interview` skill (which everyone did live), `AGENTS.md` as standing repo-level rules, chaining skills into workflows, and scheduled tasks including a Gmail integration Sungjin runs at 9am daily.

Homework: build something real with `deep-interview` before the next session.

## Analysis

### Themes and threads

**Storage versus history.** The spine of the first half. Sungjin came back to it three times: GitHub is not a folder that holds your files, it is a record of every change to them. That framing is what makes the commit-and-push ritual make sense rather than feel like bureaucracy.

**Getting the AI to remember.** Every question Philip asked circled the same frustration: he keeps having to tell the model "go back and look at my previous chats". Sungjin's answer was the same every time, in different clothes. Write it down. As a skill if it is a procedure, as `AGENTS.md` if it is a standing rule. That is the actual lesson of the session, and it arrived by accident rather than by design.

**Where a rule lives.** Global instructions versus project-level `AGENTS.md`. Raised sharply, answered vaguely, still open.

**Nobody actually did it.** Skills got installed and `deep-interview` got run, but no commit was made and nothing was pushed, which was the stated goal of the lesson.

### Notable quotes

> "GitHub is actually, every change you make it actually tracks each line and what change you made... so in that sense you can always just revert back to certain points."
> Sungjin, 05:29, the clearest thing said all session

> "If you want the LLM to just remember, you can always just write it down as a skill."
> Sungjin, 21:42

> "This is just the first file that they actually read, so you don't have to remind it."
> Sungjin, 23:37, on `AGENTS.md`

> "I've given instructions that are across the whole Claude, so whether it's a new chat, whether it's a new project or an old project, it will always call me chief."
> Philip, 25:02, setting up the question that never got answered

> "It's the new way. I don't do anything without recording any more, and if I don't I feel so lost."
> Philip, 39:39

> "For the time being I'm just building a transcribe skill that's not involved in work, because my other transcribe skill is deeply embedded in my workflow. So I just want a personal one."
> Philip, 39:18, describing the skill that produced this file

### Honest critique

**The best question of the session got the worst answer.** At 25:02 Philip asked something genuinely sharp: if you can already give an assistant standing instructions that follow you everywhere, what does a project-level `AGENTS.md` actually buy you? Sungjin's reply drifted into "it's more of a software engineering project" and never touched the thing that matters, which is what happens when the global rule and the project rule disagree. Worth re-asking directly next session.

**Sungjin contradicted himself on context.** He warned that `AGENTS.md` "shouldn't be really long because... the LLM can be confused", then immediately undercut it with "but nowadays the model is just too good, so probably it doesn't even". The first instinct was the right one. Long standing-instruction files do degrade behaviour, and telling beginners not to worry about it sets them up to write bloated ones.

**The original confusion never got cleared.** Philip's first question, at 03:08, was whether Codex organises the GitHub repo itself or whether you have to tell it how. Sungjin said "I'm gonna get to it" and did not. Repository versus project was never defined, and that was the gap the whole session was meant to fill.

**A 43-minute session where one person spoke for 61% of it.** Some of that is unavoidable in a first lesson. But the students mostly said "okay" and "nice", and the two times someone shared a screen were the two times anything concrete got fixed. More screen sharing, less narration.

**The homework will not get done as set.** "Build whatever things, small things or big thing" is not an assignment. Compare it to the one concrete instruction that did land, install this skill and run it, which everyone completed inside two minutes.

**Roughly five minutes of the recording is flatmate drama.** Fine for the vibe, but if these sessions get recorded and kept, the signal-to-noise is worth watching.

### Context beyond the recording

> Not from the transcript. Background and judgment added on top.

**`AGENTS.md` is a real open standard, not a Codex quirk.** It is stewarded by the Agentic AI Foundation under the Linux Foundation, developed with OpenAI Codex, Google's Jules, Cursor, Amp and Factory, and is used in over 60,000 open-source projects. The project describes it as "a README for agents". Claude Code's equivalent file is `CLAUDE.md`. Worth knowing that Philip already works in a repo carrying both, so the concept was familiar even though the name was not. ([agents.md](https://agents.md/))

**The precedence answer Sungjin did not give.** For Claude Code specifically, skills live at three levels: personal in `~/.claude/skills/` which apply to all your projects, project in `.claude/skills/` which apply to that project only, and enterprise. When names collide, enterprise beats personal and personal beats project. Project skills also load from every parent directory up to the repo root. That is exactly the global-versus-project distinction the session got stuck on. ([Claude Code docs](https://code.claude.com/docs/en/skills))

**On the model advice.** Sungjin steering people away from the newest, most expensive model and towards the mid-tier is sound. For learning-by-doing, where you run the same thing repeatedly and iterate, the cheaper model gets you more attempts per pound, and attempts are what teach you.

**On what Philip announced at 39:18.** The personal transcribe skill he described in this call is the one that produced this document. First run.
