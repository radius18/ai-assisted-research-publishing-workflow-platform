# AI-Assisted Research & Publishing Workflow Platform

A local research-to-publishing platform for turning an initial content idea into evidence-grounded research, structured outputs, managed media, article composition, QA, and publication-ready content.

**Current working use case:** Daring Places travel publishing  
**Status:** Work in progress · September 2026–Present

## Project Overview

This project was designed around a principle I wanted to keep explicit:

**research, evidence, media, and writing should remain connected rather than becoming one opaque “generate article” step.**

The application separates the major stages of the publishing workflow:

**Intake → Research → Outputs → Media → Article → QA / CTA → Preview**

Research findings retain source and verification context before they move downstream. Outputs can branch from shared project research. Media is processed non-destructively with lineage between the original asset, working versions, generated outputs, and placements. Article structure is built from reusable components rather than one fixed template.

The current implementation is being developed around travel publishing, but the underlying workflow is intended to be reusable for other research-heavy publishing and content-production use cases.

## Evidence-Grounded Research

![Evidence-grounded research workspace](Screenshot%202026-10-19%20012908.png)

*Research workspace showing durable research passes, source records, claim-verification state, editorial workflow, and explicit separation between verified and still-unverified evidence before content moves downstream.*

The research layer is designed to distinguish:

- research findings
- source records
- verified claims
- items that still need verification
- editorial decisions
- hooks and media briefs
- the latest research pass versus the overall research corpus

AI-emitted URLs are treated as candidates until the research workflow successfully retrieves and validates the supporting source evidence.

## Multi-Output & Editorial Branching

![Multi-output planning](Screenshot%202026-10-19%20013051.png)

*Output-planning workspace for creating follow-ups, alternative editorial angles, custom articles, or separate projects while choosing whether to reuse existing project research or begin a distinct research path.*

A project can produce more than one deliverable without forcing every article to repeat the same research process.

The workflow supports concepts such as:

- follow-up articles
- alternative editorial angles / forks
- custom articles inside an existing project
- separate new projects
- shared project research
- explicit article/project relationships
- manual output creation without silently forcing a new research run

## Non-Destructive Media Processing

![Media Processing Lab](Screenshot%202026-10-19%20013249.png)

*Processing Lab for reviewing assets, creating enhancement/crop versions and output sets, managing placement status, and preserving the archived original rather than overwriting source media.*

The media workflow is designed around lineage rather than disposable image edits.

Key concepts include:

- archived immutable original
- current processing source
- non-destructive Processing Versions
- enhancement presets and manual adjustments
- crop/focal-point versions
- Output Sets and Output Files
- provenance/history
- asset status separated from article placement

This keeps image processing, ownership, derivatives, and later article use traceable.

## Modular Article Composition & Voice Controls

![Modular article composition](Screenshot%202026-10-19%20013411.png)

*Configurable article profile with reusable content primitives, layout/emphasis controls, profile revisions, and a separate voice pass applied after factual drafting.*

The article system uses reusable composition primitives rather than one hard-coded page structure. Current examples include:

- Hero
- Quick Facts
- Place / Destination Chapter
- Gallery / Visual Story
- Swipe Story
- Food / Cuisine
- Map / Location
- Planning / Logistics
- Callout / Don't Miss
- Comparison
- Contextual CTA
- Sources / Freshness

Each primitive can be enabled, pinned, disabled, reordered, or given different emphasis depending on the article profile.

A separate voice/humanization pass is designed to improve readability and editorial voice **after** factual drafting while preserving facts, structure, source links, names, numbers, and researched distinctions.

## Durable Workflow & QA

The platform also includes infrastructure for longer-running work rather than treating AI operations as disposable browser requests.

Current design areas include:

- durable background jobs
- progress/heartbeat tracking
- restart recovery
- duplicate-run protection
- activity and error history
- explicit research verification state
- reusable project/output relationships
- media provenance and lineage
- non-destructive editing
- QA / CTA stages
- explicit user actions rather than hidden automatic generation

## Why This Project Matters

The goal is not simply to generate articles faster.

The broader goal is to explore how an AI-assisted publishing system can remain:

- **evidence-aware** — claims retain source and verification context
- **modular** — research, outputs, media, article structure, and QA remain separable
- **traceable** — media and research artifacts preserve lineage
- **human-controlled** — major workflow actions remain explicit
- **reusable** — one project can support multiple outputs and editorial directions
- **recoverable** — long-running work is persisted rather than disappearing on refresh/restart

## Skills Demonstrated

- Applied AI workflow design
- Python-based web application development
- Requirements analysis
- Quality Assurance / UAT
- Research and source verification workflows
- Data / provenance modeling
- Media asset management
- Non-destructive processing workflows
- Product / UX design
- Durable job and state management
- Debugging and regression testing
- Technical documentation

## Portfolio Scope

This repository is a public portfolio presentation rather than the complete private Publishing Engine codebase or production workspace.

The screenshots demonstrate working research, output-planning, media-processing, and article-composition surfaces. Internal project data, local paths, private configuration, test fixtures, logs, and implementation source remain outside this public repository.

A polished public Preview screenshot can be added later as that presentation layer continues to mature.
