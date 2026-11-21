# Homework 05 — Information Architecture & User Flow

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Proposed architecture; terminology testing pending.

## Content Inventory
| Group | Information |
| --- | --- |
| Account | Login state; private seller identity |
| Vehicle | Make, model, production year, version, body type, mileage, fuel, transmission |
| Condition | Vehicle state, service history, known defects, optional equipment |
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

## Label Validation Plan
Ask **three actual participants** how they interpret terms such as "Vehicle Details", "Equipment", "Review", "Publish", and "Draft". Record the date, task, and anonymized observations.

| Participant | Tested? | Confusing labels | Suggested revisions |
| --- | --- | --- | --- |
| T01 | No | — | — |
| T02 | No | — | — |
| T03 | No | — | — |

The table is a testing plan and **does not report results**.
