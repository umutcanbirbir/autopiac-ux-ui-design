# Homework 08 — Usability Test and UI Guidelines

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Report date:** 21 November 2026  
**Prototype:** [AutoPiac Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)

## Test Goal

I wanted to check whether people could follow the main car-listing screens and understand the basic steps without getting lost.

## Method

Three people tried the initial clickable Figma prototype. Their task was to navigate from the beginning of the listing flow to its final screen.

The form fields, checkboxes and photo upload areas were only visual elements. This was therefore a **navigation test**, not a test of entering vehicle details or publishing an actual advertisement. I did not record individual completion times or whether assistance was needed for each participant.

## Results

| Participant | Reached the final screen? | Difficulties mentioned | Suggestions |
| --- | --- | --- | --- |
| P01 | Yes | None mentioned; fields were not editable | None recorded |
| P02 | Yes | None mentioned; fields were not editable | None recorded |
| P03 | Yes | None mentioned; fields were not editable | None recorded |

**Result:** All three participants reached the end of the screen flow (3/3). The overall feedback was positive: the interface was considered simple and easy to follow. No specific improvement requests were recorded during these initial walkthroughs.

These results support the clarity of the screen navigation but do not establish the success rate for creating a real car listing, because participants could not fill in the fields.

## What I Took From the Test

| Observation | Design decision |
| --- | --- |
| All three people could get through the screens | Keep the guided flow |
| The simple interface was appreciated | Avoid overloading each step |
| Data entry was outside the scope of this test | Prepare a separate test with editable fields |
| Error recovery was not exercised with real inputs | Make error messages and return paths clear in the prototype |

Afterward, I also discussed the prototype with a first-time prospective seller. His requests for equipment selection and damage information informed later improvements; that interview is documented separately in [Homework 02](../02/README.md). The interview is not counted here as an additional fourth participant.

## Feedback on the Expanded Equipment Screen

Further feedback on the grouped Equipment & Condition screen was positive about the **visibility and meaning of the features and labels**. However, participants could not change the preselected equipment choices, and the long screen prevented them from reaching the **Continue to photos** action. They were able to go back from later screens they viewed.

The initial problem was traced to a 1360 px Figma frame with no scrolling. I reduced the viewport to 390 × 844 px and enabled vertical scrolling, preserving the existing Photos navigation link. **After the change, follow-up feedback indicated the navigation worked without further reported problems.** The participant count and individual outcomes for this confirmation were not recorded. At the time of that feedback, equipment choices and search were visual examples. A later iteration replaced the 16 equipment boxes with clickable checked/unchecked components and removed the nonfunctional search visual; the follow-up report now confirms the interactive choices work in Figma Present mode. The report did not include participant counts or per-option test results.

