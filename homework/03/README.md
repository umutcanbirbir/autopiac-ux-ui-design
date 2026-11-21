# Homework 03 — Competitor UX/UI & Accessibility Audit

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Date:** 2026-11-21  
**Method:** Public-documentation desk research; **not** hands-on testing of logged-in forms.  
**Primary competitor:** [Használtautó.hu](https://www.hasznaltauto.hu/)  
**Additional benchmark:** [mobile.de](https://www.mobile.de/en/sell/car/)

## Sources Reviewed
1. Használtautó.hu's official step-by-step listing guide: https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/
2. Használtautó.hu user-facing overview of listing requirements: https://garazs.hasznaltauto.hu/ha-autot-adnal-el/utmutato-hasznalt-auto-eladasahoz/
3. mobile.de's private selling guide: https://www.mobile.de/en/sell/car/
4. W3C Web Content Accessibility Guidelines (WCAG) 2.2: https://www.w3.org/TR/WCAG22/

## Evidence-Based Competitive Observations
- Használtautó.hu describes a multi-step flow: vehicle details, photos/documents, photo management, packages, promotions, and submission.
- The guide identifies mandatory fields such as make/model/variant and describes auto-filled fields that remain editable.
- It explains photo upload, ordering, and captions, then a separate offer/package choice.
- A success state confirms the created advertisement.
- The platform has significant feature depth; whether this makes the *current user interface* difficult requires direct testing.

## Six Audit Items: Observations, Risks & Proposed Improvements

| # | Documented observation / audit target | Potential usability risk (not verified defect) | AutoPiac response | How to verify |
| --- | --- | --- | --- | --- |
| 1 | Vehicle details include mandatory and auto-filled attributes. | A novice may confuse required and optional technical fields. | Separate essentials, optional details and contextual explanations. | User task observation |
| 2 | Photos are handled across upload and separate photo-management steps. | People may miss image-order controls or not know photo completeness. | Immediate preview, reorder and progress indicator. | Observe photo task |
| 3 | Users encounter package and promotion choices before finishing. | Sellers may misunderstand the effect of optional paid services. | Keep premium offer clearly optional, with transparent costs. | Comprehension test |
| 4 | The guide describes multiple sequential stages. | Progress and return navigation may not feel obvious. | Explicit stepper, saved draft and back navigation. | Step-navigation testing |
| 5 — accessibility check | Form field labels, required markers, and validation need direct inspection. | A screen reader may miss purpose or error cues **if** labels and messages are not programmatic. | Persistent text labels, associated errors, field-level instructions. | Keyboard + screen-reader inspection, WCAG 3.3.2 / 3.3.1 |
| 6 — accessibility check | Photo sorting and interactive controls need direct inspection. | Drag-only operation or undersized touch targets **if present** could exclude users. | Keyboard move-up/down alternatives and clear touch targets. | Keyboard-only testing, WCAG 2.1.1 / 2.5.8 |

**Important distinction:** The table describes confirmed *features from the guide* and **potential risks**. It does **not** claim six verified usability defects or confirmed accessibility violations.

## UI State Audit Checklist
- [ ] Loading state while submitting/uploading
- [ ] Empty photo collection
- [ ] Missing mandatory field
- [ ] Photo type/size upload error
- [ ] Network/server failure
- [ ] Draft recovery
- [ ] Successful publishing confirmation

## Scope and Limitation
A final evidence-based interface audit requires actually opening the competitor's listing screens (with appropriate access), recording annotated screenshots, and checking the six items. Do not describe these checks as completed.

## Early Design Implications
1. Make minimum required information unambiguous.
2. Provide contextual vehicle-data help without overwhelming the user.
3. Keep photos, preview, and error recovery easy to understand.
4. Distinguish core publishing from optional promotional purchases.
5. Use WCAG 2.2 as an accessibility verification framework.
