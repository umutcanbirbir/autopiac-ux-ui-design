# Homework 09 — Design Iterations, Components and Handoff

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Design file:** [AutoPiac Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC)  
**Color guideline:** [Yellow and White](../../project/docs/color-guideline.md)

## Design Iterations

After preparing the first clickable prototype, I worked on three areas: required information, photo guidance and reviewing a listing. The purpose was to make the flow clearer while keeping the layout simple.

| Change | Earlier design | Revised design |
| --- | --- | --- |
| **01 — Required fields** | Basic form fields with little guidance | Visible required-field explanations and a separate missing-field example |
| **02 — Photos** | Photo count and a basic upload concept | Five example thumbnails, cover-photo label, photo count, recommended angles and missing-photo example |
| **03 — Review** | Simple summary and a generic Back action | Linked sections for returning to vehicle details, photos, price and description |

### Compare the Screens

| Screen | Before | After |
| --- | --- | --- |
| Vehicle details | [Earlier](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-20) | [Revised](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-25) |
| Photos | [Earlier](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-50) | [Revised](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-62) |
| Review | [Earlier](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-93) | [Revised](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-115) |
| Completion | [Earlier](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=9-116) | [Revised](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-143) |

The first three revisions were based on design review and the limitations of the initial prototype, not on specific complaints from the three-person navigation test. I kept the earlier frames in the file so the changes can be compared.

## Improvements Based on Interview Feedback

My interview with a first-time prospective seller identified two missing areas:

- **Vehicle equipment:** Sellers should be able to indicate a car's features.
- **Damage and repairs:** Sellers should have a clear place to report repainted, replaced or damaged panels.

I added a separate [Equipment & Condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) between Vehicle Details and Photos. The Review screen links back to this section.

When I showed the first version to the same participant, he liked it but wanted a more complete equipment list. I expanded the sample from four choices to **16 choices in four groups**:

- Safety & Driver Assistance
- Comfort & Interior
- Infotainment & Connectivity
- Exterior & Parking

