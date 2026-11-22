# AutoPiac — Public User-Review Evidence for Competitor UX

**Student:** Umut Can Birbir (DUJ3ZD)  
**Reviewed:** 22 November 2026  
**Scope:** Public user comments about Használtautó.hu and mobile.de, selected for relevance to **creating, correcting and managing a vehicle listing**. These complement the [official-source comparison](../../homework/03/README.md) and [source log](competitor-sources.md).

## Research Method

I searched Hungarian and German-language Reddit discussions, official app-store review pages and public customer-review sites. I focused on messages about publishing, photo visibility, technical vehicle data, editing, costs, search filters and usability. I also checked for positive impressions to avoid basing the comparison only on complaints.

**Evidence class:** All findings here are **individual publicly posted comments**, not verified observations of the live 2026 product and not results of a controlled usability study. Their accuracy, the commenters' exact circumstances and whether later versions fixed the issues are generally unknown. The sample was selected by relevance rather than statistical representativeness. I did not count comments as survey participants or treat app-search complaints as proof of listing-form problems.

## Használtautó.hu — Hungarian User Voices

| Source and date | Reported experience | UX implication | Confidence |
| --- | --- | --- | --- |
| [r/CartalkHungary: photo-package cost discussion](https://www.reddit.com/r/CartalkHungary/comments/1qfi94t/komolyan_20000_ft_hogy_k%C3%A9peket_rakhassak_fel/), 17 Jan 2026 | Several commenters object to paying to keep photos visible; some other users argue that the marketplace's reach can justify paid visibility. A figure mentioned in the discussion is **not** a verified current package price. | Show exactly which images remain visible on a free listing, for how long, and what a premium purchase changes. | Multiple self-reported viewpoints, no checkout test |
| [r/CartalkHungary: private-seller packages](https://www.reddit.com/r/CartalkHungary/comments/1klj70z), 2025 | A community post describes images remaining visible for an introductory period and then requiring a photo package; this broadly resembles the historical official guide. | Communicate free-to-paid transitions before publishing, not only afterward. | Community report, partly supported by official guide |
| [r/CartalkHungary: advertisement editing complaint](https://www.reddit.com/r/CartalkHungary/comments/1xtnten/ennyi_volt_a_hahu/), 11 Nov 2026 | A commenter says an ad was flagged following a mistaken report, but the detail they were required to correct was not editable. | Do not trap sellers in an unfixable validation/moderation state. Make required corrections and help paths clear. | Single unverified incident, search-visible quotation |
| [r/CartalkHungary: robot-check complaint](https://www.reddit.com/r/CartalkHungary/comments/1qxdc70/a_hahu_nem_akar_usereket/), 2026 | One commenter reports repeatedly hitting a robot-verification step when trying to start an advertisement, across browsers. | Explain verification errors and offer a meaningful retry or alternative, rather than an unclear dead end. | Single unverified incident |
| [Használtautó.hu App Store](https://apps.apple.com/hu/app/haszn%C3%A1ltaut%C3%B3/id1201640871), 10 Apr 2025 | One positive review describes the app as user-friendly, responsive and informative. | Preserve the simple, familiar marketplace structure; do not assume the entire experience is disliked. | Individual public review |
| [Google Play app reviews](https://play.google.com/store/apps/details?hl=hu&id=com.schibsted.hasznaltauto), 2026 examples | Some users describe search filters resetting after switching apps or not consistently applying. This concerns **buyer search**, not directly the seller editor. | In a future functional AutoPiac, consider preserving draft and search state across interruptions; not an observed listing problem. | Individual app reviews, different user task |

### Interpretation

The clearest seller-related public concerns are **the cost and continued visibility of images**, **correctability when an advertisement needs changes**, and **clear recovery from unexpected verification steps**. Positive app feedback supports keeping the UI straightforward. I have not independently confirmed that every reported fault still exists.

## mobile.de — German User Voices

| Source and date | Reported experience | UX implication | Confidence |
| --- | --- | --- | --- |
| [r/automobil: “Warum sind Auto Verkaufsapps so schlecht?”](https://www.reddit.com/r/automobil/comments/1mjt5rp), 7 Aug 2025 | A seller reports that the mobile.de app only offered manual transmission for their selected car configuration, although their vehicle was automatic. Others discussed reliance on incomplete catalog databases. | Auto-filled make/model/engine/gearbox data should be **editable**, with an exception or “not listed” route. | Seller anecdote and discussion, unverified |
| [r/LegaladviceGerman: motorhome category dispute](https://www.reddit.com/r/LegaladviceGerman/comments/1u0d2if/agbversto%C3%9F_be_mobilede/), 8 Jun 2026 | A seller reports being forced into a car category for a VW T6 California, later facing ad removal and a fee dispute. The company account and facts have not been independently verified. | Before paid publication, make category constraints and their consequences clear; provide correction/appeal options. | One detailed user report, disputed situation |
| [r/automobil: equipment data discussion](https://www.reddit.com/r/automobil/comments/1srjdlk), 21 Apr 2026 | A commenter who identifies as working at a dealership says equipment filled from the VIN is often incomplete and they supplement it manually. Their numerical claim about completeness is anecdotal, **not a measured statistic**. | Do not present equipment suggestions as unquestionable facts. Allow additions and corrections. | One self-described professional's comment |
| [r/automobil: complaints about fees and ads](https://www.reddit.com/r/automobil/comments/1liags5), 23 Jun 2025 | Commenters criticize paid listing thresholds, promotional clutter and perceived performance problems; other users may have different experiences. | Keep paid upgrades distinguishable from the listing's core functionality and avoid distracting promotional interruptions. | Opinion discussion, not controlled performance measurement |
| [Trustpilot mobile.de customer reviews](https://de.trustpilot.com/review/www.mobile.de), 2026 | Some reviewers criticize limits on how many pictures they can include; a review refers to a **15-image** ceiling when trying to document issues. An official [mobile.de seller FAQ](https://www.mobile.de/magazin/artikel/verkaufen-40898) also describes up to 15 images for its documented workflow. | Make image limits and documentation expectations explicit. Do not assume the same limit applies to every package or current use case. | Review with separately documented limit |
| [mobile.de iOS App Store reviews](https://apps.apple.com/tr/app/mobile-de-buy-sell-cars/id378563358?platform=iphone&see-all=reviews), review date not reliably established | A seller reports difficulty deleting an advertisement after selling; a developer response in the displayed review suggests a future fix. | Provide prominent “Sold / Unpublish / Delete” actions and useful confirmation states. | One historical app review; current status unknown |
| [Trustpilot reviews of mobile.de](https://de.trustpilot.com/review/www.mobile.de), examples dated Aug 2026 | Some buyers describe the search/filter options as clear and appreciate price comparisons and the large vehicle selection. This is **buyer-side** feedback, not a test of creating a listing. | Retain recognizable categories and clear price information; do not disregard competitors' strengths. | Positive individual reviews; different user task |

### Interpretation

The most useful seller-side concerns relate to **incorrect catalog-derived values**, **limited editing in special cases**, **category selection**, **photo limits**, and **paid listing expectations**. These are not proof that a random mobile.de seller will experience the same problems. Positive buyer reports show strengths in search and comparison, but cannot validate the listing editor.

## Thematic Comparison

| Theme | Használtautó.hu examples | mobile.de examples | AutoPiac design decision |
| --- | --- | --- | --- |
| Cost transparency | Debate about paid photo visibility | Concerns about paid listing thresholds and promotions | Label premium as optional; display exact effect and duration before purchase |
| Correcting vehicle data | Report about an uneditable flagged ad field | Reports of locked or incomplete vehicle/catalog data | Make fields editable and offer “unknown / other” routes |
| Photos | Complaints about continued image visibility | Concerns about image-count limits | Clear minimum and maximum count, cover identification, guidance and accessible reordering |
| Failure recovery | Reported verification dead end | Category/correction and ad removal disputes | Specific error explanations, retry and correction paths |
| Simple interaction | Positive review of app responsiveness | Positive comments about search/filter structure | Guided steps with clear labels rather than unnecessary controls |
| Completeness | First-time seller concern about important details (separate AutoPiac interview) | Reported missing equipment metadata | Grouped selectable equipment, condition disclosure and helpful explanations |

## Accessibility Limitations

**I did not find independently verified evidence in the sampled public comments that establishes a specific WCAG failure in either competitor's current authenticated seller form.**

Reviewers' complaints about form mistakes, app filtering, image limits and verification gates are **usability reports**, not substitutes for a keyboard-only test, screen-reader audit, focus analysis, target-size measurements or color-contrast testing. The [WCAG review checklist](../../homework/03/README.md) is therefore still a **planned direct assessment**, not completed competitor accessibility certification.

## What Is and Is Not Completed

- [x] Published-source competitor feature comparison.
- [x] Dated sample of external user reports and positive feedback, with direct links.
- [x] Common potential UX issues mapped to AutoPiac design decisions.
- [x] Separation of publicly posted claims from independently observed defects.
- [ ] Authenticated live-editor usability tests for each competitor.
- [ ] Direct keyboard, screen-reader and image-upload tests on each competitor.
- [ ] Statistical estimates of competitor issue frequency — not possible from this selected sample.

**Conclusion:** The public comments support the *importance* of editable fields, clear fees, photo guidance and error recovery as design priorities. They **do not** establish that AutoPiac is objectively more usable than either competitor or that the reported bugs are present in the latest product.
