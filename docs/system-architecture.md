# System Architecture — Tomboj Studio

Tomboj Studio is designed as a private operating system for AI-assisted content workflows.

This document summarizes the public-facing architecture concept. It does not include private source code, credentials, deployment details, or production data.

## Architecture Principle

The system separates three layers:

1. **Human decision layer**
   The user approves, redirects, reviews, and confirms.

2. **Application state layer**
   Studio stores content state, workflow stage, revisions, events, metrics, and goals.

3. **Agent work layer**
   AI agents read from and write to Studio through structured APIs, leaving visible traces of their work.

## Core Data Objects

### Cards

A card represents one content asset.

A card may include:

* Identity
* Title
* Format
* Stage
* Target post time
* Brief
* Current draft
* Waiting-on status
* Published URL
* Performance data

### Revisions

Revisions preserve the history of content changes.

They allow the system to track how drafts evolve and how human feedback improves future outputs.

### Thread Messages

Thread messages capture notes, decisions, requests, and context attached to a card.

### Events

Events create an audit trail of what happened.

The system is designed so automated actions do not succeed or fail silently.

### Goals and Metrics

Goals and metrics connect content activity to performance outcomes.

The system is designed to evaluate each identity against its own target, rather than treating all content as the same.

## Views

The same underlying system can be viewed through multiple lenses.

### Today View

The front door for daily triage. Shows what needs attention now.

### Board View

A pipeline view of content state.

Example stages:

* Calendar
* Brief
* Draft
* Edit Loop
* Visuals
* Scheduled
* Published
* Analyzed

### Calendar View

A time-based view of planned, scheduled, and published content.

### Dashboard View

A performance view showing progress against goals, recent results, and trends.

## Agent Collaboration Model

Agents are expected to work through structured interfaces rather than disconnected chat outputs.

An agent can:

* Create a card
* Update a draft
* Add a revision
* Log an event
* Write metrics
* Surface a failure
* Move work to the next state

The human remains responsible for judgment and final approval.

## Trust Model

Tomboj Studio is designed around trust, not just automation.

Trust requirements include:

* No silent failures
* Visible action history
* Clear waiting-on status
* Human approval gates
* Recoverable revision history
* Analytics tied back to content decisions

## Private Implementation

The private implementation is planned around a modern web application stack using a React frontend, Node/Express backend, Postgres database, REST API, and MCP-compatible agent access.

The implementation code is not included in this public repository.
