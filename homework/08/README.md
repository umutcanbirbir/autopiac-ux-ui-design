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

## Latest Prototype — Three Testers Confirmed

The student confirmed that **three different people tested the latest Figma prototype**. The final overall feedback from the three testers was consistently positive: **all three reported no problems and liked the design**, describing it as **simple and easy to use**. Earlier follow-ups also confirmed the equipment selections, front-left-fender choices and scrolling/continuation issue had been addressed.

These observations are reported **for the group**, not as three individual task records. There are no measured completion times, per-person assistance records or full task checklists for this latest round. It is not confirmed whether these people were also involved in the initial three-person navigation walkthrough, so the two groups are not combined into a six-person sample.

[Follow-up report](../../project/docs/prototype-test-feedback-2026-11-21.md)

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

Selected text-color pairs were checked during the later [design QA](../../project/docs/design-qa-2026-11-21.md); that is not a full accessibility audit.

## Next Test

The corrected Equipment & Condition navigation has now received positive follow-up confirmation. A further informal retest reported the on/off equipment selections worked. A structured test should still record results per participant for option selection, damage-status interpretation and Review editing, despite the positive informal feedback. I will record whether they needed help, what they could not find, and their feedback.

[Participant instructions and results template](../../project/docs/usability-test-instructions.md) · [Design changes](../09/README.md)

The **scrolling/navigation blocker is reported resolved** after retesting. Individual test sheets and a real form-completion test remain separate.
