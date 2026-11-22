# Homework 03 — Competitor Analysis

**Project:** AutoPiac | **Student:** Umut Can Birbir (DUJ3ZD)  
**Review updated:** 22 November 2026  
**Competitors:** Használtautó.hu (Hungary) and mobile.de (Germany)  
**Research question:** What can AutoPiac learn from established vehicle marketplaces while keeping the private-seller listing process easy to understand?

## 1. Research Method and Scope

I compared the public seller-facing pages and official guidance provided by both marketplaces. I reviewed how they describe vehicle data, equipment, condition, photographs, prices, paid upgrades and publishing. I also checked their public routes into the listing process.

**What I could inspect:** Publicly readable pages, the mobile.de public selling entry form, the competitors' own descriptions of their workflows, and screenshots published in Használtautó.hu's 2025 step-by-step guide.

**What I could not independently test:** The complete authenticated listing editors, real uploads, keyboard navigation across the complete forms, error handling after invalid submissions or real publishing. The mobile.de listing editor route returned no publicly readable form data in this review, and Használtautó.hu states that logging in is required before creating an advertisement. I therefore treat potential usability difficulties as **design questions**, not confirmed competitor defects.

**Evidence labels used below:**
- **Publicly visible:** Present on a public landing page.
- **Officially documented:** Described in a guide or product page, but not independently exercised in a live editor.
- **Design interpretation:** My recommendation for AutoPiac; not a measured competitor result.

## 2. Competitor A — Használtautó.hu

**Market:** Hungary. This is the most relevant local benchmark because AutoPiac is aimed at Hungarian private sellers.

The official listing walkthrough dated **14 April 2025** explains a sequence of sign-in, vehicle information, photographs/documents, photograph ordering and captions, advertising packages, optional promotion and confirmation. It describes required vehicle fields marked with an asterisk. Some fields can be automatically populated and then corrected by the seller. Another official selling guide describes a detailed equipment checklist and a limit of **12 photographs** for the documented process.

The photograph management step supports reordering by dragging and adding captions. The private-seller package description distinguishes a basic advertisement from paid visibility options. According to the published guide, uploaded pictures in the free package are visible for the **first three days**, while paid picture packages provide longer photo visibility; current purchase prices and eligibility depend on the platform's terms.

**2026 update:** A Használtautó.hu announcement dated **21 October 2026** describes an asking-price assessment showing whether the listed price is below, around or above comparable asking prices. A November 2026 company recap also describes this price assessment as part of listing creation. This is a useful newer benchmark that was missing from the original analysis. It is not evidence that the system can evaluate a vehicle's unique condition perfectly.

**Strengths supported by official sources:** broad data coverage; required-field guidance; editable automatic suggestions; structured extras; photo management; packages; market price context.

**Points for AutoPiac to consider:** Preserve completeness without overwhelming a first-time seller; make the consequences of optional packages clear; provide a non-dragging photo-order method in an eventual functional implementation.

