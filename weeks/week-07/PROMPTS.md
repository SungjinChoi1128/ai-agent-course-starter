# Week 7 copy-paste prompts

## Contract first

```text
Help me complete an automation contract for this weekly job: [JOB].
Include: trigger, inputs, outputs, duplicate prevention, failure behavior, and a stop switch.
Prefer local draft files. No sending email or deleting data. Wait for my approval before building.
```

## Build dry-run

```text
Implement the approved contract with a dry-run mode that writes a local draft only.
Explain how I run it once, how duplicates are prevented, and how I flip the stop switch.
```

## Prove two runs

```text
I will run the job twice. Help me record outputs and confirm the second run did not duplicate.
Then help me flip the stop switch and show that it refuses to proceed.
```
