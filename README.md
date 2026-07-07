# Tomboj Studio Overview

Tomboj Studio is a private AI-assisted content operations system designed to manage multi-brand LinkedIn workflows from one daily operating surface.

This repository is a public product overview and portfolio artifact. It does not contain the private Tomboj Studio application codebase.

## What Tomboj Studio Is

Tomboj Studio is designed to be the home base for a multi-brand content engine.

The product brings together:

* Content planning
* Draft review
* Approval workflows
* Revision history
* Calendar visibility
* Performance tracking
* AI-agent collaboration
* Human-in-the-loop decision points

The goal is simple: open one tab, understand what needs attention, approve or redirect the right items, and move on.

## Product Principle

Studio is a database with a good face.

Agents can work in the system constantly. The human user should only need to check the surface briefly, understand the state of everything, and act on the few items that need judgment.

## The Problem

Content operations can become messy quickly when multiple brands, formats, goals, and AI tools are involved.

Common problems include:

* Drafts living in too many places
* No clear state for each piece of content
* Unclear ownership between human and AI
* Revision history getting lost
* Approved content becoming disconnected from analytics
* AI outputs improving slowly because feedback is not structured
* Too much manual effort to know what is ready, blocked, scheduled, or performing

Tomboj Studio is designed to solve the operating layer around AI-assisted content creation.

## Core Concepts

### One Card Per Content Asset

Each content idea, draft, article, carousel, or post lives as a card.

A card can carry:

* Identity
* Format
* Stage
* Target post time
* Brief
* Current draft
* Revision history
* Thread notes
* Asset links
* Approval state
* Published URL
* Performance data

### Multiple Lenses Over One System

The same underlying content data can be viewed through different surfaces:

* Today view
* Board view
* Calendar view
* Dashboard view
* Card detail overlay

### Human-in-the-Loop Approval

The system is not designed to remove the human. It is designed to reduce low-value coordination work while preserving human judgment at important gates.

Examples:

* Approve a draft
* Request changes
* Reroll a concept
* Change format
* Confirm something is scheduled
* Confirm something is published
* Review performance recommendations

### Agent-Visible System of Record

AI agents need a structured place to work.

Tomboj Studio is designed so agents can:

* Read card state
* Create or update drafts
* Add revisions
* Log actions
* Surface failures
* Write metrics
* Use the same service layer as the app

Every automated action should leave a visible trace.

## Intended Workflow

A typical daily workflow:

1. Open Tomboj Studio.
2. Review the Today view.
3. See what needs attention.
4. Approve, note, reroll, or redirect.
5. Confirm scheduled or published items.
6. Review any live performance signals.
7. Close the tab.

The product is designed around a short daily operating ritual, not constant manual management.

## Planned Sections

### Today

The daily front door. Shows what needs attention first.

### Board

A pipeline view for content state, such as Calendar, Brief, Draft, Edit Loop, Visuals, Scheduled, Published, and Analyzed.

### Calendar

A time-based view of what is planned, scheduled, and already live.

### Dashboard

A performance view that shows each identity against its own goals and baselines.

### Settings

Configuration for boards, tokens, imports, and system health.

## Design Direction

Tomboj Studio is intended to feel like a real product, not an internal spreadsheet.

Design principles:

* Light-first interface
* Clean dashboard layout
* Clear hierarchy
* Minimal visual clutter
* Fast card movement
* Visible status
* No silent failures
* Auto-save everywhere
* Mobile triage, not full mobile administration

## Technical Direction

The private application is planned around:

* React
* Vite
* Tailwind
* shadcn/ui
* dnd-kit
* Node.js
* Express
* Drizzle ORM
* Postgres
* REST API
* MCP server
* Google Sign-In
* Bearer-token agent access

This public repository does not include the private implementation.

## What This Repository Is

This repository is:

* A public product overview
* A portfolio artifact
* A summary of the operating model
* A way to explain the product concept without exposing the private codebase

## What This Repository Is Not

This repository is not:

* The live application
* The private source code
* A public SaaS template
* An open-source project
* A customer data repository
* A deployment repository

## Related Work

Tomboj Studio is part of a broader body of work around AI-enabled operating systems, customer success workflows, content operations, and human-in-the-loop automation.

Related public work:

* Innovate Project Development Mode
* Hey Haas Product Overview

## License and Use

This repository is a public product overview and portfolio artifact. It does not include the private Tomboj Studio application codebase.

No license is currently granted for reuse, redistribution, or derivative works.
