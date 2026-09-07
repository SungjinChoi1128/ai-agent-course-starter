# Sources and maintenance

Guidance checked on 2026-09-07. This course's teaching scripts, examples and rubrics are original instructional materials. Product behavior and upstream skill mechanics are sourced below.

| Topic | Primary source | Use here |
| --- | --- | --- |
| Git installation | [Git installation](https://git-scm.com/install/) | Choose the learner's platform and package route |
| Official OMX identity | [oh-my-codex README](https://github.com/Yeachan-Heo/oh-my-codex) | Distinguish the official project from similarly named forks |
| Skill source | [Pinned Deep Interview](https://github.com/Yeachan-Heo/oh-my-codex/blob/304fb3b4825c4132c273732b14d2d5e86b54f8e3/skills/deep-interview/SKILL.md) | Download the one requested skill |
| Upstream license | [Pinned MIT license](https://github.com/Yeachan-Heo/oh-my-codex/blob/304fb3b4825c4132c273732b14d2d5e86b54f8e3/LICENSE) | Preserve with an installed copy |
| Codex local skills | [Build skills](https://learn.chatgpt.com/docs/build-skills) | Local discovery and explicit skill references |
| Claude Code skills | [Extend Claude with skills](https://code.claude.com/docs/en/skills) | Local discovery, invocation and refresh |

Pinned upstream commit: `304fb3b4825c4132c273732b14d2d5e86b54f8e3`.
Verified source skill inventory: `skills/deep-interview/SKILL.md`.

## Compatibility findings

The upstream skill assumes runtime state commands and downstream OMX workflows. Copying the skill does not install those capabilities. This course retains the original downloaded file and supplies an explicit user-level classroom adaptation in `prompts/01-deep-interview.md`. It uses the interviewing method, then an ordinary approved build request. No full-framework compatibility claim is made.

The package known as OMO in the earlier discussion is not the official repository name used for this installation. Use the exact owner/repository above, not a search result with a similar name.

## Updating this pack

Before changing the pin, inspect the new directory and all its references, preserve its license, repeat extraction and file-hash checks, and smoke-test the adapted interview in both agents. Update every pin occurrence together and record what was actually tested in VALIDATION.md. Do not claim a Windows, Linux or Claude execution test merely from reading documentation.
