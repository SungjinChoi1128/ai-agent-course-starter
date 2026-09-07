# Sample approved brief: meeting-action tracker

Use this as a fallback example, then explicitly approve it before building.

User: a volunteer coordinator following up after a small meeting.
Problem: actions are scattered through notes, so the coordinator misses what is still open.

Build a local tracker with manual task entry, an optional owner, a completion checkbox and an open-task count. Use only fake examples. One page or a similarly simple local interface is sufficient.

Constraints: no paid service, account system, messaging or remote database. Prefer no external dependencies. This first version keeps data only for the current open session; refreshing may reset it. Show that limitation clearly. Persistence is a separate agreed improvement.

Non-goals: extracting actions automatically, sending reminders, sharing across users, calendar sync and authentication.
Agent may choose simple layout and internal implementation.
User keeps decisions about persistence, external services and publication.

## Three checks

1. Enter “Book room” with owner Alex: one open task appears and the open count is 1.
2. Mark it complete: it remains visible as complete and the open count becomes 0; reopen it and the count becomes 1.
3. Submit a blank or whitespace-only task: no empty task is created and helpful feedback appears.

Edge case for later: a task without an owner is allowed and clearly labelled unassigned.

## Example output

- Open: Book room — Alex
- Open: Draft welcome message — Sam
- Completed: Check projector — Jo

Open count: 2.

## Instructor fallback

Before class, build this brief in a disposable local project and verify all three checks. This repository contains the curriculum and fixtures, not a prebuilt tracker application.
