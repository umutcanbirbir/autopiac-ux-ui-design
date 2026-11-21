# Homework 06 — Low-Fidelity Wireframes

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Status:** Initial editable wireframes created in Figma on 2026-11-21; detailed QA pending.
**Figma file:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC

## Scope
Design the seller's primary listing task with 5–6 connected grayscale wireframes. Keep visual decoration minimal; emphasize structure, hierarchy, form requirements, and screen states.

## Screen Inventory
| Screen | Primary UI | Main action |
| --- | --- | --- |
| 01 — Start | Short requirements summary, "Create listing" button, progress overview | Begin |
| 02 — Vehicle Details | Make/model/year/version, mileage, fuel, condition, inline guidance | Continue |
| 03 — Photos | Upload area, visible count (minimum 5), reorder/remove controls | Continue |
| 04 — Price & Description | Price, currency, condition notes, description | Continue |
| 05 — Review | Summary of all sections, edit links, clear validation feedback | Publish |
| 06 — Success | Publication confirmation, listing reference placeholder, next steps | View listing |

## Critical States
- **Insufficient photos:** User attempts to continue with fewer than five images; message explains the minimum and focuses the upload control.
- **Invalid vehicle data:** One or more required details are missing; error summary and field-level cues allow correction.
- **Submission failure (optional additional state):** Draft remains available, and Retry is offered.

## Responsive Design
Create one primary screen for mobile (e.g., 390 px content width) and a larger screen (e.g., 1280 px frame). Mobile gets a single-column form, desktop can use a content column plus a clear progress or help panel.

## Required Figma Techniques
- Auto Layout for major structures and form rows.
- Reusable simple controls where practical.
- Content hierarchy and readable labels.
- Navigation connected in the subsequent prototype stage.

## Completion Checklist
- [x] Low-fidelity Figma file linked here.
- [x] Seven mobile wireframe states and one desktop variant created.
- [x] Two critical states created: insufficient photos and missing required vehicle data (static frame states).
- [x] Mobile and larger-screen layout for vehicle details.
- [x] Auto Layout used across primary structures; final visual QA pending.
