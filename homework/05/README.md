# Homework 05 — Information Architecture and User Flow

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)

## Information Architecture

I organized the seller journey around the information needed to create one complete vehicle listing.

| Section | Content |
| --- | --- |
| Account | Sign-in and private seller |
| Vehicle Details | Make, model, year, mileage and other specifications |
| Equipment & Condition | Feature choices, damaged/repainted/replaced panels and repair notes |
| Photos | Required images, cover photo and order |
| Price & Description | Listing title, asking price and description |
| Review | Summary of the information and links to edit each section |
| Completion | Confirmation that the prototype flow has ended |

## Sitemap

The sitemap is placed directly in the existing [AutoPiac FigJam board — Homework 05](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2011-299), next to the user-flow diagram, which now includes Equipment & Condition. The page hierarchy is also listed below.

```text
AutoPiac
├── Home
├── My Listings
│   ├── Drafts
│   └── Published Listings
└── Create Listing
    ├── Vehicle Details
    ├── Equipment & Condition
    ├── Vehicle Photos
    ├── Price & Description
    ├── Review Listing
    └── Completion
```

## Main User Flow

The [same FigJam board](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2011-299) presents the main listing journey as a readable connected flow, with missing fields, insufficient photos, Review edits and planned submission retry grouped below as separate recovery notes. **Equipment & Condition** remains between vehicle details and photos, matching the clickable Figma prototype.

```text
Start a listing
    ↓
Sign in if needed
    ↓
Enter vehicle details
    ↓
Choose equipment and describe condition
    ↓
Add at least five photos
    ↓
Enter price and description
    ↓
Review information
    ├── Need to change something → Open that section → Review again
    └── Everything looks correct → Finish
```

[FigJam — compact Sitemap beside User Flow](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2011-299) · [Current Figma prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2)

## Error States

1. **Missing vehicle information:** Show the field that needs attention.
2. **Not enough photos:** Explain that five photos are required and provide a way back.
3. **Submission error:** In a functional product, keep the draft and offer a retry action.

The current Figma prototype illustrates the first two error cases. The third is a future implementation scenario.

## Update After User Feedback

The initial flow did not include equipment or body condition as a dedicated step. After the first interview, I added [Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) between Vehicle Details and Photos, without changing the main four-stage structure.

The project also has a planned limit of one active listing per private seller, including drafts. A future design should explain that limit if someone tries to create a second one.

## Terminology Feedback — Individual Confirmation

All three participants (T01, T02, T03) independently completed the assigned Figma tasks and correctly understood the screen terms in Turkish, according to the student's **23 November 2026 clarification**. The following Turkish interpretations were recorded across the group: **Vehicle Details → araç detayları; Equipment → donanım; Review → incele; Publish → yayınla; Draft → kaydet**.

| Participant | Understanding | Exact response transcript | Design note |
| --- | --- | --- | --- |
| **T01** | Student confirmed all five term meanings were understood correctly in Turkish | Not retained individually | First encountered broken controls/Continue navigation, then finished after the fix |
| **T02** | Student confirmed all five term meanings were understood correctly in Turkish | Not retained individually | Completed on corrected prototype |
| **T03** | Student confirmed all five term meanings were understood correctly in Turkish | Not retained individually | Completed on corrected prototype |

These were direct Turkish translations or interpretations. **Draft → kaydet** expresses saving, but may not explicitly convey the meaning *saved without publishing*. “Save as draft” remains a possible clarity improvement, not a demonstrated failure. We cannot quote each participant's exact individual wording because separate verbatim transcripts were not recorded.

All three completed the assigned tasks and reached the final screen independently; the approximate reported times were **T01 ~4 minutes** (included encountering and recovering from the prototype defects), **T02 ~1 minute** and **T03 ~1 minute** on the corrected version. These are student-reported estimates, not stopwatch measurements. The same three participants must not be assumed to be additional unique users beyond the earlier navigation walkthrough.

[Participant-level results in Homework 08](../08/README.md) · [Detailed follow-up feedback](../../project/docs/prototype-test-feedback-2026-11-21.md) · [Task guide](../../project/docs/usability-test-instructions.md)
