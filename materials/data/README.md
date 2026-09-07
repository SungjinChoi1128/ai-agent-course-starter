# Synthetic action data

JSON fixtures avoid requiring a spreadsheet library. Preserve these source files.

## Schema

Each input is an array of action objects.

| Field | Meaning | Rule |
| --- | --- | --- |
| id | Stable action identifier | Required nonempty string |
| title | What to do | Required nonblank string |
| owner | Responsible fictional person | Nonempty string or null; null means Unassigned |
| due | Due date | Valid calendar date in YYYY-MM-DD format |
| completed | Whether finished | Boolean true or false, not text |

## Expected results

[actions.json](actions.json): 4 valid unique records, 3 open and 1 completed. Open owners: Alex 2, Sam 1. Jo's completed task is excluded from the open-actions report. Do not classify overdue items using the real current date; if needed use a declared reference date.

[empty-actions.json](empty-actions.json): 0 records; display “No open actions,” not an error.

[dirty-actions.json](dirty-actions.json): 5 rows. Row 1 is valid; row 2 exactly duplicates its ID and contents, so keep one. Row 3 is valid with owner null and should be labelled Unassigned. Row 4 has an invalid date. Row 5 has a blank title and a string completed value. Accept 2 unique records, deduplicate 1 identical row, reject 2 rows with reasons. Both accepted records are open.

For a conflicting duplicate (same ID, different contents), flag the conflict for human resolution rather than choosing an arbitrary winner. The exercise can create that case in a local working copy.
