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

These revisions have not yet been evaluated with a new group of users. See [Homework 02](../02/README.md) and the [follow-up notes](../../project/docs/r01-follow-up-2026-11-21.md).

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

## What Remains to Be Tested

The latest equipment list, error-state comprehension and Review editing paths need feedback from additional users. Figma demonstrates how the screens connect but does not save field values or support real photo uploads. A separate interaction demo can be used if a real form-entry test is needed.

[Next testing instructions](../../project/docs/usability-test-instructions.md)
