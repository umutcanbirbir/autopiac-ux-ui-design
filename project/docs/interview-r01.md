# AutoPiac — Exploratory Interview & Prototype Walkthrough (R01)

**Project:** AutoPiac UX/UI Semester Project  
**Research record prepared:** 2026-11-21  
**Interview date:** Not separately confirmed  
**Research type:** Informal interview combined with a navigation-only Figma prototype walkthrough  
**Source:** Project owner's report of an actual conversation with their sibling; researcher did not independently observe or record the session  
**Participant ID:** R01 (anonymous; 18 years old)  
**Relationship to researcher:** Researcher's sibling (convenience recruitment; potential familiarity/positivity bias)  
**Previous car-listing experience:** Has never posted a car advertisement online  
**Session duration:** Not recorded  
**Prototype:** [AutoPiac Figma design](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)

## 1. Objective

Understand how a first-time prospective car seller perceives the AutoPiac listing flow, whether navigation is understandable, and which important listing details appear to be missing.

**Scope limitation:** This was not a full functional listing creation task. Figma has static visual inputs; no actual equipment selections, damage entries, photo uploads or publishing occurred.

## 2. Interview & Walkthrough Notes (Paraphrased, Not Direct Quotes)

These observations are faithfully paraphrased from the owner's account. **No verbatim user quotation, time stamp, task completion time or recording was supplied.**

| Topic | Participant report (via owner) | Meaning for design |
| --- | --- | --- |
| Experience | 18 years old; never previously created a vehicle listing | Represents a potentially relevant first-time-user perspective; not evidence from an experienced seller |
| Simplicity | Liked the interface; described it as simple, with few/limited options rather than a complicated selection/search interface | Keep the main steps and choices focused; do not treat this as a formal search usability test |
| Understanding | Understood the elements presented in the prototype; reported no confusing terminology | No demonstrated label problem in this single session |
| Navigation | Completed the available Figma interaction flow independently, with no reported assistance | Supports navigation comprehension, **not** real form completion |
| Missing content 1 | Could not choose or specify equipment/features for the car | Add a clear **Vehicle Equipment / Features** section |
| Missing content 2 | No dedicated place for damage information or repaired/replaced vehicle parts | Add a **Damage & Replacement History** section with structured, comprehensible disclosure |
| Other negative feedback | None was reported | Do not infer that other deficiencies are absent |

## 3. Supported Findings

**F-01 — The prototype is understandable to this first-time participant.**  
Evidence: R01 reportedly understood the interface and completed its available navigation independently, without getting confused by displayed terminology. General reaction was positive toward simplicity.  
Caution: One convenience-recruited participant cannot establish that all sellers will have the same experience.

**F-02 — Equipment information is an important missing part of the listing task for this participant.**  
Evidence: R01 explicitly pointed out that users cannot choose vehicle equipment/features.  
Design requirement candidate: A multi-select equipment section (e.g., climate control, parking sensors, navigation) with "Other" or "Not sure" handling and clear distinction between equipment and condition.

**F-03 — Vehicle damage/repair disclosure is another missing part of the flow for this participant.**  
Evidence: R01 explicitly identified the absence of an area for damage and replaced parts.  
Design requirement candidate: Dedicated condition/disclosure step with **Original / Repainted / Replaced / Damaged / Unknown** panel states, clear explanations, and optional notes/photos. Precise taxonomy and legal obligations must be verified separately; this is a design concept, not a statement of mandatory local disclosure law.

## 4. Initial Affinity Mapping (Real Notes Only)

| Theme | Evidence note | Result |
| --- | --- | --- |
| Clarity & learnability | "Simple / understood elements / independent navigation" — paraphrased owner report | Keep step-by-step flow |
| Vehicle completeness | "Cannot select car equipment" — paraphrased owner report | Add structured equipment choices |
| Vehicle transparency | "No damage/replaced-parts section" — paraphrased owner report | Add structured damage & repair history |

