# Workflow Model — Tomboj Studio

Tomboj Studio is designed around a clear content lifecycle.

The goal is to make every content asset answer three questions:

1. What is this?
2. What state is it in?
3. Whose turn is it?

## Content Lifecycle

A typical content card may move through the following stages:

```text
Calendar → Brief → Draft → Edit Loop → Visuals → Scheduled → Published → Analyzed
```

Blocked work is treated as a visible exception, not hidden inside the main workflow.

## Stage Definitions

### Calendar

The idea or planned content slot exists, but the brief may not be complete.

### Brief

The content direction is defined. The system has enough context to draft.

### Draft

A draft exists and is waiting for review or next action.

### Edit Loop

The draft needs human feedback, AI revision, rerolling, or format changes.

### Visuals

The written asset is ready, but image or creative assets need selection, approval, or finalization.

### Scheduled

The content has been approved and scheduled externally.

### Published

The content is live.

### Analyzed

Performance data has been imported or recorded, and the post can be used for learning.

## Waiting-On Status

Every card should make ownership clear.

Possible states:

* Waiting on human
* Waiting on agent
* Waiting on external action
* No action needed

This prevents the system from becoming another list that has to be manually interpreted.

## Human Actions

The human user can take simple actions:

* Approve
* Add a note
* Request changes
* Reroll
* Change format
* Confirm scheduled
* Confirm published
* Review performance recommendation

## Agent Actions

Agents can support the workflow by:

* Drafting
* Revising
* Summarizing context
* Generating recommendations
* Preparing metrics
* Logging actions
* Flagging failures

Agents do not replace the approval layer. They reduce the coordination burden around it.

## Measurement Loop

Published content should eventually connect back to performance data.

The measurement loop helps answer:

* Which identity is on pace?
* Which posts beat baseline?
* Which formats are working?
* Where is revision effort going down?
* What should be repeated, changed, or stopped?

## Operating Goal

The workflow is designed so the user can open Studio once a day and quickly understand:

* What is live
* What needs attention
* What is blocked
* What is scheduled
* How each identity is tracking

The product succeeds when the user can understand the system state without opening multiple tools or rereading old chats.
