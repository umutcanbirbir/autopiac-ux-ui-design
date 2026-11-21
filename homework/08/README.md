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

I plan to ask three additional people to use the **latest** Figma version, locate specific equipment options, interpret damage statuses and try the Review editing links. I will record whether they needed help, what they could not find, and their feedback.

[Participant instructions and results template](../../project/docs/usability-test-instructions.md) · [Design changes](../09/README.md)

The latest equipment revision has not yet been independently tested, and a real form-completion test remains separate.
