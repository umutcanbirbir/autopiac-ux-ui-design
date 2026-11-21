# Homework 09 — Iteration Plan, Mini Design System & Developer Handoff

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Iterations **planned, not implemented or verified**. Existing yellow/white visual treatment was designed **before** this participant walkthrough.  
**Figma screens:** https://www.figma.com/design/cEkbZFkMY32FYY4q5op5Jm?node-id=9-2  
**Color guideline:** [Yellow & White](../../project/docs/color-guideline.md)  
**Test evidence:** [Homework 08](../08/README.md)

## Summary of Available Evidence

The project owner reported that 3/3 participants reached the end of the non-editable Figma screen flow. Participants did not need to fill in forms; no particular problem or change request was reported. The owner summarized the response as positive about the interface's simplicity.

**Interpretation:** Keep the straightforward structure. Do not claim the walkthrough revealed three specific user pain points. The changes below are **designer-proposed responses to known prototype limitations and future testing requirements**.

## Three Planned Design Iterations

| ID / priority | Baseline | Proposed revision | Why | What counts as completed? |
| --- | --- | --- | --- | --- |
| **I-01 / P0 — Validation clarity** | Fields are static; an error screen is a separate example | Clearly distinguish required vs optional fields; add field-level help; annotate a missing-field state and a corresponding correction path | Makes a future realistic task testable and reduces ambiguity about error recovery | Before/after frames + at least one observed user attempting to fix a missing field |
| **I-02 / P1 — Photograph guidance** | Photo upload is presented as a visual placeholder | Provide visible 0/5 through 5/5 progress, photo angle examples, cover-photo label and explicit missing-photo instruction; show keyboard-accessible sort options in specification | Product requires at least 5 photos; the current Figma demo did not test photo selection | Before/after photo frames + participant observation on the 5-photo rule |
| **I-03 / P1 — Review and completion** | Review and success are navigation-only frames | Add a concise editable review summary, obvious return-to-section actions, clear submission feedback and an explicit notice that this is a prototype | The walkthrough demonstrated navigation, not understanding or correction of actual entered data | Before/after review screen + task observation confirming users can identify and correct a seeded error |

These are **proposals**: their effectiveness is not established by the three navigation walkthroughs.

## Follow-Up Study to Validate Changes

### Realistic task
"Using sample fictional vehicle information, create an AutoPiac listing, choose at least five photos, add a price and description, fix an intentionally missing field, review your listing and finish the prototype."

### Required records
- Anonymous participant ID and date.
- Relevant selling experience, if participant volunteers it.
- Start/end time and total duration.
- Completed without help? (yes/no).
- Number and type of validation errors encountered.
- Exact step where a participant hesitated.
- Participant's own feedback in their own words, only if actually recorded.
- Before/after design version tested.

### Success criteria
- At least **2 of 3** complete the full test task independently (proposed threshold).
- No observed critical unrecoverable navigation or validation failures.
- Re-test at least one actual design change and document the outcome.

The [browser-based interactive demonstration](../../docs/index.html) has data-entry behavior and can support task simulation, while the Figma file remains the primary design artifact for the coursework.

## Mini Design System — Planned Component Inventory

- **Button:** primary, secondary, disabled, loading, hover and keyboard focus.
- **Text Input:** empty, filled, focused, invalid and disabled.
- **Select:** default, expanded, selected, error.
- **Progress Indicator:** completed, current and upcoming steps.
- **Photo Tile:** empty, uploading, uploaded, failed, cover.
- **Information Alert:** hint, validation error and success.

### Foundational Tokens (Design Proposal)
- Primary yellow: \`#FFD400\`
- Light yellow: \`#FFF7D8\`
- White: \`#FFFFFF\`
- Primary text: \`#1F1F1F\`
- Error red: \`#B42331\`
- Spacing: 8/16/24/32 px rhythm
- Type: accessible hierarchy and clearly distinguished labels
- Contrast: manually verify WCAG 2.2 Level AA

**Status:** This is the component specification. It is not a completed Figma component library.

## Annotated Handoff Screen — Scope

Annotate the Figma **Vehicle Details** frame with:
1. Mobile and desktop responsive frame widths.
2. Label positioning, spacing, and min input target height.
3. Required and optional fields.
4. Exact validation/error text and placement.
5. Button states and keyboard focus behavior.
6. Progress indicator semantics and accessibility notes.

## Iteration Evidence Log

| Iteration | Figma before link | Figma after link | Supporting test evidence | Re-tested? |
| --- | --- | --- | --- | --- |
| I-01 | Pending | Pending | Not yet gathered | No |
| I-02 | Pending | Pending | Not yet gathered | No |
| I-03 | Pending | Pending | Not yet gathered | No |

## Completion Checklist

- [x] Drafted three prioritized design revision hypotheses, grounded in known prototype/test limitations.
- [x] Defined the mini design system's required components and design tokens.
- [ ] Implement the three revisions in Figma.
- [ ] Capture before/after evidence.
- [ ] Verify at least one revision with an actual participant.
- [ ] Build reusable Figma components and states.
- [ ] Produce annotated developer handoff screen.
