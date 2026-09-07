# Classroom Deep Interview

Use this after setup. Enter the prompt in agent chat. Select the installed skill first if the agent supports it; otherwise replace `[SKILL_FILE]` with the verified path from your setup report.

The upstream file remains unchanged. This user prompt explicitly requests a **course adaptation** of that file's interview method. It is needed because the extracted skill contains OMX runtime and handoff instructions that do not become available merely by copying a Markdown file. The adaptation is not endorsed or tested by upstream.

```text
Use the installed Deep Interview skill, or read [SKILL_FILE] if native skill
discovery is unavailable. First confirm which actual file you loaded.

For this lesson I explicitly want a standalone classroom adaptation.
Follow the skill's intent-first questioning, concrete examples, scope,
non-goals, constraints and success criteria. Ask one question at a time
and wait for my answer. Revisit at least one assumption or tradeoff.

Do not invoke omx commands, state/MCP services, other named skills,
or multi-agent workflows. They were not installed for this class.
Use ordinary chat for questions. Keep state in this conversation.
Do not write .omx state or pretend that unavailable tools ran.
If the file cannot be read, say so and ask me to use the fallback below.

Aim for a quick interview with at most five questions. If an important
decision remains unresolved at the cap, identify it and stop for my choice
to continue clarifying or accept the stated uncertainty. Do not invent answers.
If you show an ambiguity score, label it a subjective heuristic, not
a measured guarantee that the project will succeed.

My vague idea: I want something that helps me keep track of meeting actions.

Use only the course's synthetic examples. At the end, draft a short brief
with user, problem, example input/output, must-haves, non-goals, constraints,
decisions I keep, three observable success checks and unresolved questions.
Show it to me. After I approve, save it as brief.md in
workspace/projects/my-first-agent-project/. Do not implement anything.
End the interview and wait for a separate build request.
```

For setup smoke testing, answer the first question and then say “Stop the smoke check; do not write or build anything.” Successful questioning is a useful behavioral check, but it does not prove every upstream feature is supported.

## Fallback without the skill

If the download or skill loading fails, say clearly that this is a teacher-provided interview prompt, not an invocation of the upstream skill.

```text
Run the course's fallback requirements interview; no installed skill is assumed.
My idea is: [ONE SENTENCE].
Ask one concrete question at a time about the person, the problem, an example,
the smallest useful result, and what should stay out of scope.
Challenge one assumption. Stop after at most five questions and summarize
what is known and still uncertain. Give three observable success checks.
Do not build until I review the brief and send a separate build request.
```
