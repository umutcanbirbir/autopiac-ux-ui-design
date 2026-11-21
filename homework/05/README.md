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

[FigJam user flow](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB) · [Current Figma prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2)

## Error States

1. **Missing vehicle information:** Show the field that needs attention.
2. **Not enough photos:** Explain that five photos are required and provide a way back.
3. **Submission error:** In a functional product, keep the draft and offer a retry action.

The current Figma prototype illustrates the first two error cases. The third is a future implementation scenario.

## Update After User Feedback

The initial flow did not include equipment or body condition as a dedicated step. After the first interview, I added [Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2) between Vehicle Details and Photos, without changing the main four-stage structure.

The project also has a planned limit of one active listing per private seller, including drafts. A future design should explain that limit if someone tries to create a second one.

## Terminology Test

I plan to ask three additional people to explain these labels in their own words: **Vehicle Details, Equipment, Review, Publish and Draft**. I will note any confusing terms and update the design if necessary.

| Participant | Terms understood | Unclear terms | Suggested change |
| --- | --- | --- | --- |
| T01 | Not tested yet | — | — |
| T02 | Not tested yet | — | — |
| T03 | Not tested yet | — | — |

[Test questions and recording template](../../project/docs/usability-test-instructions.md)