An informal follow-up on the expanded screen found that participants could read the equipment categories, but could not change the visual selections or reach the next-step button. The exact participant count and individual outcomes are not available. See [Homework 02](../02/README.md), [first follow-up](../../project/docs/r01-follow-up-2026-11-21.md), and [later prototype feedback](https://github.com/umutcanbirbir/autopiac-ux-ui-design/blob/main/project/docs/prototype-test-feedback-2026-11-21.md).

## Iteration 05 — Fixing the Long-Screen Navigation Blocker

**Issue found:** In the expanded Equipment & Condition prototype, the **Continue to photos** button appeared below the visible screen and could not be reached. The original Figma frame was 1360 px tall with scrolling disabled.

**Correction:** I changed the frame to a fixed **390 × 844 px** mobile viewport with **vertical scrolling**, so the damage section and continuation button can be reached by scrolling. Its links to Photos and Vehicle Details remain intact.

**Status:** The Figma correction was applied and visually checked. Follow-up feedback then confirmed the revised navigation works and no further problem was reported. Individual participants and exact test times were not recorded. At this stage, equipment checkboxes still displayed noneditable example states.

[Revised Equipment & Condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) · [Observed feedback](https://github.com/umutcanbirbir/autopiac-ux-ui-design/blob/main/project/docs/prototype-test-feedback-2026-11-21.md).

## Iteration 06 — Clickable Equipment Selections

After the scrolling issue was resolved, I addressed the remaining complaint that the equipment choices could not be changed. I created an [AutoPiac Equipment Toggle component](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2040-9) with **two variants (Selected=On / Selected=Off)** and two-way **On Click → Change To** prototype reactions. All **16 items** were replaced with independent instances of this component; the equipment label is a text property that remains unchanged when its selection state changes. The starting selection states were preserved.

I also removed the visual search field, which could not accept typing, and added the instruction **“Tap a feature to select or deselect it.”**

**Checked:** All 16 Figma instances now reference the two-state component. The bidirectional reactions and a test switch of the Apple CarPlay variant were checked in the file, including preservation of its label. The scrolling frame and Continue / Back navigation remain in place. **A subsequent student-relayed retest reported that the choices worked in Figma Present mode.** The exact participants and individual options tested were not recorded.

**Scope:** Figma maintains visual checkbox state during component interaction; it does not write to a database, compute a live selected count, or automatically update the Review page.

[Interactive equipment screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) · [Toggle component](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2040-9).

## Iteration 07 — Interactive Body Panel Condition

A follow-up pointed out that the **damage-status choices still could not be changed** after the equipment checkboxes became interactive. I built a [Body Panel Condition component](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2044-34) with five mutually exclusive variants: **Original, Repainted, Replaced, Damaged and Unknown**.

Each variant has clickable alternatives that change the whole control to the selected status. The panel heading and **Selected: ...** label update with the choice. I added this component to the existing *Front-left fender* section, replacing the earlier static status chips.

**Checked in Figma:** 20 valid between-state click reactions; all five variants display exactly one selected option and the correct label. The initial state is **Replaced**. The 390 × 844 px vertically scrolling viewport and Continue to Photos action remain unchanged.

**Follow-up check:** The student reported that the updated damage-status controls work in Present mode, and the design was described as simple and practical. Individual participant results and timings were not recorded. The current screen demonstrates **one body panel**; a complete interactive condition diagram covering all vehicle panels would require further work. Selected values are not stored as listing data or transferred to Review.

[Body panel component](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2044-34) · [Updated equipment & condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2).

## Follow-Up Test Summary — Three Participants, Different Prototype States

The student clarified the individual test results on 23 November 2026. **T01** independently worked through the flow but found the controls and Continue button did not work; they completed the assigned tasks and reached the final screen after prototype fixes (**approximately four minutes across the problem and correction/retest process**). **T02** and **T03** independently completed the assigned tasks on the corrected version, **approximately one minute each**, with no remaining control issues reported.

All three understood the displayed interface terms in Turkish, and the design was generally described as simple and practical. The time estimates were not measured with a stopwatch. We cannot compare T01 directly to T02/T03 because their prototype conditions were different, or infer that all three tested every interactive variant. We also do not know if these three overlap with the earlier navigation test group.

[Individual outcomes and evidence limitations](../../homework/08/README.md) · [Follow-up details](../../project/docs/prototype-test-feedback-2026-11-21.md)


## Mini Design System

I prepared four component groups in Figma with **15 variants**:

| Component | Variants | Link |
| --- | --- | --- |
| Button | Primary, Secondary, Disabled, Focused | [Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-2) |
| Input | Default, Filled, Focused, Error | [Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-11) |
| Alert | Info, Error, Success | [Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-20) |
| Photo Tile | Empty, Filled, Cover, Error | [Figma](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-30) |

The visual language uses yellow `#FFD400`, white `#FFFFFF`, pale yellow `#FFF7D8`, dark text `#1F1F1F`, Inter type and consistent spacing. These components are defined as Figma variants; the screens have not all been rebuilt from component instances.

## Developer Handoff and Quality Check

The [handoff panel](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55) explains mobile/desktop dimensions, field requirements, validation, photo limits and basic accessibility expectations.

I also reviewed the latest screens and corrected issues with back navigation, photo previews, error-message spacing, desktop balance and button proportions. The details are recorded in the [design QA notes](../../project/docs/design-qa-2026-11-21.md).

## Accessibility and Readability Follow-Up — 22 November 2026

I checked ten Figma screens using a design-level [WCAG 2.2 AA review](../../project/docs/accessibility-review-2026-11-22.md). Nine essential input/textarea borders originally had only **1.54:1** contrast against white; I changed them to **#8A8275**, around **3.80:1**. I increased the shared interactive equipment labels from **10 to 13 px**, the body-condition status labels from **10 to 12 px**, and small photo captions from **9 to 11 px**. A structural spot check found **44 prototype action targets** with a minimum bounding dimension of **36 px**. An approximate comparison of **204 text layers** with nearest solid ancestor backgrounds did not flag text below WCAG AA text-contrast thresholds.

The [Figma handoff](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55) now emphasizes semantic checkboxes/radio groups, keyboard access and announced state changes for implementation. The static mockup cannot establish complete WCAG compliance, since keyboard interaction, screen readers, zoom/reflow and actual browser input errors remain untested.

## What Remains to Be Tested

The scrolling blocker has been reported resolved. The interactive equipment toggles have received positive reported feedback. The front-left fender interaction has received positive informal follow-up feedback. The student reported that all three completed the assigned Figma tasks, but detailed action-by-action logs of error-state comprehension and Review editing were not retained. Figma demonstrates how the screens connect but does not save field values or support real photo uploads. A separate interaction demo can be used if a real form-entry test is needed.

[Next testing instructions](../../project/docs/usability-test-instructions.md)
