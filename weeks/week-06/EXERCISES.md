# Week 6 exercises

Work in your own project under `workspace/projects/`. Use synthetic data only. Copy blank worksheets from [templates](../../templates/README.md).

## Hands-on exercise

1. Read the data dictionary and calculate the expected open/completed counts manually.
2. Ask the agent to explain the schema and inspect dirty-actions.json without modifying it.
3. Write an automation contract specifying inputs, output, validation and duplicate rules.
4. Implement a local draft report in your existing project using the simplest available tooling.
5. Inspect the success, empty and unavailable-source API fixtures; label them as simulated responses.
6. Run the workflow twice with the same input and verify no duplicate report entries.
7. Test a missing owner, duplicate ID, invalid date and missing input file.
8. Save failure evidence and explain how you would stop an enabled automation. Leave any real schedule disabled unless separately authorised.

## Minimum completion

A correct local report, a repeat run without duplicates, one observed failure path and an automation contract. The API lesson can be completed entirely with fixtures.

## Stretch exercise

With explicit instructor approval, replace only the input reader with a documented public read-only API. Keep the same validation, timeout, rate-limit handling and fixture fallback. Record what changed.

## Homework: 20–30 minutes

Write a contract for one repetitive job from your life using fake inputs. Run a draft twice manually. Do not enable a schedule, send messages or add real credentials as homework.

## Submit or show

Draft report, input-validation evidence, repeat-run evidence and an automation contract with scheduling status.

You may demonstrate live or share a sanitized screenshot and short note. Do not upload raw chats, real credentials or private work materials.
