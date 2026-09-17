# Week 6 copy-paste prompts

## Plan least access

```text
I want a read-only connection to [SERVICE OR LOCAL FOLDER] for this task: [TASK].
Help me write an allow list and a deny list (no send, no delete, no write unless I explicitly say so).
Do not configure anything yet. Ask me before any OAuth or secret use.
```

## Connect carefully

```text
Help me connect [TARGET] in Codex with the least permissions for a single read test.
Prefer official read-only scopes. Stop and explain any request that can write, send, or delete.
After connect, tell me how to verify with one safe read, then stop.
```

## Prove and document

```text
Perform one read-only check: [CHECK].
Show the tool result. Help me write a short trust boundary: can touch / must not / how to revoke.
Do not store secrets in the repo.
```
