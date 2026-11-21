# Homework 08 — Usability Testing & Mini UI Guideline

**Project:** AutoPiac — A User-Friendly Car Listing Experience  
**Student:** Umut Can Birbir (DUJ3ZD)  
**Report prepared:** 2026-11-21  
**Evidence:** The project owner's report of a test with three participants, received on 2026-11-21. Individual session dates, recordings, and timestamps were not provided.  
**Prototype:** [Figma — yellow/white AutoPiac flow](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)

## 1. Objective

Evaluate whether users can understand and navigate the initial AutoPiac listing prototype. The broader project goal is to assess whether private car sellers can create a complete, accurate advertisement; **this test did not cover that full task**.

## 2. Method and Actual Task Scope

**Study type:** Initial navigation walkthrough, reported by the project owner.

Three participants were shown the prototype. The task was to move through the listing screens and reach the publication/completion screen. The Figma input fields were **static visual elements**, so participants could not enter vehicle information, upload actual photographs, or submit real form values in Figma. The walkthrough therefore measured screen-flow completion, not end-to-end listing completion.

The project owner did not report participant demographics, prior car-selling experience, recruitment method, test durations, recordings, or whether any prompting or assistance was given. These details must not be inferred.

## 3. Participant Results (reported, not independently observed by the author)

| Participant | Reached final screen? | Reported difficulty | Specific suggestion | Task time |
| --- | --- | --- | --- | --- |
| P01 | Yes | None reported; fields were not fillable | None reported | Not recorded |
| P02 | Yes | None reported; fields were not fillable | None reported | Not recorded |
| P03 | Yes | None reported; fields were not fillable | None reported | Not recorded |

**Aggregate owner-reported feedback:** The interface was considered simple and was liked. This is a summary from the project owner, **not** a verbatim quotation attributable to a specific participant.

## 4. Results and Interpretation

- **Navigation completion:** 3/3 participants (100%) reportedly reached the end of the screen flow.
- **Reported navigation difficulties:** None; participants were not required or able to fill in the form.
- **Reported specific change requests:** None.
- **Reported general impression:** Positive reaction to the interface's simplicity.
- **Time-on-task:** Not measured or supplied.
- **Independent completion:** Not separately recorded (no claim of unaided completion).
- **Real data entry, photo upload, validation and error recovery:** Not evaluated.
- **Accessibility:** Not formally evaluated.

**Important distinction:** The initially proposed success target was at least **2 of 3 participants completing the full listing task independently**. This walkthrough does **not** establish that target because the prototype had no functional data entry and independence was not recorded. It supports the narrower observation that **3 of 3 reportedly traversed the prototype screens**.

The small number of participants and limited task scope prevent generalizing results to the overall Hungarian private-car-seller population.

## 5. Findings and Design Implications

| ID | Finding / limitation | Evidence type | Severity | Design implication |
| --- | --- | --- | --- | --- |
| F-01 | All three reported participants reached the final screen. | Owner-reported navigation outcomes | Positive observation; not a defect | Preserve the simple linear structure while refining details |
| F-02 | The interface's simplicity was liked. | Owner-reported aggregate feedback | Positive observation; not individually attributed | Avoid introducing unnecessary steps and complexity |
| L-01 | Form entry could not be tested because Figma controls were static. | Known prototype limitation, also stated in owner report | High *validation gap*, not an observed user error | Provide a working task simulation or a more expressive Figma interaction model |
| L-02 | Field errors, minimum photo count and recovery were not genuinely tested. | Untested tasks | High *validation gap* | Add explicit scenarios and test how people recover |
| L-03 | Time, assistance level, accessibility and participant profiles were not captured. | Missing research metadata | Medium *study quality gap* | Collect the measures in a follow-up study |

**No participant-reported usability defect was identified in this walkthrough.** The issues above are limitations in prototype fidelity or test coverage, **not claims that participants experienced these problems**.

## 6. Prioritized Next Steps

**P0 — Test a realistic listing task:** Use the existing [interactive browser demonstration](../../docs/index.html), which has real input fields, photo selection and validation. It is a local prototype, not a deployed marketplace. Ask three participants to complete the task using fictional vehicle data; record completion, timing, assistance and errors.

**P1 — Clarify Figma's static nature and states:** Keep the Figma design as the primary academic artifact. Ensure it depicts vehicle fields, photo requirements, review, missing-field validation, missing-photo validation and submission confirmation. Label demonstration-only error-state links clearly.

**P2 — Refine guidance without sacrificing simplicity:** Maintain the yellow/white interface and readable labels. Consider concise field help, a visible step indicator and photo-count guidance. These are **proposed improvements**, not changes requested by participants.

**P3 — Accessibility review:** Verify contrast, visible focus, keyboard interaction expectations, labels, error text and appropriate touch targets against WCAG 2.2 AA.

See [Homework 09 — Proposed Iteration Plan](../09/README.md) for detailed before/after acceptance criteria and verification.

## 7. Mini UI Guideline — Draft

The following is a **design guideline**, not a claim that the interface has passed all accessibility tests.

| Element | Design guidance |
| --- | --- |
| Primary color | Yellow \`#FFD400\`; dark text \`#1F1F1F\` on yellow |
| Secondary surfaces | White \`#FFFFFF\`, pale yellow \`#FFF7D8\` |
| Body text | Dark, legible sans-serif; body text typically ~16 px |
| Inputs | Visible label, neutral border, clear required indication |
| Primary actions | Yellow fill, high-contrast dark text, visible pressed/focus states |
| Validation | Specific textual instructions and an error indicator beyond color alone |
| Progress | Clearly distinguish completed, current and upcoming steps |
| Photographs | Explain minimum of five, show count, and permit accessible reordering |
| Spacing | Consistent 8/16/24/32 px system |
| Contrast target | WCAG 2.2 AA: 4.5:1 normal text, 3:1 large text where relevant |
| Keyboard target | Clear tab order, focus outline and non-drag alternatives for sorting |

Reference: https://www.w3.org/TR/WCAG22/

## 8. Evidence Checklist

- [x] Three participant navigation results reported by the project owner.
- [x] Aggregated positive impression and absence of reported suggestions documented without invented quotations.
- [x] Results and their limitations explicitly distinguished.
- [x] Improvement priorities documented.
- [x] Draft mini UI guideline included.
- [ ] Actual task-performance measures using editable data fields.
- [ ] Participant context, timing, and assistance level recorded.
- [ ] Verified accessibility results.
- [ ] Changes implemented and re-tested.

## 9. Research Integrity Note

No individual quotes, precise test durations, demographics, screen recordings or error observations were supplied. None have been invented. The walkthrough is presented as **owner-reported navigation testing**, not as a complete or independently verified usability study.
