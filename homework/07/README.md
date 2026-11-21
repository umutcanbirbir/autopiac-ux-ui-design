# Homework 07 — Interactive Figma Prototype

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Clickable screen navigation implemented. One additional first-time-user walkthrough and informal interview documented; actual data-aware interaction testing remains pending.
**Figma file:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC

## Primary Interaction Path
Start → Vehicle Details → Photo Upload → Price & Description → Review → Publish → Success.

## Navigation Behaviors
- **Next:** Validate mandatory information, keep existing entries, move to the next stage.
- **Back:** Return to the previous step without losing entered data.
- **Edit on review:** Jump directly to the relevant step, then return to review.
- **Publish:** Show a success message only in the valid branch.
- **Invalid submission:** Reveal error details and a correction path.

## Prototype State Coverage
| State | Interaction | Expected behavior |
| --- | --- | --- |
| Default | User lands on an empty step | Clear instructions and fields |
| Missing required data | Continue clicked | Explain missing fields |
| Too few photographs | Continue clicked | Display minimum-5 requirement |
| Review-ready | Required data completed | Present structured summary |
| Success | Publish clicked in valid flow | Show confirmation |

## Peer Feedback — Real Interview & Walkthrough (R01)

The project owner reported an interview plus Figma navigation walkthrough with their 18-year-old sibling, a first-time prospective seller who had never posted a vehicle listing. The participant understood the screens and navigated the available prototype independently; Figma controls did not accept actual data.

| Evidence ID | Actual feedback (paraphrased, not a direct quotation) | Design response |
| --- | --- | --- |
| PF-01 | Positive response to the simple, not overly busy interface | Keep the guided linear journey rather than adding unnecessary complexity |
| PF-02 | Could not select a vehicle's equipment/features | Plan dedicated equipment selection |
| PF-03 | Missing damage/replaced-parts information area | Plan dedicated damage and repair-history disclosure |

**These are three authentic observations, of which two are concrete design shortcomings.** No task duration was recorded, and the exact interview date was not separately confirmed. This participant is a relative of the project owner; the study is limited by convenience recruitment.

[Detailed R01 research report](../../project/docs/interview-r01.md) · [Homework 02 synthesis](../02/README.md)

## Remaining Prototype Validation

- The walkthrough confirms **navigation only**, not accurate form entry or user ability to recover from real validation errors.
- Equipment and damage sections are **new proposals from actual feedback**, not yet tested improvements.
- A subsequent user/peer test should evaluate the changed prototype after implementation.
- The three-person first navigation walkthrough in Homework 08 is reported separately. Do not add this relative as a fourth unique test participant unless the identities are confirmed to differ.

## Completion Checklist
- [x] Figma prototype share link.
- [x] Connected frame-to-frame main task path (not dynamic forms).
- [x] Success screen, photo error branch and missing-vehicle-field error frame created. The required-field branch needs wiring into a complete data-aware interaction model.
- [x] One reported first-time-user walkthrough documented (R01, researcher's sibling).
- [x] Three concrete feedback observations captured (one positive + two missing features).
- [ ] Retest equipment/damage additions after implementation.
