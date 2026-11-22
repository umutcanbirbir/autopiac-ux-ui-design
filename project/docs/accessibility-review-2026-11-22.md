# AutoPiac — WCAG 2.2 AA Design-Level Accessibility Review

**Student:** Umut Can Birbir (DUJ3ZD)  
**Date:** 22 November 2026  
**Scope:** Current mobile-first [AutoPiac Figma prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2), including vehicle details, equipment/condition, photo stage, price and description, Review, success, two example errors and one desktop details frame. Ten screen frames were inspected.

**Standard:** [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/). This is a **visual and structural design review**. The prototype is not an accessible production website, and this document is **not a WCAG certification**.

## 1. Method

I inspected the ten current Figma frames, their text sizes, text/background fills, input borders, prototype link hit boxes, component states, mobile viewport dimensions and navigation reactions. I visually reviewed the current vehicle, equipment, photo and price screens. I inspected the interactive equipment toggle and five-state front-left-fender component after the adjustments.

A Figma script checked **204 text layers**, comparing each text fill with the nearest visible solid ancestor fill and using WCAG luminance contrast calculations; **no pair fell below the estimated 4.5:1 normal-text / 3:1 large-text thresholds** in that model. **This is a spot-check approach, not a pixel-perfect conformance test**: composite fills, overlays, different rendering environments and component semantics can affect outcomes. The nearest-ancestor color may differ from the final rendered background in complex layouts.

The same inspection identified **44 prototype interaction hit boxes** across the ten reviewed frames. The smallest observed width or height among them was **36 px**. This exceeds the WCAG 2.2 AA **2.5.8 Target Size (Minimum)** baseline of 24 × 24 CSS pixels, although full actual implementation hit areas were not tested. For touch usability, the developer handoff still recommends a **44 × 44 px target where practical**; 44 px is a recommended design target, **not** the WCAG 2.5.8 AA threshold.

## 2. Issues Found and Corrected in Figma

| ID | Evidence | Correction made | Result / limit |
| --- | --- | --- | --- |
| A11Y-01 — Low-contrast field outlines | Nine input/textarea boundaries on Vehicle Details, Price & Description and Equipment/Condition used **#D5D0C4 on white**, about **1.54:1**, below the 3:1 non-text boundary contrast target when their outline identifies the input. | Set all nine to **#8A8275**, about **3.80:1** against white. | Improved essential form-field visibility. WCAG **1.4.11 Non-text Contrast** relevant for visible control boundaries. |
| A11Y-02 — Small equipment labels | All 16 interactive equipment choices used **10 px** text in selected/unselected variants. | Increased both shared component variant label sizes to **13 px**. | The existing 16 instances inherit the improvement. On/off interactions and initial states remain in place. |
| A11Y-03 — Small damage-status labels | The five status names used **10 px** text in each of five condition variants. | Raised the label and radio glyph sizes to **12 px**, widened the text boxes, and changed the status summary from 11 to 12 px. | Five mutually exclusive states remain linked; 20 transitions between different states remain available. |
| A11Y-04 — Tiny photo labels / helper text | Thumbnail captions such as PHOTO and COVER used **9 px**. Some supporting hints were 11 px. | Raised five captions to **11 px**, expanded their text boxes and increased selected helper copy to **12 px**. | Improved readability without changing the existing photo guidance and action layout. |
| A11Y-05 — Missing implementation instructions | Figma only visually simulates selections; a click reaction is not an accessible HTML checkbox or radio group. | Updated [Developer Handoff](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55) to specify native checkbox/radio semantics, keyboard interaction, visible focus and announced states. Clarified the difference between 24 px WCAG minimum and 44 px preferred touch size. | Handoff improved; **real keyboard and assistive-technology behavior cannot be certified in Figma**. |

**Note on font size:** WCAG 2.2 does not mandate a universal 12, 13 or 16 px minimum font size. These typography changes were practical readability improvements, not a claim that 10 px automatically violates WCAG.

## 3. Checks Completed

