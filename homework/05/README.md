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

The sitemap is now drawn directly in the existing [AutoPiac FigJam board — Homework 05](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2007-200), alongside the latest seller user flow. The page hierarchy is shown below as a text reference.

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

The same [Homework 05 FigJam section](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2007-200) also contains the updated visual flow with **Equipment & Condition** between Vehicle Details and Photos, as well as the missing-field, photo-count and review-edit notes.

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

[Sitemap and revised user flow — FigJam](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2007-200) · [Current Figma prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2)

## Error States

1. **Missing vehicle information:** Show the field that needs attention.
2. **Not enough photos:** Explain that five photos are required and provide a way back.
3. **Submission error:** In a functional product, keep the draft and offer a retry action.

The current Figma prototype illustrates the first two error cases. The third is a future implementation scenario.

## Update After User Feedback

The initial flow did not include equipment or body condition as a dedicated step. After the first interview, I added [Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) between Vehicle Details and Photos, without changing the main four-stage structure.

The project also has a planned limit of one active listing per private seller, including drafts. A future design should explain that limit if someone tries to create a second one.

## Terminology Feedback

In a later discussion of the revised prototype, participants gave the following Turkish interpretations: **Vehicle Details → araç detayları, Equipment → donanım, Review → incele, Publish → yayınla, Draft → kaydet**. Most terms matched their intended meanings. **Draft** was associated with saving, but did not clearly express that the listing remains unpublished; “Save as draft” may be easier to understand. The number of participants and individual responses in this feedback were not recorded, so these results are not assigned to T01–T03.

[Follow-up feedback and navigation issue](https://github.com/umutcanbirbir/autopiac-ux-ui-design/blob/main/project/docs/prototype-test-feedback-2026-11-21.md). I still plan to record individual responses from three participants in a structured terminology test.

| Participant | Terms understood | Unclear terms | Suggested change |
| --- | --- | --- | --- |
| T01 | Not tested yet | — | — |
| T02 | Not tested yet | — | — |
| T03 | Not tested yet | — | — |

[Test questions and recording template](../../project/docs/usability-test-instructions.md)
