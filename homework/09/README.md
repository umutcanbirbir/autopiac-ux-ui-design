# Homework 09 — Iteration, Mini Design System & Developer Handoff

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Three designed improvements implemented in Figma; reusable variants and handoff created. **No post-change participant retest yet.**  
**Date:** 2026-11-21  
**Primary Figma file:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC  
**Before (Yellow/White):** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-20  
**After (Homework 09):** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-25  
**Color guide:** [Yellow & White Color Guideline](../../project/docs/color-guideline.md)  
**Test basis:** [Homework 08](../08/README.md)

## Evidence and Interpretation

The owner reported a three-participant navigation walkthrough of the static Figma prototype: all reportedly reached the final screen, and the interface was liked for its simplicity. No participant reported a concrete navigation problem or feature request. Actual text input, photo upload, error correction and unaided completion were not tested in Figma.

**Therefore the iterations below are designer-initiated responses to demonstrable prototype limitations and to the need for clearer guidance. They must NOT be described as participant-requested changes or as proven usability improvements.**

## Three Documented Design Iterations

| ID | Before | After (implemented in Figma) | Design rationale | Validation |
| --- | --- | --- | --- | --- |
| **I-01 — Validation / required data** | Vehicle screen with visual form fields and basic help; separate missing-field error example | Enhanced vehicle form copy explicitly explains required fields; new yellow guidance card explains make/model/year/mileage; missing-field example emphasizes explicit corrective text and remains linked from vehicle screen | Make data expectations and recovery path more apparent | **Not yet retested** |
| **I-02 — Photo minimum / guidance** | Photo screen showed minimum count and a simple prototype branch | Updated photo count/status, 5 required / 30 standard / 55 premium copy, cover-photo explanation, new guidance card listing five recommended viewing angles, and missing-photo error copy emphasizing 2/5 + add three | Reduce ambiguity about image quantity and useful coverage | **Not yet retested** |
| **I-03 — Review / completion clarity** | Read-only overview with generic back-to-edit button and “listing submitted” state | Review section cards are clickable and navigate to their corresponding step; new edit instruction card; success screen explicitly states prototype completed and nothing was published; return-to-review and restart buttons are connected | Improve step correction and avoid implying a real listing was published | **Not yet retested** |

### Before / After Figma Screen Links

| Part | Before | After |
| --- | --- | --- |
| Vehicle details | [Before](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-20) | [After](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-25) |
| Photos | [Before](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-50) | [After](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-62) |
| Review | [Before](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-93) | [After](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-115) |
| Success | [Before](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-116) | [After](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-143) |

**Preservation:** The grayscale low-fidelity originals, first yellow/white colored version, and Homework 09 revised version are in separate Figma frame rows. All revised primary navigation buttons were re-linked to revised frames (rather than sending users to the older designs). The review summary sections and the success-state actions also have prototype links.

## Mini Design System — Real Figma Components

Four **real Figma COMPONENT_SET** groups with **15 variants** have been created:

| Component set | Variants | Figma |
| --- | --- | --- |
| **AutoPiac / Button** | Primary, Secondary, Disabled, Focused | [Button](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-2) |
| **AutoPiac / Input** | Default, Filled, Focused, Error | [Input](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-11) |
| **AutoPiac / Alert** | Info, Error, Success | [Alert](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-20) |
| **AutoPiac / Photo Tile** | Empty, Filled, Cover, Error | [Photo Tile](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-30) |

Foundations are documented in the design file: primary yellow \`#FFD400\`, white \`#FFFFFF\`, pale-yellow \`#FFF7D8\`, dark-text \`#1F1F1F\`; Inter font; 8/16/24/32 px spacing. Keyboard/focus and contrast checks remain requirements, **not verified compliance results**.

Note: These are reusable component variant definitions in Figma, but the existing screens are not necessarily refactored into instances of all components.

## Annotated Developer Handoff

[Vehicle Details — Developer Handoff Panel](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55) includes:

1. Responsive mobile 390 px / desktop 1130 px references and single-column mobile rules.
2. Explicit make, model, production year, mileage field requirements.
3. Field-level validation summary, explanation, and focus behavior.
4. Photo constraints: minimum five; standard max 30, premium max 55; 8 MB maximum per photo.
5. Button colors, interactive states and WCAG 2.2 AA target.
6. Clear distinction between Figma simulation and functional browser demonstration.

## New Evidence-Driven Design Backlog (R01 Interview)

A separate exploratory interview with an 18-year-old first-time prospective seller identified two missing sections in the current AutoPiac listing flow. This feedback was collected **after** the earlier I-01 to I-03 refinements and should not be retroactively attributed to those revisions.

| ID | Directly reported participant concern | Proposed next Figma revision | Status |
| --- | --- | --- | --- |
| **I-04 — Vehicle Equipment** | "Users cannot choose the car's equipment/features" (paraphrase) | Add an optional, searchable or grouped multi-select for common equipment and show selected items in Review | **Planned, not built or tested** |
| **I-05 — Damage & Replaced Parts** | "There is no section for damage/replaced parts" (paraphrase) | Add structured vehicle-condition/damage disclosure, allowing users to identify repaired/repainted/replaced body panels and add notes; include summary in Review | **Planned, not built or tested** |

Preserve the simple step-by-step flow that this participant liked. Verify the terminology and controls with additional participants rather than assuming that extra fields automatically improve usability.

[Source interview R01](../../project/docs/interview-r01.md) · [Homework 02 synthesis](../02/README.md)

## Follow-Up Validation — Remaining

To evaluate whether these changes helped users in practice, ask participants to complete a **realistic interactive listing task** using the HTML demonstration or a prototype capable of actual input. Capture time, independent completion, field errors, where correction was needed, and real participant remarks. Retest at least one improved Figma state or compare versions. **No such follow-up results are claimed here.**

## Completion Checklist

- [x] Three **implemented and documented** before/after design refinements.
- [x] Revised yellow/white Figma screens with basic clickable navigation.
- [x] Four reusable Figma component sets and 15 variants.
- [x] Developer handoff panel with field, spacing, error and breakpoint notes.
- [x] Cross-links to evidence, palette and source frames.
- [ ] Independent human visual and accessibility QA of final screens.
- [ ] At least one real user/peer follow-up evaluation of a design improvement.
- [ ] Actual end-to-end editable-field completion test (not possible using static Figma forms alone).