**Important:** Three affinity categories above arise from one session and may not be recurring themes in the wider population. This is a small, evidence-limited first synthesis, not validated saturation.

## 5. Evidence-Based Persona Snapshot (R01-Based, Anonymized)

**Persona label:** "First-Time Prospective Seller" (persona-style profile; **not** a fictional research participant).

- **Known:** 18 years old; has not posted a vehicle listing before.
- **Observed/reported behavior:** Could navigate AutoPiac's current prototype independently.
- **Positive preference:** Appreciated a simple, not overly busy interface.
- **Task expectations:** Wants to specify a vehicle's equipment and its damage/replaced-parts history.
- **Design needs inferred from feedback:** Structured choices rather than leaving important details in free-form description.
- **Not known:** Location, device preferences, car ownership, occupation, accessibility requirements, time to complete a real task, familiarity with technical vehicle terms beyond those shown.

This profile is sourced from a **single interview**. The project's older fictional persona "Márk" remains an assumption-based design aid and should not be presented as a validated user.

## 6. Journey Map — Reported Touchpoints and Proposed Future Steps

| Stage | Evidence status | Experience / concern | Design opportunity |
| --- | --- | --- | --- |
| Enter listing flow | **Reported observation** | Could progress independently; liked simplicity | Preserve straightforward navigation |
| Vehicle details | **Reported gap** | Equipment/features cannot be selected | Add dedicated optional equipment choices |
| Vehicle condition | **Reported gap** | No structured way to disclose damage or replaced parts | Add damage/repair history and visual panel selection |
| Photos | **Not independently assessed** | No actionable observation about file upload from this interview | Keep existing photo flow, test later |
| Price & description | **No specific observed issue** | Current labels understood generally | Avoid unnecessary complexity |
| Review / submission | **Reported navigation only** | Reached end of prototype; no actual submission performed | Reflect newly collected equipment and condition data in review |

## 7. Decisions & Follow-Up Test

Two feature additions were **proposed from real participant feedback**; their initial **static Figma mockup** has since been implemented at [Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2). They have not been re-tested:

1. **Equipment selector** within Vehicle Details or a compact "Features" subsection.
2. **Damage & Replacement History** as a clearly explained condition subsection with structured body-panel selection and explanatory text.

### Follow-Up Questions for R01 or Another Participant
- Which equipment items should appear first? Can you find your car's features?
- What is the distinction between "Repainted", "Replaced", "Damaged" and "Unknown"?
- Can you record repaired panels without feeling accused of hiding information?
- Would a dedicated damage step feel too long or still straightforward?
- Can you return from Review and correct a selected feature or panel status?

### Validation That Is Still Needed
- [x] One real, owner-reported interview/walkthrough recorded.
- [x] At least two distinct evidence-linked findings from that one interview.
- [x] Anonymized persona-style snapshot and evidence-labeled journey map.
- [x] Preliminary theme clustering using authentic reported notes.
- [ ] Confirm actual session date, duration, consent for academic use if required by the course.
- [ ] Collect additional participants to check if findings recur.
- [x] Implement illustrative equipment/damage controls in Figma (static selections, no saved data) and link revised Review screen.
- [ ] Perform and record at least one **post-change test**.
- [ ] Evaluate a realistic task using functional inputs; the Figma fields do not accept data.

## FigJam Synthesis

An R01 affinity/themes diagram using only the actual reported themes was added to the [AutoPiac FigJam board](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB).

## 8. Research Integrity

The interview participant is the owner's sibling and may be especially familiar with the project; this relationship limits independence. The participant is also inexperienced at selling cars. The account is second-hand and does not contain audio, notes with timestamps, or direct quotations. These limitations are explicitly disclosed. The initial three-person navigation walkthrough documented in Homework 08 remains a separate study; R01 is **not counted as a fourth distinct person** unless the project owner verifies that relationship.
