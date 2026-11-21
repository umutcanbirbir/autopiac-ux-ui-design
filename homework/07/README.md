# Homework 07 — Interactive Figma Prototype

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Basic clickable frame navigation implemented; actual feedback and data-aware interactions pending.
**Figma file:** https://www.figma.com/design/cEkbZFkMY32FYY4q5op5Jm

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

## Peer Feedback Plan
Ask at least one real student to try the flow and note a minimum of three specific pieces of feedback. Do not script the feedback for them.

| Tester | Date | Feedback observation | Follow-up action |
| --- | --- | --- | --- |
| Not yet tested | — | — | — |

## Completion Checklist
- [x] Figma prototype share link.
- [x] Connected frame-to-frame main task path (not dynamic forms).
- [x] Success screen, photo error branch and missing-vehicle-field error frame created. The required-field branch needs wiring into a complete data-aware interaction model.
- [ ] At least one actual peer walkthrough.
- [ ] Three recorded concrete observations.
