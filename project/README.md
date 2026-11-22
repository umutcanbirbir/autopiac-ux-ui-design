# AutoPiac — Project Overview

**Student:** Umut Can Birbir (DUJ3ZD)  
**University:** University of Pécs (PTE MIK)  
**Course:** UX/UI Design

## Project Idea

AutoPiac is a marketplace concept for selling used vehicles in Hungary. For this course I concentrated on the private seller's listing journey rather than the whole marketplace.

The main design question was: **How can I make a detailed car-listing process feel simple, especially for someone posting for the first time?**

## Scope

The listing flow includes:

1. Starting a listing and entering vehicle details.
2. Choosing equipment and reporting body condition or replaced parts.
3. Adding vehicle photos and choosing a cover image.
4. Entering price and description.
5. Reviewing information, making corrections and finishing.

The design includes mobile screens and a desktop vehicle-details example. Some important business rules are a minimum of five photos, up to 30 standard photos or 55 premium photos, and one active private-seller listing including drafts.

## Research and Competitor Review

I spoke with my 18-year-old brother, who had not previously posted a car listing. He found the prototype straightforward but noticed the missing equipment and damage sections. After reviewing the first new version, he suggested a more developed equipment list.

I also reviewed published selling guides from Használtautó.hu and mobile.de. Their advice supports presenting equipment, repair history and photos clearly.

- [Interview, persona and user journey](../homework/02/README.md)
- [Competitor comparison](../homework/03/README.md)
- [Research notes](docs/interview-r01.md)

## From Idea to Prototype

The [FigJam board](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB) contains the initial problem, interview themes and impact/feasibility matrix. The [Homework 05 sitemap](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2011-299) is integrated beside the updated FigJam user-flow diagram, which includes Equipment & Condition. Both match the current Figma prototype.

The [Figma file](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC) contains the grayscale wireframes, the yellow-and-white visual direction and the revised prototype. The latest design includes a grouped equipment checklist, condition statuses, photo thumbnails, review/edit links and two example validation states.

- [Start the revised prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2)
- [Equipment & Condition](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2)
- [Component variants](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-2)
- [Developer handoff](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-55)

## User Testing

Three participants tried the initial clickable screen flow. All three reached the final screen, and the general feedback was positive about the interface's simplicity. These were navigation walkthroughs: the Figma inputs were not editable, and individual task times were not recorded.

The later interview and follow-up helped me identify missing vehicle details and expand the equipment sample. After further feedback that the original checkboxes could not be changed, I implemented 16 individual **checked/unchecked interactive component instances**. The updated interactions received positive follow-up feedback from three testers, all of whom reported no remaining problems and liked the simple, usable design. These are qualitative reports, not individually timed tasks; selections are not saved as real listing data.

- [Initial navigation test](../homework/08/README.md)
- [Design iterations](../homework/09/README.md)
- [Additional test instructions](docs/usability-test-instructions.md)

## Homework Progress

| Homework | Main output | Status |
| --- | --- | --- |
| 01 | Problem definition | Draft completed |
| 02 | Interview, persona and journey | First interview documented |
| 03 | Competitor comparison | Public-source research completed; live form audit outstanding |
| 04 | Ideation and prioritization | FigJam matrix completed |
| 05 | Information architecture and flow | Compact visual sitemap integrated next to existing FigJam user flow; individual terminology results outstanding |
| 06 | Wireframes | Mobile and desktop examples completed |
| 07 | Clickable prototype | Main flow and examples connected |
| 08 | Usability testing | Initial walkthrough and positive three-person updated-prototype feedback documented; individual task records not collected |
| 09 | Revisions and components | Latest Figma revisions, component interactions, handoff and qualitative retest documented |
| 10 | Final presentation | Not yet completed |

## What Is Still Open

The updated equipment/condition screen received positive feedback from three testers. The next steps are to document any individual terminology results if available, check remaining accessibility details and prepare the final presentation. The current Figma file is a clickable design demonstration, not a functioning listing application.

The [AutoPiac GitHub Projects Board](https://github.com/users/umutcanbirbir/projects/1/views/1) now displays all eight repository issues in Todo / In Progress / Done columns. The [repository task overview](KANBAN.md) and [GitHub Issues](https://github.com/umutcanbirbir/autopiac-ux-ui-design/issues) provide the detailed work list.

[Design QA notes](docs/design-qa-2026-11-21.md) · [Color guideline](docs/color-guideline.md) · [Design decision log](docs/decision-log.md)
