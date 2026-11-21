# AutoPiac — UX/UI Design Semester Project

**University:** University of Pécs — PTE MIK  
**Course:** UX/UI Design  
**Student:** Umut Can Birbir — Neptun: DUJ3ZD  
**Project focus:** User-centered private vehicle listing creation for the Hungarian market.

## Overview

This repository documents the semester-long UX/UI design process for **AutoPiac**, an automotive marketplace concept. The academic scope is intentionally focused on one user journey: creating and submitting a private car advertisement.

The deliverable is an evidence-based, clickable Figma prototype, **not a complete production application**.

## Project Links

- **[FigJam — UX/UI Project Discovery](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB)**
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

## Real Interview R01 — Findings Implemented as Static Mockups

An owner-reported interview with an 18-year-old first-time prospective seller identified two missing content areas: equipment choices and damage/replaced-parts information. [Research record](project/docs/interview-r01.md) · [Homework 02](homework/02/README.md). A new [Figma Equipment & Condition mockup](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) has been linked into the listing flow. Controls remain static and no follow-up test has occurred.

## Competition and Next User Tests

- [Homework 03 competitor analysis](homework/03/README.md) compares official Használtautó and mobile.de source evidence without claiming untested competitor defects.
- [Homework 04 FigJam prioritization matrix](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2003-182) and [competitor comparison cards](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2003-214).
- [R01 follow-up feedback](project/docs/r01-follow-up-2026-11-21.md) led to a [16-option grouped equipment screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2).
- [Send this anonymous user testing instruction sheet to three participants](project/docs/usability-test-instructions.md). Results are **not yet recorded** for this newer design.

## Full Figma Design QA — 2026-11-21

The latest AutoPiac mobile screens, desktop layout and all four component groups were visually and structurally reviewed. Photo thumbnails, navigation gaps, input-error clipping, desktop spacing, button variant dimensions, user-facing copy and body-panel status controls were corrected. [Read the full review and remaining limitations](project/docs/design-qa-2026-11-21.md). Real form entry and publishing remain outside the static Figma prototype.

## Homework 09 — Implemented Figma Revisions and Mini Design System

- [Revised AutoPiac prototype — Student Figma account](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2): an independent row of nine yellow/white screens with field guidance, photograph count and angles, clickable review-section corrections, and honest prototype completion wording.
- [Figma Mini Design System](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-2): four real component sets with 15 variants.
- [Developer Handoff](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55): responsive, validation, color and photo limits.
- [Homework 09 documentation](homework/09/README.md) records before/after links, implementation and the remaining unverified participant re-test.

**Research integrity:** These improvements were designed based on known prototype limitations, not on unreported user complaints. Their effectiveness has not yet been re-tested.

## Initial Test Evidence

- **[Homework 08 — Three-person Navigation Walkthrough Report](homework/08/README.md)**: 3/3 reportedly navigated the static Figma flow successfully; simplicity received positive aggregate feedback. This was **not** an end-to-end test using editable forms.
- **[Homework 09 — Three Proposed UX Improvements](homework/09/README.md)**: validation clarity, photo guidance, and review/confirmation. Proposals await Figma implementation and re-testing.

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

## Yellow & White UI Direction

- [Open the recolored AutoPiac screen set in Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)
- [Yellow & White Color Guideline](project/docs/color-guideline.md)
- Nine colorized frame copies sit below the preserved grayscale wireframes. Primary buttons, information panels, photo placeholders and progress elements use yellow accents. Basic navigation links point among the colored frames.
- Visual QA and user testing are still pending; Figma controls are not real editable data-entry inputs.

## Figma Wireframes and Prototype

- [Editable Figma wireframes and click-through prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)
- Eight mobile screen states and one desktop variation have been drafted.
- Basic screen-to-screen click navigation has been added. Form inputs are **visual placeholders**, not functional data-entry widgets.
- Real participant tests, validation-dependent interactions and final high-fidelity UI are still pending.

## Actionable Task Tracking

Seven course project tasks are tracked in [GitHub Issues](https://github.com/umutcanbirbir/autopiac-ux-ui-design/issues). These issues are not a substitute for the lecturer's requested Kanban board.

## GitHub Project Board

**Status:** Not created yet. Add the URL for the project board with **Todo → In progress → Done** after setup.

## Research Integrity

The initial problem statement and user-behavior assumptions are hypotheses. Any personas, simulated examples, or proposed tests will be labeled; research findings will only be reported after real participant input.
