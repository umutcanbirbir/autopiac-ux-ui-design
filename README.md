# AutoPiac — UX/UI Design Semester Project

**University:** University of Pécs — PTE MIK  
**Course:** UX/UI Design  
**Student:** Umut Can Birbir — Neptun: DUJ3ZD  
**Project focus:** User-centered private vehicle listing creation for the Hungarian market.

## Overview

This repository documents the semester-long UX/UI design process for **AutoPiac**, an automotive marketplace concept. The academic scope is intentionally focused on one user journey: creating and submitting a private car advertisement.

The deliverable is an evidence-based, clickable Figma prototype, **not a complete production application**.

## Project Links

- **[FigJam — UX/UI Project Discovery](https://www.figma.com/board/8M1vecaiwW7U9MpYBbuok2)**
- **[Homework 01 — Project Discovery](homework/01/README.md)**
- **[Project Scope and Milestones](project/README.md)**
- **[User Research Plan](project/docs/research-plan.md)**
- **[Design Decision Log](project/docs/decision-log.md)**
- **[Presentation Planning](presentation/01-01/README.md)**

## Repository Structure

```text
autopiac-ux-ui-design/
├── README.md
├── homework/
│   └── 01/
│       └── README.md
├── project/
│   ├── README.md
│   └── docs/
│       ├── research-plan.md
│       └── decision-log.md
└── presentation/
    └── 01-01/
        └── README.md
```

## Work Plan

1. Problem framing and target users.
2. Actual user interviews / observation and research synthesis.
3. Competitor analysis and usability audit.
4. Information architecture and wireframes.
5. Clickable Figma prototype.
6. Usability tests, revisions, UI guidelines, and final presentation.

## Interactive Browser Demo (Data Entry and Photo Upload)

The [standalone interactive prototype](docs/index.html) is a pure HTML/CSS/JavaScript simulation that can be used directly in a browser. Unlike the Figma wireframes, it supports:

- Vehicle brand/model selection, year, mileage, fuel, and transmission inputs.
- Uploading 5–30 local photographs (max 8 MB each), previewing, reordering, and removing them.
- Price, title, condition, and description fields.
- Required-field validation, review, editing and successful task completion.

**Privacy:** Images and form values remain inside the user's browser; no backend, database, authentication or real listing publication exists. The success screen confirms completion of the **prototype task only**.

**How to publish on GitHub Pages:** Repository → Settings → Pages → Build and deployment → Deploy from a branch → main → /docs → Save. The expected site address is `https://umutcanbirbir.github.io/autopiac-ux-ui-design/`, **after GitHub Pages finishes publication**.

## Figma Wireframes and Prototype

- [Editable Figma wireframes and click-through prototype](https://www.figma.com/design/cEkbZFkMY32FYY4q5op5Jm)
- Eight mobile screen states and one desktop variation have been drafted.
- Basic screen-to-screen click navigation has been added. Form inputs are **visual placeholders**, not functional data-entry widgets.
- Real participant tests, validation-dependent interactions and final high-fidelity UI are still pending.

## Actionable Task Tracking

Seven course project tasks are tracked in [GitHub Issues](https://github.com/umutcanbirbir/autopiac-ux-ui-design/issues). These issues are not a substitute for the lecturer's requested Kanban board.

## GitHub Project Board

**Status:** Not created yet. Add the URL for the project board with **Todo → In progress → Done** after setup.

## Research Integrity

The initial problem statement and user-behavior assumptions are hypotheses. Any personas, simulated examples, or proposed tests will be labeled; research findings will only be reported after real participant input.
