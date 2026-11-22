# AutoPiac — Final Presentation Speaking Notes

**Student:** Umut Can Birbir (DUJ3ZD)
**Course:** UX/UI Design — University of Pécs
**Duration:** Approximately 8–9 minutes, plus an optional live Figma demonstration.

These notes are written in simple spoken English. The ninth PowerPoint slide contains clickable project links for questions and references.

## Slide 1: AutoPiac — Introduction

**Target time: 45 seconds**
Hello, my name is Umut Can Birbir. This is AutoPiac, my UX/UI semester project.
AutoPiac is a car marketplace concept for Hungary. I focused on one important journey: how a private seller creates a car listing.
My goal was to make the process clear and easy to follow, without leaving out important information. I will show my research, design, prototype and user feedback.

## Slide 2: The challenge

**Target time: 55 seconds**
My starting hypothesis was that long forms and unclear vehicle requirements may make car listing difficult. This was a hypothesis, not a proven fact.
I focused on private sellers in Hungary, especially people with little experience.
I did not design the whole marketplace. I focused on one journey, from starting an advertisement to checking and completing it.
I wanted to keep the steps simple, show what is required, and let sellers correct mistakes.

## Slide 3: What the first user taught me

**Target time: 65 seconds**
For my first research session, I talked with an 18-year-old who had never posted a car advertisement. He is my brother, so I know this is a small convenience sample.
He moved through the prototype without help and understood the labels. He liked the simple layout.
But he noticed two missing things: vehicle equipment and repair history. This changed my design direction.
I decided to keep the clean flow, but add a separate equipment and condition step. This is a useful example of how real feedback changed the first idea.

## Slide 4: Competitor research

**Target time: 60 seconds**
I compared Használtautó.hu in Hungary and mobile.de in Germany. I used official selling guides and selected public user comments. I did not test the full logged-in seller forms.
Használtautó.hu offers structured information, photo features and an announced price assessment. mobile.de strongly recommends detailed equipment and repair information.
Some public comments also raise concerns about incorrect vehicle options or unclear paid photo features. These are user reports, not confirmed bugs.
For AutoPiac, my main lessons were: keep data editable, explain photo limits, and separate equipment from repair history.

## Slide 5: Information architecture and user flow

**Target time: 65 seconds**
I organized the information before making the final screens.
The sitemap separates Home, My Listings and Create Listing. The main design is the Create Listing journey.
Instead of one long form, the seller moves through vehicle details, equipment and condition, photos, price and description, and Review. Finally, the prototype shows completion.
There are also example error states. A seller can see if required fields or photographs are missing, and the Review screen links back to sections for editing.
This structure helped me keep the journey clear, even when more information was added.

## Slide 6: Clickable Figma prototype

**Target time: 90 seconds, including a short live demonstration**
These are the main parts of my Figma design.
The first screen shows required vehicle information. The second screen has four equipment groups with 16 selectable features, and five condition states for one example body panel. The next stage explains that at least five photos are needed.
Users can scroll, select equipment, change the fender condition, go forward and go back. Review also has links to edit sections.
I will briefly open the live Figma prototype to show these interactions. This is not a working car marketplace: text fields and real publishing are not connected to a database.

## Slide 7: Testing and iteration

**Target time: 95 seconds**
I started with three navigation walkthroughs. All three people reached the last Figma screen, but this was only a screen navigation test. They did not create real listings.
Later, three people tested the latest interactive version. They reported no remaining problems and described the interface as simple and easy to use. I do not have individual task times or full task records, and I do not know whether the two test groups overlap.
The feedback helped me fix three important problems. First, the equipment screen was too long and could not scroll. Second, equipment could not be changed. Third, the damage choice was static.
I added scrolling and interactive component states, and tested the updated prototype again.

## Slide 8: Accessibility and reflection

**Target time: 60 seconds**
I also checked the visual design for accessibility. I inspected ten Figma screens and improved nine low-contrast input borders. Their contrast against white increased from about 1.54 to 3.80 to one. I also enlarged some equipment and damage labels.
This is only a visual design review. I have not certified keyboard or screen-reader accessibility.
My main lesson is that a simple interface should not leave out important information. Real feedback showed me how to keep the process clean while adding equipment and vehicle history.
Next I would build real form inputs, extend the body-panel tool, and test keyboard access and screen readers. Thank you.

## Presentation links

- **Figma prototype:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2
- **FigJam:** https://www.figma.com/board/FReaY560jfsj9gfCeta8oB
- **GitHub project:** https://github.com/umutcanbirbir/autopiac-ux-ui-design

**Evidence limitation:** Three people gave positive feedback about the latest interactive prototype, but their individual task timings and form-entry outcomes were not recorded. The deck does not claim actual advertisement publication or verified WCAG conformance.