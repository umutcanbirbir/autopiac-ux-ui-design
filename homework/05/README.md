# Homework 05 — Information Architecture & User Flow

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Proposed architecture; one interviewed first-time user understood existing wording but requested vehicle-equipment and damage/replaced-parts sections. Three-person terminology test remains pending.

## Content Inventory
| Group | Information |
| --- | --- |
| Account | Login state; private seller identity |
| Vehicle | Make, model, production year, version, body type, mileage, fuel, transmission |
| Equipment | Vehicle features, grouped selectable options, 'Other' / 'Not sure' choices (proposed from R01) |
| Condition | Vehicle state, service history, known defects, damage/paint/replaced panel history (proposed from R01) |
| Photos | Required images, cover photo, order, captions |
| Listing | Title, price, currency, description, location and contact preferences |
| Publishing | Progress, validation results, preview, optional premium, submit confirmation |

## Proposed Sitemap
```text
AutoPiac
├── Home
├── My Listings
│   ├── Drafts
│   └── Published Listings
└── Create a Listing
    ├── Vehicle Details
    ├── Equipment & Features (proposed)
    ├── Condition / Damage & Replaced Parts (proposed)
    ├── Photos
    ├── Price and Description
    ├── Review and Fix Errors
    └── Publish Confirmation
```

## Primary Task Flow
```text
Open Create Listing
    ↓
Sign in if needed
    ↓
Enter vehicle details
    ↓
Select equipment and disclose damage/replaced parts (new proposed subsections)
    ↓
Add minimum 5 vehicle photos
    ↓
Enter listing price and description
    ↓
Review listing
    ↓
Any errors or missing fields?
    ├── Yes → Open relevant step → Correct → Review again
    └── No  → Publish → Success
```

## Three Exceptional States
1. **Missing required field:** Explain the exact field and retain previously entered data.
2. **Too few photos:** Show "At least 5 vehicle photos are required" with an actionable upload control.
3. **Submission/network error:** Preserve the draft and display an accessible retry action.

## Additional Rule to Consider
The planned AutoPiac product allows only one active private-seller listing, counting drafts and published listings. This needs a specific limit-reached UI state in later prototypes.

## R01 Interview — Content Gaps

A first-time prospective seller (R01, 18, researcher's sibling) reportedly understood the existing terminology and navigated the prototype independently. They explicitly identified missing **equipment selection** and **damage/replacement history** entry. See [research interview](../../project/docs/interview-r01.md).

These content areas have now been incorporated into a [new static Figma Equipment & Condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2), with a linked path between Vehicle Details and Photos. Actual editable choices, persistence and preferred layout have **not** been tested.

## Label Validation Plan
Ask **three actual participants** how they interpret terms such as "Vehicle Details", "Equipment", "Review", "Publish", and "Draft". Record the date, task, and anonymized observations.

| Participant | Tested? | Confusing labels | Suggested revisions |
| --- | --- | --- | --- |
| T01 | No | — | — |
| T02 | No | — | — |
| T03 | No | — | — |

The table is a testing plan and **does not report results**.
