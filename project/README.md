# AutoPiac — UX/UI Design Semester Project

**Course:** UX/UI Design, University of Pécs (PTE MIK)  
**Student:** Umut Can Birbir — Neptun: DUJ3ZD  
**Progress:** Wireframes and initial three-person navigation walkthrough documented; realistic task tests and final design work pending.  
**FigJam board:** https://www.figma.com/board/FReaY560jfsj9gfCeta8oB

## Project Description
AutoPiac is a Hungarian automotive marketplace concept. This semester project focuses on the **private seller's vehicle-advertisement creation flow**, not the entire commercial product. Its goal is to design and test an accessible, guided listing experience.

## Problem and Audience
**Hypothesis:** Complicated listing forms and unclear vehicle requirements can confuse some private sellers. This needs validation through real research.

**Target users:** Private individuals selling a car in Hungary, including first-time sellers.

## Proposed Primary User Flow
1. Start a new listing.
2. Enter vehicle specifications.
3. Upload vehicle photos.
4. Set price and description.
5. Review the listing and fix highlighted errors.
6. Submit the listing and see a success state.

## Expected Deliverables
- Problem framing, user goals, assumptions, and success metrics.
- Real user research, anonymous notes, persona, and journey map.
- Competitor and accessibility audit.
- Information architecture, sitemap, and task flow.
- Low-fidelity Figma wireframes for mobile and larger screens.
- Clickable prototype with success and exceptional states.
- Usability test results and documented changes.
- Mini design system and developer handoff.
- Final 5–10 minute presentation.

## Milestone Plan
| Stage | Activity | Status |
| --- | --- | --- |
| 01 | Problem framing and FigJam | Initial draft |
| 02 | User research | Initial R01 interview, two evidence-based content gaps, persona and journey documented; more validation needed |
| 03 | Competitor and accessibility audit | Official-source desk comparison complete; live interface/accessibility inspection pending |
| 04 | Prioritization and project brief | Four-quadrant matrix added to FigJam and revised from R01 feedback |
| 05 | Sitemap and task flow | Not started |
| 06 | Low-fidelity wireframes | Initial Figma screens created |
| 07 | Interactive prototype | Basic screen navigation created; forms remain static |
| 08 | Usability testing and UI guideline | Three-person navigation walkthrough reported; full task not yet tested |
| 09 | Design revisions, components, handoff | Three revisions implemented, 15 Figma variants and handoff created; user re-test pending |
| 10 | Final presentation and reflection | Not started |

## Competitor Audit, FigJam and Next Usability Test

- [Homework 03 — official-source Használtautó and mobile.de comparison](../homework/03/README.md) with six UX risk cases and two conditional accessibility checks.
- [Homework 04 — impact/feasibility matrix and updated ideation](../homework/04/README.md) in FigJam.
- [R01 informal follow-up](docs/r01-follow-up-2026-11-21.md): revised mockup liked but equipment list still requested improvement.
- [16-option categorized equipment design in Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2), **not yet independently tested**.
- [Three-participant test instructions and blank results form](docs/usability-test-instructions.md).

## Complete Figma QA Review

All current mobile screens and the desktop reference plus mini-design-system variants were inspected. Corrections included photo thumbnail concepts, coherent back-navigation, shorter validation copy, a better-balanced desktop layout and damage-status selection chips. The main revised mobile flow has connected buttons and no identified top-level content overflow. See [Figma QA Report](docs/design-qa-2026-11-21.md) for verified checks and remaining limitations.

## Homework 09 — Design Iterations Implemented

After preserving the grayscale and first yellow/white prototypes, a separate Figma row now contains revised screen designs. Three refinements were implemented: **I-01 clearer required fields/error guidance**, **I-02 minimum photo count and recommended views**, and **I-03 review/edit and truthful prototype completion**.

- [Revised listing flow](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2)
- [Figma reusable component sets](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-2) — 15 variants across button, input, alert and photo tile
- [Developer handoff notes](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55)
- [Homework 09 before/after evidence](../homework/09/README.md)

**Outstanding:** User follow-up evaluation of changed screens, end-to-end realistic task testing and final human visual/accessibility QA. The three refinements have been built, **not proven to improve performance**.

## Research Interview — First-Time Prospective Seller

A separate owner-reported exploratory interview with an 18-year-old first-time prospective seller (the researcher's sibling) identified two clear content gaps: **equipment/features selection** and **damage/replaced-parts disclosure**. The participant understood the current interface and navigated its static prototype independently; no actual form data was entered. The report explicitly discloses convenient-family recruitment and missing session metadata.

- [R01 Interview Evidence](docs/interview-r01.md)
- [Homework 02 — Interview, Insights, Persona Snapshot and Journey](../homework/02/README.md)
- [Homework 09 — Two New Planned Improvements](../homework/09/README.md)

These content areas have been added in a [static Figma equipment and condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) and connected to Review. They have **not** been re-tested, and the controls do not accept real data. The original three-person navigation walkthrough is documented separately in Homework 08; avoid counting R01 as an additional distinct participant without confirmation.

## R01-Driven New Figma Screen

- [Equipment & Condition — new static mobile screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2)
- [Review screen — edit link to Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-115)
- [FigJam actual interview affinity themes](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB)

**Still pending:** user re-test of these content changes and actual interactive form behavior.

## Initial Usability Walkthrough Results (Owner-Reported, 2026-11-21)

The project owner reported a three-participant walkthrough of the static Figma listing flow. All three reportedly reached the final screen and the interface's simplicity received positive general feedback. No specific participant problems or improvement suggestions were provided.

**Scope limitation:** Because the Figma form fields are not editable, this was a **navigation walkthrough**, not a complete listing-creation test. The original 2-of-3 unaided end-to-end completion target has **not** been verified. No participant task times, demographics, or independence/assistance details were recorded.

- [Homework 08 — Detailed Test Report](../homework/08/README.md)
- [Homework 09 — Planned Design Iterations](../homework/09/README.md)

## UI Color Exploration

A yellow/white visual version of the original wireframes has been created in Figma while retaining the grayscale originals. See [the colored screens](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC) and [the documented palette](docs/color-guideline.md). Screen interactions remain illustrative; no real Figma text input is implemented.

## Design Artifacts — Created 2026-11-21

**[Figma — Low-Fidelity Wireframes and Basic Click-Through](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)**

Created: eight mobile frames (start, vehicle details, photos, price/description, review, success, photos error, required vehicle field error), plus a desktop vehicle details layout. Basic click navigation connects the main path and error branch. Input controls are currently visual and must not be described as working data entry. Initial navigation-test results are now reported, but real end-to-end task testing and final polish remain pending.

**[FigJam — Planned Seller User Flow](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB)**

## Project Management
**Repository-hosted Kanban:** [Todo / In Progress / Done](KANBAN.md), with links to all existing [GitHub Issues](https://github.com/umutcanbirbir/autopiac-ux-ui-design/issues). A native **GitHub Projects** board is still pending because the connected GitHub tool lacks Projects creation; see [Issue #7](https://github.com/umutcanbirbir/autopiac-ux-ui-design/issues/7).

## Navigation
- [Homework 01](../homework/01/README.md)
- [Research Plan](docs/research-plan.md)
- [Design Decision Log](docs/decision-log.md)
- [Presentation Plan](../presentation/01-01/README.md)

**Evidence policy:** Hypothetical personas, simulated observations, and design assumptions will be explicitly labeled and never passed off as real participant data.