| WCAG success criterion | Evidence from the prototype | Assessment |
| --- | --- | --- |
| **1.4.3 Contrast (Minimum)** | 204 text layers compared in an approximate direct-fill/nearest-ancestor analysis; no ratios flagged below 4.5:1 for normal text or 3:1 for large text. Earlier documented text pairs included yellow/dark text and error red/white. | **Design-level spot check passed**; not formal certification |
| **1.4.11 Non-text Contrast** | Nine essential input borders improved from 1.54:1 to 3.80:1 against white. | **Specific input-outline issue corrected**; not a complete icon/state audit |
| **2.5.8 Target Size (Minimum)** | 44 Figma interaction boxes inspected, minimum dimension 36 px. | **Observed prototype surfaces meet 24 px dimension**; real hit areas unknown |
| **1.4.1 Use of Color** | Equipment choices use checkbox glyphs as well as selected yellow backgrounds; fender states use a selected indicator and a Selected: text label. | **Multiple visible cues present** in these components |
| **3.3.1 Error Identification** | Separate missing-required-fields and not-enough-photos screens display explanatory text and return routes. | **Design examples present**, not actual input validation |
| **3.3.2 Labels or Instructions** | Vehicle and price fields have persistent visible labels and * required indicators; photo minimum is stated. | **Visual guidance present**; programmatic field-label association not tested |
| **2.5.7 Dragging Movements** | Photo ordering is described in the developer handoff as requiring move alternatives. Current Figma photos are illustrative. | **Implementation requirement documented**, not implemented |

## 4. What Cannot Be Verified Yet

**Needs an actual functional frontend:**

- **2.1.1 Keyboard:** Tab order, Enter/Space checkbox activation, radio-group arrow-key behavior and usable keyboard navigation.
- **2.4.7 Focus Visible / 2.4.11 Focus Not Obscured:** Visible focus indicator for every working control, including any sticky elements or scrolling areas.
- **4.1.2 Name, Role, Value:** Actual screen-reader names, checkbox checked state, radio-group selection, errors and announcements. Figma visual variants do not provide this guarantee.
- **1.4.10 Reflow / 1.4.4 Resize Text:** Layout at narrow 320 CSS px and 200% browser text size without clipped information or two-dimensional scrolling. The Equipment & Condition prototype uses a vertically scrolling 390 × 844 frame; reflow is not established.
- **1.3.1 Info and Relationships:** Heading hierarchy, form grouping and label/control associations in HTML.
- **Photo accessibility:** Useful alternative text for meaningful vehicle photos, cover identification, accessible remove/move controls and non-drag sorting.
- **Form error behavior:** Actually moving focus to invalid fields, preserving values, announcing errors and supporting retry/publishing.
- **Real-device focus and target areas:** The script measured Figma frames, **not the browser's actual clickable CSS hit regions**.

**Limitations of the course deliverable:** Vehicle inputs and photo upload are still illustrative. All 16 equipment options and one front-left-fender condition component respond visually in Figma, but values are not saved or synchronized with Review. These constraints should remain explicit when presenting the project.

## 5. Recommended Implementation Checks

1. Build real, labelled fields and accessible native checkbox/radio controls, with visible focus rings and keyboard operation.
2. Confirm all essential input borders, icons and selected states at **3:1 non-text** contrast, and ordinary text at **4.5:1**, including error states and focus.
3. Test a 320 CSS px layout and 200% text zoom; ensure content can scroll vertically, buttons remain reachable and the text is not cut off.
4. Add aria-describedby or native descriptions for required hints and error messages only as needed; connect labels to fields programmatically.
5. Use actual browser tools and at least one screen reader to validate control names, state changes and error announcements.
6. Offer move-up/down controls for photo ordering instead of requiring drag gestures.
7. Re-test the implemented UI with keyboard-only navigation and participants who use assistive technology if feasible.

## Relevant Screens and References

- [Vehicle Details](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-25)
- [Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2)
- [Photos](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-62)
- [Price & Description](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-83)
- [Figma handoff notes](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55)
- [Earlier visual review](design-qa-2026-11-21.md)
- [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/)
- [W3C Understanding 1.4.3 Text Contrast](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html)
- [W3C Understanding 1.4.11 Non-text Contrast](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast)
- [W3C Understanding 2.5.8 Target Size](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum)

**Conclusion:** The revised Figma prototype now has more legible equipment and condition text, visible input boundaries above 3:1, and observed action boxes larger than 24 px. The design is **better prepared for accessible implementation**, but the complete product has **not** been tested or certified as WCAG 2.2 AA conformant.
