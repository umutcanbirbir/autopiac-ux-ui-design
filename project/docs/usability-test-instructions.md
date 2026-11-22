# AutoPiac — User Test Guide

**Prepared:** 21 November 2026  
**Purpose:** Test the updated listing flow and gather feedback for Homework 05, 08 and 09.  
**Figma starting screen:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2  
**Equipment and condition screen:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2  
The Figma file is a clickable design prototype. All 16 equipment checkboxes on the current screen can be toggled individually. The front-left-fender condition is also clickable (Original / Repainted / Replaced / Damaged / Unknown). Other text fields and additional body panels remain examples; participants cannot save vehicle details or upload actual photos.

## Participants

Three different people have now tested the latest prototype. For any further structured test, recruit people who did not design the project and were not coached. If possible, include someone who has advertised a car before. Keep records anonymous as T01, T02, T03; ask permission before recording notes. Keep names, contact details and vehicle identifiers out of the public results.

## Script to Read or Send (English)

> I'm testing a UX/UI concept for a car-advertisement site called AutoPiac. Please open the Figma link and select the first mobile screen, then click Present (▶). This is a clickable design mockup, not a real application: you can click the equipment choices to select or deselect them, but you cannot enter and save vehicle data or upload actual photos. Please navigate without asking me for directions and tell me what you expect each screen or button to do.

## Most Important Retest

An earlier participant reported that the expanded Equipment & Condition page could not be scrolled to its Continue button. Scrolling has now been enabled and the follow-up report confirmed navigation. The 16 equipment choices have also been made clickable. **Ask the next participant to select Apple CarPlay and Heated seats, deselect ABS, then check that the other items keep their previous states.** Have them scroll to “Continue to photos” afterward. Record the outcome.

[Details of the reported issue and fix](https://github.com/umutcanbirbir/autopiac-ux-ui-design/blob/main/project/docs/prototype-test-feedback-2026-11-21.md).

## Tasks (Use This Order)

1. **Navigation:** Start a car listing and reach the final Review screen. Record whether they found the next steps **without help**. 
2. **Equipment lookup:** On Equipment & Condition, locate **Adaptive cruise**, **Heated seats**, **Apple CarPlay**, and **Rear camera**; ask which group each is in. Ask them to click each feature to toggle it, then click again to restore its starting state.
3. **Damage comprehension:** Point to how you would indicate a **replaced front fender**. Ask what "Repainted", "Replaced", "Damaged" and "Unknown" mean. Let them explain without hints.
4. **Photos and recovery:** Identify the minimum number of photos and the cover photo. If useful, click **Remove 3 photos** to view the error-example branch, then find the route back to the photo step.
5. **Review edit:** From Review, click **Equipment & condition · Edit** and see whether they understand where it leads.
6. **Terminology check:** Ask the participant to explain in their own words **Vehicle Details**, **Equipment**, **Review**, **Publish**, and **Draft**. Keep their answers separate from your own interpretation.
7. **Feedback:** Ask **"What was clear? What was confusing? Which item or detail was missing?"** 

## While Observing

- Ask the participant to **think aloud**, but do not explain the meaning of terms during the task.
- Start a stopwatch before the first task; stop at final Review if measuring duration.
- If they need help, note **when**, **what help you gave**, and whether they finished afterward.
- Separate what you **observed** from what the participant **said**.
- Remember that this test covers navigation and understanding, not functional data entry.
- Use a functional demo for a separate real form-entry test if needed.

## Notes for Each Participant

**Participant ID:** T__  
**Date and approximate time:**  
**Prior experience creating a car listing:** Yes / No / Prefer not to answer  
**Tested version:** Figma student copy, revised grouped equipment screen  
**Observed independently or remotely reported?**  
**Assistance provided?** None / Yes (record where)  
**Navigation to Review completed?** Yes / No  
**Time to Review (if actually measured):**  
**Equipment lookup and actual on/off toggling outcome for 4 specified features:**  
**Damage terms explained correctly?** Record individual answers  
**Photo minimum / cover comprehension:**  
**Review edit found?** Yes / No  
**Terminology answers (in participant's own words):**  
**Observed hesitation / errors:**  
**Participant's feedback:**  
**My notes on possible design changes:**

## Recorded Participant-Level Results (Student Clarification, 23 November 2026)

The following results relate to the **three distinct participants labelled T01, T02 and T03**. The actual test-session dates and exact stopwatch measurements were not supplied.

| ID | Prototype tested | Independent final-screen completion and assigned tasks | Terminology understood? | Approximate duration | Important observation |
| --- | --- | --- | --- | --- | --- |
| **T01** | Earlier controls/scrolling problem, then correction | **Yes, after the prototype fix**; user independently navigated | **Yes**, straightforward Turkish interpretations reported | **~4 minutes** (including problem discovery and correction/retest) | Identified buttons/selection controls not working; Continue reachable after correction |
| **T02** | Corrected Figma version | **Yes**, independently | **Yes**, straightforward Turkish interpretations reported | **~1 minute** | No remaining control or navigation problem reported |
| **T03** | Corrected Figma version | **Yes**, independently | **Yes**, straightforward Turkish interpretations reported | **~1 minute** | No remaining control or navigation problem reported |

**Recorded terminology examples:** Vehicle Details → araç detayları; Equipment → donanım; Review → incele; Publish → yayınla; Draft → kaydet. The examples are from the group's answers; individual word-for-word transcripts were not collected. "Draft" might benefit from more explicit "Save as draft" wording to express that an advertisement remains unpublished.

The time values are **student-reported approximations**. The 4-minute T01 session includes the original broken prototype and subsequent correction, so do not treat it as a controlled timing comparison with the roughly one-minute corrected-version runs. All three reported completing the assigned Figma interaction/navigation tasks, but detailed button-by-button logs are not available. No real data entry or publishing was tested. It is unknown whether this group overlaps with the earlier three-person navigation walkthrough.

The results are summarized in [Homework 08](../../homework/08/README.md) and [the follow-up feedback report](prototype-test-feedback-2026-11-21.md).

## Optional Template for a New Test

| Participant | Actual test date | Device | Independent task completion | Exact timed duration | Specific controls tried | Issues |
| --- | --- | --- | --- | --- | --- | --- |
| New test only | — | — | — | — | — | — |

This blank template is for any **future** structured retest, not a claim that T01–T03 are missing test records.