**Sources:**
- [Official step-by-step listing guide — 14 Apr 2025](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/)
- [Official used-car selling guide — 2026](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/utmutato-hasznalt-auto-eladasahoz/)
- [Official tips for an effective advertisement](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-hirdess-a-hasznaltauto-hu-n-a-sikeres-jarmuhirdetes-titka-5-percben/)
- [New price assessment — 21 Oct 2026](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/realis-aron-hirdetned-az-autod-igy-segit-az-uj-arertekeles-a-hahu-n/)
- [2026 platform update — Nov 2026](https://garazs.hasznaltauto.hu/kereskedoknek/uj-felulet-app-arertekeles-ennyi-minden-valtozott-a-hahu-n-2026-ban/)

## 3. Competitor B — mobile.de

**Market:** Germany. I chose mobile.de as a second benchmark for mature listing content and guidance, not as a local Hungarian marketplace.

The [public seller landing page](https://www.mobile.de/verkaufen/auto) distinguishes **selling through a classified advertisement** from **selling directly to a partner dealer**. A publicly readable starting form includes vehicle make, model, first registration and mileage. These are directly visible public elements, but they are not the complete authenticated advertisement editor.

The official article **“Richtig inserieren” (9 Nov 2024)** identifies three parts of a useful listing: representative photos, a completed equipment list and a detailed description. It explicitly recommends describing repairs, paintwork, accidents and defects in the text rather than simply repeating the equipment checklist. The public safety/selling guide also emphasizes service documents, realistic pricing and disclosure of known problems.

The public [private-seller package comparison](https://www.mobile.de/service/pricelistConsumer) offers Basic, Standard and Premium packages, including optional promotional visibility and extra photos. Its official 2026 listing guide describes packages with different durations and features. Prices should be checked at purchase rather than copied into an enduring UX comparison.

**Strengths supported by official sources:** clear distinction between listing and direct sale; structured entry information; emphasis on equipment and history; detailed seller guidance; transparent existence of optional promotions.

**Points for AutoPiac to consider:** Keep vehicle equipment separate from narrative condition/history; make a seller's selected selling route unambiguous; offer optional price guidance without blocking the listing flow.

**Sources:**
- [Public seller landing page](https://www.mobile.de/verkaufen/auto)
- [How to describe a vehicle advertisement — 9 Nov 2024](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776)
- [2026 private listing guide](https://www.mobile.de/magazin/artikel/gebrauchtwagenverkauf-auto-inserieren-13368)
- [Official private-seller package comparison](https://www.mobile.de/service/pricelistConsumer)
- [Official selling and safety guidance](https://www.mobile.de/sicherheit/guide-and-tips/sicher-verkaufen)

## 4. Feature Comparison

| UX area | Használtautó.hu | mobile.de | Current AutoPiac design |
| --- | --- | --- | --- |
| Start / account | Login required for listing (official guide) | Public vehicle-start fields; full editor not tested | Linked Start and Vehicle Details frames |
| Vehicle data | Required fields and editable suggestions (documented) | Make, model, registration and mileage visible publicly | Guided fields; visual values do not save |
| Equipment | Broad extras checklist (documented) | Complete equipment list emphasized | **16 individually clickable choices** in 4 groups |
| Repairs and damage | Complete condition description encouraged; separate panel map not confirmed | Repair history, paintwork, accidents and defects emphasized | **One interactive front-left-fender selector** with five states |
| Photos | Up to 12 in documented guide; reorder and captions | Detailed photos recommended; extra images in premium packages | Five sample previews, cover guidance and two photo/error examples |
| Price guidance | Price assessment added in 2026 (company announcement) | Public value estimate route and comparison advice | Price entry mockup; **no live price assessment** |
| Paid options | Free and paid photo/visibility packages described | Basic / Standard / Premium packages | Optional premium concept; no checkout |
| Review / confirmation | Successful-listing confirmation described | Complete editor review not tested | Clickable Review → Edit and completion frames |
| Accessibility | No authenticated keyboard test performed | No authenticated keyboard test performed | Contrast spot checks; keyboard/reader testing still outstanding |

**Comparison note:** A production website and a clickable Figma course prototype are not at the same functional stage. The AutoPiac column describes what is *demonstrated*, not proof of feature parity.

## 5. Usability Heuristic Review — Six Design Questions

| Criterion | Evidence / risk to investigate | AutoPiac response |
| --- | --- | --- |
| **1. Visibility of required information** | Használtautó.hu documents asterisks and some automatic suggestions. Their current error feedback has not been tested. | Keep labels and required-field explanations visible; include a missing-field screen. |
| **2. Recognition instead of recall** | Both sources encourage structured equipment rather than relying only on free text. | Use four equipment categories with 16 interactive options; expand the catalog only if user testing supports it. |
| **3. Error prevention and recovery** | Missing data, too few photos and submission failures are plausible high-cost tasks; live competitor errors were not exercised. | Show missing-vehicle and insufficient-photo examples with return navigation. |
| **4. Control over photos** | Használtautó.hu documents drag-and-drop photo ordering and captions. Alternative keyboard handling remains unverified. | Show previews and a cover label; add keyboard-accessible move controls in a real implementation. |
| **5. Trust and disclosure** | mobile.de explicitly recommends mentioning accidents, repairs, repainting and known defects. | Keep a separate body-panel condition area with an Unknown state instead of forcing a false answer. |
| **6. Pricing and paid upgrades** | Both offer optional paid visibility. Használtautó.hu now documents a market-price assessment. | Clearly distinguish optional premium from required steps; price feedback is a possible future improvement. |

These are **design opportunities and hypotheses**, not six proven usability violations on competitor sites.

## 6. Accessibility Checks to Carry Forward

I used [WCAG 2.2](https://www.w3.org/TR/WCAG22/) to identify what a real implementation should verify:

| Check | WCAG criterion | Status / AutoPiac implication |
| --- | --- | --- |
| Form labels and required hints | 3.3.2 Labels or Instructions | Design guidance exists; implementation untested |
| Clear validation errors | 3.3.1 Error Identification | Two example states; error handling not executed |
| Keyboard interaction | 2.1.1 Keyboard | Actual keyboard behavior not tested in a production UI |
| Visible focus | 2.4.7 Focus Visible | A component focus state exists; no complete keyboard audit |
| Accessible photo sorting | 2.5.7 Dragging Movements | Offer reorder buttons, not only drag interaction |
| Target size | 2.5.8 Target Size (Minimum) | Verify click/tap targets on real devices |
| Color contrast | 1.4.3 Contrast (Minimum) | Selected AutoPiac color pairs checked separately; not full conformance |

**No claim of WCAG failure or compliance is made for Használtautó.hu or mobile.de.** A reliable verdict needs direct accessibility tests on their current live forms.

## 7. What People Report Online — Public Review Sample

I added a separate review of publicly posted comments from **Reddit, app stores and Trustpilot**, including positive and negative experiences. This is **secondary user-review research**, not a substitute for directly testing the current authenticated forms.

| Competitor | Publicly reported experience | Example source | AutoPiac design response |
| --- | --- | --- | --- |
| Használtautó.hu | Some private sellers object to image visibility becoming paid after an introductory period; other commenters value the marketplace's reach. | [Photo-package discussion, 17 Jan 2026](https://www.reddit.com/r/CartalkHungary/comments/1qfi94t/komolyan_20000_ft_hogy_k%C3%A9peket_rakhassak_fel/) | Explain free and premium photo visibility and duration before publication. |
| Használtautó.hu | One commenter says a reported ad required a correction in a field that was not editable. | [11 Nov 2026 discussion](https://www.reddit.com/r/CartalkHungary/comments/1xtnten/ennyi_volt_a_hahu/) | Allow corrections and show clear moderation-recovery steps. |
| Használtautó.hu | A reviewer describes a frustrating robot-verification step when starting an ad. | [2026 user discussion](https://www.reddit.com/r/CartalkHungary/comments/1qxdc70/a_hahu_nem_akar_usereket/) | Explain what failed and provide retry/support guidance. |
| Használtautó.hu | The app also receives praise for being user-friendly and responsive. | [App Store, 10 Apr 2025](https://apps.apple.com/hu/app/haszn%C3%A1ltaut%C3%B3/id1201640871) | Retain a familiar, uncluttered layout. |
| mobile.de | One seller reports a locked wrong gearbox option based on the chosen vehicle, while others discuss catalog data gaps. | [Reddit, 7 Aug 2025](https://www.reddit.com/r/automobil/comments/1mjt5rp) | Keep technical auto-fill editable and offer an alternative when missing. |
| mobile.de | Another seller reports a motorhome-category problem, paid-ad removal and difficulty correcting the category. | [Reddit, 8 Jun 2026](https://www.reddit.com/r/LegaladviceGerman/comments/1u0d2if/agbversto%C3%9F_be_mobilede/) | Validate categorization before paid submission and explain corrections. |
| mobile.de | A commenter identifying as a dealer describes incomplete equipment data imported from VIN. | [Reddit, 21 Apr 2026](https://www.reddit.com/r/automobil/comments/1srjdlk) | Let sellers inspect and change suggested equipment. |
| mobile.de | Reviews include criticisms of image limits and optional listing fees, but also praise for search options and comparing prices. | [Trustpilot, 2026 reviews](https://de.trustpilot.com/review/www.mobile.de) | Make limits and upgrades explicit without losing ease of navigation. |

**Evidence standard:** These are selected, self-reported experiences. Their factual details, prevalence and whether they still occur in today's software are **not independently verified**. Buyer-search reviews do not prove problems in the seller form, and none of these comments establishes a WCAG violation.

The review sample strengthens the design rationale for **editable technical information, clear photo/fee conditions, useful failure recovery, and maintaining a simple interface**. It does **not** establish that AutoPiac performs better than either competitor.

[Detailed external review evidence and caveats](../../project/docs/competitor-user-review-evidence-2026.md)

## 8. Key Design Decisions

**P1 — Keep the listing process simple, not empty.** The early AutoPiac walkthrough was liked for its simplicity. A first-time user's missing-equipment and missing-damage feedback showed that simplifying cannot mean excluding important seller information.

**P2 — Separate equipment from vehicle history.** Both competitors emphasize these as different information types. The current AutoPiac design now has four equipment groups and a separate condition selector.

**P3 — Explain photo requirements up front.** The AutoPiac five-photo minimum and cover-image preview are visible before Review. Future working software should also offer an accessible photo-order control.

**P4 — Make paid features optional and understandable.** Both competitors offer paid packages; avoid confusing visibility upgrades with required publishing steps.

**P5 — Consider price evaluation later.** Használtautó.hu's 2026 update makes market-price feedback a relevant competitive feature, but it is outside the semester prototype's current scope.

## 9. Evidence and Limitations

| Evidence type | What is available | What remains open |
| --- | --- | --- |
| Public entry pages | mobile.de public selling start; Használtautó.hu public sell entry | Full post-login edit screens |
| Official walkthrough illustrations | Használtautó.hu 2025 step-by-step article with screenshots; mobile.de seller guides and illustrated article | Up-to-date authenticated screenshots of both 2026 editors |
| Feature / pricing guidance | Both companies' official information; 2026 HAHU price-assessment announcement | Current transaction-specific prices and validation behavior |
| Task usability | Three people tested the **AutoPiac prototype**, with positive qualitative group feedback | Timed, independent task outcomes on either competitor |
| Accessibility | WCAG criteria and AutoPiac design spot checks | Actual keyboard/screen-reader audit of live competitor editors |

The competitor research gives AutoPiac design direction. It does **not** prove that competing platforms are confusing or less usable.

## Project Links

[Competitor findings in FigJam](https://www.figma.com/board/FReaY560jfsj9gfCeta8oB?node-id=2003-214) · [Detailed source log](../../project/docs/competitor-sources.md) · [Impact/Feasibility, Homework 04](../04/README.md) · [Current AutoPiac prototype](https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC?node-id=2003-2)
