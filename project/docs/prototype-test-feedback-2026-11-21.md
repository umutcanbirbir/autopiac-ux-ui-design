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

All five variants and their labels were inspected, with 20 valid between-state click destinations verified. The corrected damage interaction still **needs participant confirmation in Present mode**. It currently illustrates one body panel, not an interactive 13-panel vehicle map, and does not store values or update Review automatically.

[Interactive condition component](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2044-34) · [Current listing screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2).

## Next Check

- [x] Follow-up feedback received: the revised prototype's navigation works and no further issue was reported; individual task details were not recorded.
- [x] No further scrolling or access problem reported after the fix; specific component visibility was not recorded separately.
- [ ] Check whether **Save as draft** would be clearer than **Draft**.
- [x] Add on/off interactions to all 16 equipment options using a Figma component.
- [x] Follow-up report says the interactive equipment selections work in Present mode; which individual options were exercised was not recorded.
- [ ] Ask a participant to switch the front-left fender from Replaced to Repainted, then Unknown, and confirm that only one status is selected each time.
- [ ] Record the actual number of participants, individual outcomes and any measured times before drawing quantitative conclusions.

[Homework 05 — Information Architecture](../../homework/05/README.md) · [Homework 08 — Usability Test](../../homework/08/README.md) · [Homework 09 — Design Iterations](../../homework/09/README.md)
