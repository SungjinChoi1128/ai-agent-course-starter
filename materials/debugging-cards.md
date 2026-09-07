# Debugging cards

Use only a disposable copy for intentionally introduced defects.

## Card A: it will not start

Observation: the run command reports a missing file.
Possible explanations: wrong current directory; file absent; runbook names an old file.
First useful check: compare actual current directory and file list with the runbook.
Do not reinstall dependencies before checking these facts.

## Card B: wrong open count

Observation: completing a task changes its appearance, but the open count stays the same.
Possible explanations: count uses all tasks; completion state is not saved; count display is not recomputed.
Useful checks: inspect the stored completion value, compare displayed and manually counted open tasks, then inspect the count update path.
Instructor answer: depends on the defect you actually seeded. Record that change; do not assume every implementation has the same cause.

## Card C: refresh loses data

Observation: tasks disappear on refresh.
Possible explanations: accepted session-only design; missing save logic; failed storage read.
First check: read the approved brief's persistence requirement.
If session-only behavior was agreed, this is a new requirement, not automatically a defect.

## Card D: port already in use

Observation: a local server cannot start on the requested port.
Possible explanations: the same project is already running; another project uses the port; run instructions use a fixed port.
First check: identify the exact listener and owner without killing it.
Use the known project's normal stop control, or select a documented alternate port. Do not terminate unrelated processes.