The participant count, individual timing and independence data for this later feedback were not supplied. It should not be added to the earlier 3/3 result as a new measured sample. [Follow-up test notes](https://github.com/umutcanbirbir/autopiac-ux-ui-design/blob/main/project/docs/prototype-test-feedback-2026-11-21.md).

## Additional Correction — Damage Status Controls

A further participant report found that the damage-status choices were still noninteractive. I changed the *Front-left fender* example into a five-state Figma component (Original / Repainted / Replaced / Damaged / Unknown), with one choice selected at a time and a matching Selected label. Its 20 between-state links and five displayed states were checked in the design file. After the revision, the student relayed positive follow-up feedback: the damage selections now work and participants found the screen simple and practical. The exact number of testers and individual outcomes were not documented.

[Current screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) · [Component variants](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2044-34).

## Participant-Level Usability Results — Clarified 23 November 2026

The student provided **individual outcomes for three participants (T01–T03)** after the earlier aggregate report. All three independently worked through the assigned Figma navigation/interaction tasks and reached the final screen. However, **the participants tested different design states**: T01 encountered broken controls and an unreachable Continue button, while T02 and T03 tested the corrected prototype.

| Participant | Prototype state | Completed assigned flow and tasks? | Navigation assistance | Findings | Approximate time |
| --- | --- | --- | --- | --- | --- |
| **T01** | Earlier problematic version, then corrected during the iteration/retest | **Yes**, reached final screen after the controls and Continue navigation were fixed | No step-by-step navigation guidance reported; the prototype required a design fix | Reported that buttons/selections did not respond and the Continue action was unreachable; successfully used Continue after the fix | **~4 minutes** in the reported test/retest process |
| **T02** | Corrected interactive version | **Yes**, reached final screen and completed the assigned tasks | None reported; completed independently | Controls and progression worked; positive response | **~1 minute** |
| **T03** | Corrected interactive version | **Yes**, reached final screen and completed the assigned tasks | None reported; completed independently | Controls and progression worked; positive response | **~1 minute** |

**Terminology:** The student confirmed that all three interpreted the interface terms correctly in Turkish. The recorded group translations are *Vehicle Details → araç detayları; Equipment → donanım; Review → incele; Publish → yayınla; Draft → kaydet*. The responses were direct translations/interpretations rather than separate word-for-word transcripts. The nuance between **Draft** and a saved but unpublished listing still deserves clear interface copy.

**Measurement limits:** Durations are approximate recollections reported by the student, **not individually stopwatch-verified measurements**. T01's ~4 minutes included encountering a defect and resuming after correction, so it is **not comparable as a pure completion-time benchmark** with T02/T03. The exact test dates, full action-by-action logs, device details and whether this three-person group overlaps with the earlier navigation walkthrough were not documented. Do not treat these as six unique users, claim precise timing statistics, or claim actual advertisement submission.

**Result:** **3/3 participants completed the assigned Figma walkthrough independently**, with the important qualification that T01 required the prototype to be corrected before the inaccessible continuation became usable. The reported issues prompted the fixes; T02 and T03 encountered no remaining blockers in the corrected flow.

[Follow-up evidence and participant table](../../project/docs/prototype-test-feedback-2026-11-21.md) · [Participant task guide](../../project/docs/usability-test-instructions.md)

## Mini UI Guideline

| Element | Guideline |
| --- | --- |
| Main colors | Yellow `#FFD400`, white `#FFFFFF`, dark text `#1F1F1F` |
| Buttons | Use yellow for the main action and an outlined secondary button for Back |
| Forms | Keep visible labels, required-field markers and examples |
| Errors | Explain what is wrong and how to correct it; do not rely on color alone |
| Progress | Show the current step and let people return to previous steps |
| Photos | Explain the five-photo minimum and identify the cover image |
| Layout | Use consistent 8/16/24/32 px spacing |
| Accessibility | Aim for WCAG 2.2 AA; check contrast, keyboard focus and targets |

Following that review, I conducted a separate [WCAG 2.2 AA design-level accessibility check](../../project/docs/accessibility-review-2026-11-22.md) on ten Figma frames (22 November 2026). I strengthened nine input outlines, enlarged the equipment and damage labels and adjusted photo captions. The 44 prototype action hit boxes examined were at least 36 px in each dimension, and an approximate check of 204 text layers identified no below-threshold pairs. This does **not** confirm keyboard, screen-reader or responsive reflow conformance.

## Test Conclusion and Limitations

The three participants' independence, overall completion, major defect observations, terminology comprehension and approximate times are now documented individually. This closes the Figma navigation/interaction test documentation gap. Detailed per-feature click logs, stopwatch timings and testing of editable form values are **not available** and are not invented; the lecturer requested a Figma prototype rather than a working marketplace.

The observed defect-to-fix sequence is the central outcome: T01 discovered the nonworking selections and unreachable Continue button, then could proceed following the correction; T02 and T03 completed the assigned tasks independently on the corrected version without reported control failures.



[Participant instructions and results template](../../project/docs/usability-test-instructions.md) · [Design changes](../09/README.md)

The **scrolling/navigation blocker is reported resolved** after retesting. Individual test sheets and a real form-completion test remain separate.
