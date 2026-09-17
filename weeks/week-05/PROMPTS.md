# Week 5 copy-paste prompts

## Design the chain

```text
I have a NotebookLM MCP (or approved live MCP) with the live MCP tools you already connected.
Help me design a short skill that asks 2–3 questions, then tells me exactly which MCP tool to call and with what arguments.
Do not write code yet. Show the skill outline in plain language.
```

## Build the skill

```text
Create a project skill file for the approved outline.
The skill must NOT embed secrets or call cloud APIs.
It should end by instructing the agent to call the NotebookLM MCP (or approved live MCP) tool.
Show me where the skill file lives and how to invoke it in Codex.
```

## Prove the chain

```text
Run the skill workflow for this scenario: [SCENARIO].
Then call the MCP tool it specifies. Show tool results and open the live result (notebook counts, insight file, or equivalent) so I can verify.
```
