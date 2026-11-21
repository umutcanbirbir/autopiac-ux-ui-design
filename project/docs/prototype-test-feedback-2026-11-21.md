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

**Not yet verified:** A new participant has **not yet confirmed** that the repaired scrolling behavior works in their Figma presentation environment. The checkboxes and visual search field also remain static. This is a navigation fix, not an interactive equipment form.

## Next Check

- [ ] Ask a participant to reopen the revised prototype, scroll past the equipment section and reach **Continue to photos** without help.
- [ ] Confirm that the Damage & Replacement History section is visible while scrolling.
- [ ] Check whether **Save as draft** would be clearer than **Draft**.
- [ ] If selection behavior is required for the task, test it in an interactive prototype with changeable controls.
- [ ] Record the actual number of participants, individual outcomes and any measured times before drawing quantitative conclusions.

[Homework 05 — Information Architecture](../../homework/05/README.md) · [Homework 08 — Usability Test](../../homework/08/README.md) · [Homework 09 — Design Iterations](../../homework/09/README.md)
