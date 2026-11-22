# AutoPiac — UX/UI Design Semester Project

**Student:** Umut Can Birbir (DUJ3ZD)  
**University:** University of Pécs (PTE MIK)  
**Course:** UX/UI Design

## About the Project

AutoPiac is my car marketplace project. For the UX/UI course, I focused on one specific journey: helping a private seller create a clear, complete vehicle advertisement. The design covers vehicle details, equipment, damage history, photos, pricing, review and confirmation.

My aim is to keep the main process simple without leaving out important information that buyers need.

## Project Files

| Deliverable | Link |
| --- | --- |
| Current clickable prototype | [Figma — AutoPiac](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2) |
| Research, user flow and idea prioritization | [FigJam board](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB) |
| Homework 01–10 | [Homework folders](homework/) |
| Tasks and progress | [GitHub Projects](https://github.com/users/umutcanbirbir/projects/1/views/1) · [Kanban task overview](project/KANBAN.md) · [GitHub Issues](https://github.com/umutcanbirbir/autopiac-ux-ui-design/issues) |
| Detailed project notes | [Project overview](project/README.md) |
| Presentation preparation | [Presentation folder](presentation/01-01/) |

The [AutoPiac GitHub Projects Board](https://github.com/users/umutcanbirbir/projects/1/views/1) has been configured with the existing eight issues in Todo, In Progress and Done. The [repository Kanban](project/KANBAN.md) is a written overview.

## Design Process

**1. Define the problem.** I chose the private seller's listing journey rather than attempting to design the whole marketplace. The initial problem, goals and assumptions are documented in [Homework 01](homework/01/README.md).

**2. Research and compare.** I discussed the prototype with my 18-year-old brother, who had never posted a car listing before. He liked the simple layout but wanted equipment selection and a dedicated area for damaged or replaced parts. After seeing the first revision, he suggested developing the equipment list further. I also compared publicly available seller guides from Használtautó.hu and mobile.de. See [Homework 02](homework/02/README.md) and [Homework 03](homework/03/README.md).

**3. Plan the flow.** I organized the required information into steps, mapped possible errors and prioritized ideas in FigJam. The [Homework 05 sitemap](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2011-299) sits beside the updated user-flow diagram, including Equipment & Condition, on the same FigJam board. See [Homework 04](homework/04/README.md) and [Homework 05](homework/05/README.md).

**4. Design and prototype.** The Figma file contains the initial grayscale wireframes, a yellow-and-white visual direction and subsequent improved screens. The latest mobile flow goes from vehicle details through equipment/condition, photos, price, review and completion. A desktop vehicle-details example is also included. See [Homework 06](homework/06/README.md) and [Homework 07](homework/07/README.md).

**5. Test and improve.** In an initial walkthrough, three participants reached the end of the clickable screen flow and the interface was generally liked for its simplicity. Because the Figma fields were static, this tested navigation rather than actual listing entry. Later feedback led to four equipment categories with 16 example choices and clearer damage information. Results and changes are documented in [Homework 08](homework/08/README.md) and [Homework 09](homework/09/README.md).

## Visual Design and Components

The interface uses yellow (`#FFD400`), white and dark text. The Figma file also includes button, input, alert and photo-tile components with 15 variants in total, plus a developer handoff reference.

- [Equipment & Condition screen](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2007-2)
- [Component library](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2004-2)
- [Color guideline](project/docs/color-guideline.md)
- [Design review and corrections](project/docs/design-qa-2026-11-21.md)

## Prototype Scope and Remaining Work

Figma demonstrates the intended screens and navigation. The latest Equipment & Condition screen now contains **16 independently toggleable equipment checkboxes** using interactive component variants. The earlier nonfunctional search visual was removed. The front-left fender's five damage statuses are now a separate interactive single-selection component. Text fields, photo tiles and the other vehicle panels are not functional. Prototype selections are not saved or automatically reflected on Review. A separate [HTML interaction demo](docs/index.html) supports some form entry and local photo selection but is not a published marketplace.

The next steps are to collect feedback from three additional users on the revised design, record any terminology or equipment-discovery problems, complete outstanding accessibility checks, and prepare the final presentation. Refer to the [Kanban](project/KANBAN.md) for the current task list.
