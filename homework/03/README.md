# Homework 03 — Competitor Analysis

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Research notes:** 21 November 2026  
**Competitors:** Használtautó.hu and mobile.de

## Research Goal

I compared two established vehicle marketplaces to see how they help private sellers describe their cars. I focused on vehicle information, equipment, damage history, photos and listing completion.

I used the competitors' published seller guides and examples. I did not test their logged-in advertisement editors directly, so the usability concerns below are **questions for further evaluation**, not defects I personally observed.

## Sources

- [Használtautó.hu — Step-by-step advertisement guide](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/)
- [Használtautó.hu — Advice for a good listing](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-hirdess-a-hasznaltauto-hu-n-a-sikeres-jarmuhirdetes-titka-5-percben/)
- [Használtautó.hu — Preparing a car for sale](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-keszitsd-fel-eladova-valt-autodat-a-meghirdetesre/)
- [mobile.de — Writing a good advertisement](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776)
- [mobile.de — Selling guide](https://www.mobile.de/sicherheit/guide-and-tips/sicher-verkaufen)
- [WCAG 2.2](https://www.w3.org/TR/WCAG22/) for accessibility review criteria

## What I Learned

**Használtautó.hu** explains a structured advertisement process with vehicle details, photo upload and management, and package choices. Its selling advice describes choosing equipment using checkboxes and providing complete information about the car.

**mobile.de** emphasizes a detailed equipment list, high-quality photographs, service history, previous repairs and known defects. Its advice also separates structured extras from the written description.

These points helped me identify useful content for AutoPiac. They also matched the feedback from my first-time-user interview, particularly the need for a better equipment list and damage disclosure.

## Comparison

| Area | Használtautó.hu | mobile.de | AutoPiac approach |
| --- | --- | --- | --- |
| Vehicle details | Structured vehicle fields, some editable suggestions | Make, model, year and trim information | Keep the essentials clear and add advanced details only where useful |
| Equipment | Checklist of extras | Emphasis on a complete equipment list | Four groups of selectable-looking features |
| Damage and history | Advises sellers to disclose known faults | Emphasizes repairs, accidents and condition | Separate panel status and repair notes |
| Photos | Upload, ordering and captions are described | Clear and informative images | One photo stage with count, previews and cover label |
| Description | Listing details and condition information | Text supplements equipment list | Encourage service/condition details without repeating checkboxes |
| Pricing and packages | Offers package/promotion choices | Selling guidance considers vehicle details and extras | Keep optional premium separate from required listing steps |

## UX Review — Six Questions to Evaluate

| # | Design concern | Why it matters | AutoPiac response |
| --- | --- | --- | --- |
| 1 | Could auto-filled car details be incorrect? | Sellers need to recognize and correct mistakes | Keep important fields editable |
| 2 | Can users find an item in a long equipment list? | A flat list may be difficult to scan | Group extras by Safety, Comfort, Infotainment and Exterior |
| 3 | Is choosing the cover photo obvious? | The first image represents the listing | Show visible thumbnails and a cover label |
| 4 | Could users mistake optional packages for required fees? | Pricing needs to be clear | Mark premium as optional |
| 5 | Will important repair information be missed? | Condition affects buyer trust | Provide damage statuses and repair notes |
| 6 | Are technical labels understandable for beginners? | Sellers may not know every specification | Use examples and simple explanations |

I would verify these questions by watching sellers use the relevant live forms or by testing the proposed AutoPiac improvements. The table does not mean either competitor has been proven to fail these checks.

## Accessibility Review — Two Additional Checks

| Area | What needs checking | Design response |
| --- | --- | --- |
| Forms and errors | Whether labels and validation messages can be understood by keyboard and screen-reader users (WCAG 3.3.1, 3.3.2) | Persistent labels, explanatory error text and visible focus |
| Photo ordering | Whether rearranging photos can be done without dragging alone (WCAG 2.1.1, 2.5.7, 2.5.8) | Include accessible move-up/move-down controls in a functional version |

I used WCAG as a framework for what to test. I did not run a formal accessibility audit on the competitors.

## Design Priorities

The most useful changes for AutoPiac are a clear equipment selector, structured condition reporting, a photo gallery with cover selection and straightforward review/edit navigation. This combination supports complete advertisements without making the main flow unnecessarily complicated.

I recorded the comparison in [FigJam](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2003-214) and used it alongside interview feedback when preparing the [Homework 04 priority matrix](../04/README.md).

A future audit could include screenshots and task observations from the current live listing editors.
