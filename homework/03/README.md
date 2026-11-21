# Homework 03 — Evidence-Based Competitor UX/UI & Accessibility Audit

**Project:** AutoPiac — Private Car Listing Experience  
**Student:** Umut Can Birbir (DUJ3ZD)  
**Research date:** 2026-11-21  
**Status:** Official-source competitor desk audit completed; direct logged-in interface interaction and formal accessibility testing were **not** performed.  
**Competitors:** Használtautó.hu (Hungarian primary competitor); mobile.de (German market benchmark)

## 1. Goal and Research Method

Compare two established online vehicle marketplaces with AutoPiac's seller journey. Identify evidenced features, likely user needs, potential friction points, and principled design responses.

**Method:** Review public first-party guides, step-by-step screenshots described and embedded in Használtautó's official guide, official seller advice and listing documentation from mobile.de. **No account login, interactive competitor form walkthrough, screenshot annotation of live form states, automated accessibility audit, or participant comparison was carried out.** Treat any potential UX defect as a *hypothesis*, not an observed failure.

### Source Log (Primary / Official Sources)

| Source | What it directly supports | Access / limitation |
| --- | --- | --- |
| [H1: Használtautó — step-by-step advertisement guide](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/) | Advert creation steps; partially auto-populated editable vehicle fields; photo/document upload; separate image ordering/captions; package choice; contains illustrative screenshots | Describes a published flow; live current logged-in form not tested |
| [H2: Használtautó — successful listing advice](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-hirdess-a-hasznaltauto-hu-n-a-sikeres-jarmuhirdetes-titka-5-percben/) | Equipment checkboxes, description recommendations, relevant listing completeness and buyer trust | Seller guidance; not a measured usability study |
| [H3: Használtautó — pre-sale preparation and photos](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-keszitsd-fel-eladova-valt-autodat-a-meghirdetesre/) | Advises clear disclosure of known faults and photographs of vehicle details and damage | General recommendations, not a verification of an actual UI control |
| [M1: mobile.de — write a good listing](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776) | A complete equipment list, photographs, informative description, service/repair/accident history and known defects | Seller guide with illustrative screenshots; live editable form untested |
| [M2: mobile.de — selling guide](https://www.mobile.de/sicherheit/guide-and-tips/sicher-verkaufen) | Key pricing factors, extras/equipment and advice to disclose vehicle imperfections | Published advice; current selling-flow interface not individually tested |
| [A1: WCAG 2.2](https://www.w3.org/TR/WCAG22/) | Normative accessibility success criteria for testing | Standard; does not establish either competitor violates it |

## 2. Confirmed Competitor Features (Source-Based)

### Használtautó.hu (Hungary)

1. **Structured vehicle data:** The official guide describes fields such as model, year and variant; some suggested values are auto-filled and remain editable. **Implication:** Advanced vehicle data can be easier with informed suggestions, but sellers must be able to correct incorrect predictions. [H1](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/)
2. **Equipment selection:** Its official advice explicitly describes selecting extras using checkboxes (e.g. ABS, central locking). Chosen equipment appears on the vehicle page rather than requiring repetition in free-text description. **Implication:** Dedicated feature selection is a reasonable AutoPiac content model. [H2](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-hirdess-a-hasznaltauto-hu-n-a-sikeres-jarmuhirdetes-titka-5-percben/)
3. **Photo workflow:** Upload and subsequent image management (ordering/captions) are distinct described stages; the guide describes optional document photos. **Implication:** AutoPiac can show upload status, cover and ordering in one comprehensible stage (proposed simplification, not proof of superiority). [H1](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/)
4. **Package selection:** The published listing guide describes packages and promotions after image management, some affecting photo visibility. **Implication:** AutoPiac should clearly separate core listing publication from optional premium purchase and disclose terms before payment. [H1](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/)
5. **Honest vehicle history:** The official preparation article encourages declaring known defects and photographing any damage. **Implication:** A structured damage/replaced-parts section can support transparent condition reporting. [H3](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-keszitsd-fel-eladova-valt-autodat-a-meghirdetesre/)

### mobile.de (Germany)

1. **Listing completeness:** The official seller article identifies three major content pillars: high-quality photos, a fully completed equipment list and informative descriptive text. **Implication:** AutoPiac's initial four-item sample equipment list was too shallow as a product concept. [M1](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776)
2. **Distinguishing structured extras from description:** mobile.de suggests that free-text description supplement rather than merely repeat extras, emphasizing actual condition and history. **Implication:** Separate equipment/features, damage/repair disclosure, and narrative description. [M1](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776)
3. **History and damage:** Advice explicitly mentions servicing, repairs, resprays, accidents, outstanding defects and replaced components. **Implication:** A panel-status/repair-history form has a real information-value rationale independent of user research. [M1](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776)
4. **Pricing inputs:** The sales guide identifies year, mileage, condition and additional equipment among pricing factors. **Implication:** Keep those fields discoverable and consistent on Review. [M2](https://www.mobile.de/sicherheit/guide-and-tips/sicher-verkaufen)

## 3. Side-by-Side Comparison

| Dimension | Használtautó.hu | mobile.de | AutoPiac UX decision |
| --- | --- | --- | --- |
| Vehicle identification | Structured form with some editable auto-population (H1) | Listing guide emphasizes make/model/year/trim (M1) | Begin with essentials; advanced taxonomy when necessary |
| Equipment / extras | Checkbox module described (H2) | Complete equipment list emphasized (M1) | Grouped equipment checklist (Safety, Comfort, Technology, Exterior), potential search and “Other” |
| Damage and history | Known defects should be disclosed (H3) | Known/repaired damage, repairs and history emphasized (M1) | Separate body-panel status and optional notes |
| Photo management | Upload plus separate order/captions stages described (H1) | Clear, informative photographs emphasized (M1) | One photo step with counter, cover choice and visible gallery |
| Description | Contextual vehicle history/details (H2) | Narrative to supplement equipment and describe history (M1) | Prompt for repair/service/ownership details without duplicating feature list |
| Commercial choices | Packages/promotions after listing stages (H1) | Paid-package considerations in selling guide (M2) | Keep premium visibly optional, clarify benefits |
| Directly tested task completion | Not measured | Not measured | Only owner-reported AutoPiac Figma navigation results, not live form-completion data |

## 4. Eight Heuristic Review Items (Potential Risks, NOT Verified Defects)

The following are **potential risk scenarios** informed by features described in the official sources. No statement in this table establishes that the competitors fail a heuristic or accessibility criterion.

| ID | Source-backed observation | Potential risk to evaluate | Proposed AutoPiac response | Proposed validation |
| --- | --- | --- | --- | --- |
| UX-01 | Használtautó auto-suggests some specifications (H1) | Users might accept a wrong auto-filled field | Editable suggestion + explicit confirmation | Seed incorrect suggestion in a task |
| UX-02 | Equipment selection is detailed (H2 / M1) | Long, flat option lists may hinder discovery | 4 named groups + searchable optional extras | Ask user to find 3 specific options |
| UX-03 | Image upload and management occur in separate described stages (H1) | Cover/ordering could be overlooked | Inline cover and reorder controls | Cover-photo task with observation |
| UX-04 | Packages are offered before finalization (H1) | Premium choice could be confused with mandatory payment | “Optional premium” label and pricing clarity | Ask participant what is required to publish |
| UX-05 | Damage/repair history matters (H3 / M1) | Free-form-only notes may omit key parts | Body-panel status selection and optional repair details | Ask participant to disclose a replaced panel |
| UX-06 | Vehicle forms use technical terms (H1 / M1) | A first-time seller may not recognize version/trim or features | Plain-language help, “Not sure” state | Terminology comprehension test |
| A11Y-01 | Forms may include required selections and errors | **If** labels/errors are not programmatically associated, screen-reader users could miss them | Persistent labels, accessible error summary and \`aria-describedby\` in real implementation | Keyboard + screen reader; WCAG 2.4.6 / 3.3.1 / 3.3.2 |
| A11Y-02 | Photo ordering can be implemented by drag interaction (H1) | **If** dragging is the only method, keyboard/pointer accessibility can suffer | Move earlier/later buttons plus drag alternative, suitably sized targets | Keyboard-only and touch; WCAG 2.1.1 / 2.5.7 / 2.5.8 |

## 5. Research Triangulation and Prioritization

**Actual independent research signal:** One owner-reported interview of R01 (18-year-old first-time prospective seller) explicitly requested more equipment options and a place for damage/replaced parts. The initial revised mockup was then liked but the equipment list still judged insufficiently developed. The follow-up impression is **real reported feedback**, not a timed/independent full-task test. See [Interview R01](../../project/docs/interview-r01.md).

**Source convergence:** The participant's requests align with seller information needs documented by Használtautó.hu (checkbox equipment and defect transparency) and mobile.de (complete equipment list and detailed history). This supports design **priority**, not a measured claim that AutoPiac is faster or easier.

### Prioritized Changes
1. **P0 — Grouped equipment selection:** Safety & Driver Assistance / Comfort & Interior / Infotainment & Connectivity / Exterior & Lighting; show representative options, selected counts, and an option for unspecified extras.
2. **P0 — Condition transparency:** Keep Original/Repainted/Replaced/Damaged/Unknown as explainable selections; do not treat a default example as a verified vehicle fact.
3. **P1 — Photo-stage completeness:** Visible 5-photo minimum and cover control; future accessible reordering.
4. **P1 — Optional commercial add-on clarity:** Plan premium decision as optional and clear before the publish step.
5. **P2 — Advanced suggestions:** Make/model/year-based prefill after vehicle catalog integration and real testing.

## 6. Evidence / Scope and Submission Limitations

- [x] Two source-backed competitor/platform reviews with primary citations.
- [x] Six UX observation/risk cases plus two conditional accessibility risks.
- [x] Side-by-side feature matrix and specific AutoPiac responses.
- [x] Detailed evaluation methodology, assumptions, and sourced design implications.
- [ ] Full hands-on inspection of current logged-in listing editors with annotated screenshots.
- [ ] Verified actual competitor accessibility issues (none claimed).
- [ ] Comparative participant task time or conversion results (none claimed).

**Research ethics:** Never present a hypothetical risk as an observed defect, and never fabricate participant quotes or accessibility failures.
