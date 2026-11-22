# AutoPiac — Follow-Up Prototype Feedback and Navigation Fix

**Notes prepared:** 21 November 2026  
**Design reviewed:** [Equipment & Condition — expanded equipment list](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2)  
**Source:** Feedback relayed by the student following participants' use of the latest Figma design.

## What Participants Reported

Participants could see the equipment categories and generally understood the information on the screen. They could **not change which equipment features appeared selected**. The Figma checkbox states were visual examples rather than functional inputs.

The main obstacle was navigation: the long Equipment & Condition screen did **not allow users to reach the Continue to photos button**. They were able to navigate backward from later pages they viewed.

The terminology check was reported as follows:

| English term | Participant interpretation (Turkish) | Note |
| --- | --- | --- |
| Vehicle Details | Araç detayları | Meaning understood |
| Equipment | Donanım | Meaning understood |
| Review | İncele | Meaning understood |
| Publish | Yayınla | Meaning understood |
| Draft | Kaydet | Related to saving, but less specific than an unfinished draft; check whether “Save as draft” is clearer |

Participants generally understood the content they saw. **The number of people represented in this particular feedback, their individual outcomes, previous car-selling experience, task times, assistance and exact session date were not supplied.** Therefore, this note does not report a numerical success rate or count these as additional distinct participants.

## Problem and Design Response

**Problem:** The Equipment & Condition Figma frame had a 1360 px canvas height and no scrolling (`overflowDirection: NONE`). Its next-step action appeared near the bottom at y = 1221 px, out of reach for people viewing the mobile prototype.

**Fix implemented:** The same frame was changed to a **390 × 844 px mobile viewport with vertical scrolling enabled** (`overflowDirection: VERTICAL`). Its content extends past the viewport, and users should now be able to scroll to the lower Damage & Replacement History section and the Continue to photos action. The original continue link to the Photos frame and back link to Vehicle Details were preserved.

**Follow-up confirmation:** After the scrolling change, the student reported that the people who tried the revised prototype found the navigation working and did not report further problems. This supports closing the specific **unreachable Continue to photos** navigation issue. No individual participant count, time or device information was provided for this confirmation. Equipment checkboxes and search remain visual Figma elements; this confirmation does not establish functional form editing.

## Subsequent Update — Interactive Equipment Choices (22 November 2026)

I built a reusable Figma Equipment Toggle component with two On/Off variants and bidirectional click interactions, and converted all **16 equipment choices** into independent interactive instances. The checkboxes now have changeable prototype states, while their labels remain intact. I removed the nonfunctional equipment search placeholder and added a prompt to tap options to select or deselect them.

The variant switch and label preservation were checked programmatically in Figma. **Follow-up response (22 November 2026):** After the interactive variant update, the student relayed that the people who tested the equipment options said the selections **worked** in Figma Present mode. This is a positive reported retest of the toggle interaction, not a measured task-completion rate. The exact participant count, individual outcomes and whether every one of the 16 controls was tried were not recorded. Choices do not persist to listing data or synchronize the Review example.

[Interactive options](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) · [Component variants](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2040-9).

## Subsequent Correction — Interactive Fender Condition (22 November 2026)

After the equipment checkbox retest, the student reported that the **damage-status options remained noninteractive**. I replaced the static status chips for the *Front-left fender* with a reusable five-variant Figma component. It supports **Original, Repainted, Replaced, Damaged and Unknown** as mutually exclusive states. Selecting a different status updates the selected radio-style option and the status text.

All five variants and their labels were inspected, with 20 valid between-state click destinations verified. **Follow-up after the correction:** The student reported that the testers could now use the damage-status choices and described the revised screen as simple and practical. This confirms that the previously reported interaction blocker was resolved for those testers. The number of participants, individual steps, timings and assistance were not recorded. It currently illustrates one body panel, not an interactive 13-panel vehicle map, and does not store values or update Review automatically.

[Interactive condition component](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2044-34) · [Current listing screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2).

## Participant-Level Clarification — 23 November 2026

The student identified the **three individual testers** as T01, T02 and T03 and provided their task completion, issue observations, independent use, terminology and approximate durations. This supplements earlier group-level reports; it does not change historical notes about information unavailable when they were first written.

| ID | Test state | Independent assigned tasks and final-screen navigation | Reported observation | Estimated time |
| --- | --- | --- | --- | --- |
| **T01** | Started before the control/scroll fixes, continued after corrections | **Completed**; reached the final screen without navigation coaching after the prototype was fixed | Explicitly found and reported that buttons or selectable controls did not work. The Continue action only became reachable after design correction | **Around 4 min**, including dealing with problems and resuming after changes |
| **T02** | Corrected prototype | **Completed** independently | Buttons and interactions worked; positive feedback | **Around 1 min** |
| **T03** | Corrected prototype | **Completed** independently | Buttons and interactions worked; positive feedback | **Around 1 min** |

**Terminology interpretation:** All three were reported to understand the interface terms correctly and give straightforward Turkish translations/interpretations. The recorded shared terms are *Vehicle Details → araç detayları; Equipment → donanım; Review → incele; Publish → yayınla; Draft → kaydet*. There are no verbatim per-user answer transcripts. A "save" interpretation of **Draft** does not conclusively demonstrate understanding of unpublished status.

**Usability finding:** T01 exposed actionable problems in the interactive design. After correcting prototype scroll reachability and control states, T01 could continue, while T02 and T03 independently completed the given tasks on the corrected version without reported failures. This demonstrates a real feedback → fix → retest cycle within a **Figma prototype**, not a full listing application.

**Evidence quality:** Completion and times are based on the student's account, not independent recordings. Approximate durations must **not** be used as exact stopwatch observations; T01's longer session includes problem discovery and recovery. The precise sequence/date of every fix during T01's test, previous listing experience, click-by-click outcomes and any overlap with the initial three-person navigation group remain unknown. We therefore do **not** claim that three users all tested the final corrected version from the beginning, six unique users, precise mean task time or working backend publication.

## Final Figma Usability Test Status

- [x] Three participants identified separately as **T01, T02, T03**.
- [x] Independent completion of assigned Figma tasks and reaching the final screen reported for all three, subject to T01's prototype fix.
- [x] Individual approximate durations recorded: **~4 / ~1 / ~1 minutes**.
- [x] Defect discovery and corrected prototype results differentiated by tester.
- [x] Correct Turkish terminology comprehension reported for all three, with shared rather than verbatim individual translations.
- [x] Student confirmed the corrected prototype controls worked during T02 and T03 sessions.
- [ ] Optional: capture exact timestamped task logs, individual answer transcripts and stopwatch measurements in a new study, if specifically required. These are not necessary to truthfully report the existing sessions.

[Homework 05 — Terminology](../../homework/05/README.md) · [Homework 08 — Individual test results](../../homework/08/README.md) · [Homework 09 — Iterations](../../homework/09/README.md)
