# Homework 02 — User Research, Persona & Journey Map

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** One real interview and prototype walkthrough **reported by the project owner**; initial synthesis documented. Further participants and validation remain advisable.  
**FigJam:** https://www.figma.com/board/FReaY560jfsj9gfCeta8oB (R01 affinity themes diagram added)  
**Detailed primary record:** [Research Interview R01](../../project/docs/interview-r01.md)

## Research Question

How do private vehicle sellers, particularly first-time users, understand AutoPiac's listing creation process? Which vehicle attributes and disclosures do they expect to be able to enter?

## Research Method

- **Method:** Informal interview + navigation-only walk-through of the existing AutoPiac Figma prototype.
- **Participant:** R01, 18 years old, no previous experience placing a vehicle advertisement.
- **Recruitment:** The project owner's sibling (convenience sampling; potential familiarity bias).
- **Reported performance:** Navigated the prototype independently and understood the interface shown.
- **Interview session date / duration:** Not recorded; this written report was prepared on 2026-11-21.
- **Protocol limit:** Prototype inputs are static. Actual feature selection, condition entry, uploads and real publishing could not be performed.
- **Evidence:** Owner's paraphrased account, not direct quotes or independent researcher's observations.

## Results — Actual Participant Feedback

**Positive:** R01 liked AutoPiac's simplicity and limited visual/selection complexity, reported understanding the interface and navigating it without assistance.

**Two explicitly mentioned deficiencies:**
1. No dedicated way to select the car's **equipment and features**.
2. No dedicated section for **vehicle damage or replaced/repaired body parts**.

No other criticism or confusion was reported. The absence of reported difficulty is **not** proof that every interaction is usable.

## Initial Evidence-Backed Insights

| ID | Real reported evidence | Insight / design implication |
| --- | --- | --- |
| INS-01 | The participant described the interface as simple and could navigate it without help | Preserve the guided linear flow and avoid overloading the primary steps |
| INS-02 | The participant noticed they could not select equipment | Add an organized equipment selector with sensible categories and optional choices |
| INS-03 | The participant noticed no damage/replaced-parts section | Add structured condition/history disclosure with understandable terms |

These are **findings from one person**, not population-level conclusions.

## Preliminary Affinity Map — Three Authentic Themes

| Theme | Authentic paraphrased note | Candidate action |
| --- | --- | --- |
| Simple navigation | Understood the interface and finished available navigation unaided | Keep the core step-by-step flow |
| Listing completeness | Wanted selectable equipment/features | Add a feature selection section |
| Condition transparency | Wanted to disclose damage and replaced parts | Add body-panel/damage information |

The themes above are intentionally limited to what this participant actually reported. [Full synthesis](../../project/docs/interview-r01.md).

## Evidence-Based Persona Snapshot (Limited-Sample)

**Label:** First-Time Prospective Seller — R01-informed snapshot  
**Age:** 18  
**Experience:** Has never published a vehicle listing  
**Reported behavior:** Completed Figma screen navigation without assistance and understood the existing interface  
**Preferences:** A straightforward, not overloaded process  
**Expressed unmet needs:** Select vehicle equipment and disclose damaged/replaced parts  
**Not known:** Car ownership, device preference, location, listing task time, level of vehicle expertise, accessibility needs

**Caution:** This is a small research-based persona snapshot, **not** an independently validated representative archetype. The older hypothetical "Márk" profile was an initial design aid and is superseded for this submission.

## User Journey — Evidence-Labeled

| Phase | Directly reported? | Participant perspective | Proposed improvement |
| --- | --- | --- | --- |
| Start and navigate | **Yes** | The flow was understandable and simple | Keep guided steps |
| Specify the vehicle | **Gap reported** | Could not select equipment | Add equipment categories / checkboxes |
| Describe condition | **Gap reported** | No damage / repaired or replaced panels section | Add condition history and body-panel state selection |
| Add photos | **No specific finding** | Not tested as a real upload | Revisit during functional testing |
| Price and description | **No specific finding** | No criticism reported | Preserve concise labels |
| Review and finish | **Navigation only** | Reached the end; no real listing submitted | Include equipment/damage summary and editing |

## Design Revision from R01 Feedback

A first Figma redesign now shows vehicle-equipment sample choices and a damage/replacement-history panel in the existing listing flow. [View the added Equipment & Condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2). The Review screen links back to this new section. These are illustrative, static Figma controls and are **not** real interactive feature selectors. **Effectiveness has not been re-tested.**

## Design Direction

Add the missing structured sections **without turning the simple flow into an intimidating long form**. Use optional disclosure panels with concise explanations and a summary on Review. Test whether a combined "Equipment & Condition" screen or two short subsections is easier to understand; do not assume the preferred layout.

## Remaining Work

- [x] At least one genuine interview/walkthrough documented using an anonymous participant ID.
- [x] Two specific user-raised content gaps recorded.
- [x] Initial affinity themes based only on real reported feedback.
- [x] Evidence-informed persona snapshot and user journey.
- [ ] More interviews/observations for stronger evidence and more diverse perspectives.
- [ ] Verify the exact session date and permission for academic use, if required.
- [x] Add an equipment-and-condition design screen in Figma.
- [ ] Conduct a follow-up user test after the changes.
- [ ] Record task time, actual data entry and error recovery on a prototype supporting those interactions.

**Research integrity:** No invented participant quotations, precise durations, demographic details or additional interview subjects.
