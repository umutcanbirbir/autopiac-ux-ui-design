# AutoPiac — Competitor Research Evidence Log

**Student:** Umut Can Birbir (DUJ3ZD)  
**Checked:** 22 November 2026  
**Main report:** [Homework 03](../../homework/03/README.md)

## Method

I reviewed two competitors' public selling pages, published listing guides and package information. These are authoritative statements about their services, but **not** substitutes for completing a real seller task. Screens that require a login, a valid vehicle or an actual advert submission were not tested.

The evidence is marked **Public** (page content readable without login), **Documented** (described in an official source) or **Not verified** (would require direct hands-on testing).

## Használtautó.hu — Hungary

| Source | Publication / context | What it supports | Evidence |
| --- | --- | --- | --- |
| [Step-by-step listing guide](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/hirdetesfeladas-a-hasznaltauto-hu-n-lepesrol-lepesre/) | 14 Apr 2025 | Account required; mandatory vehicle fields; some editable auto-filled suggestions; photo upload, reorder and captions; packages, promotion and confirmation screens | Documented, with guide screenshots |
| [Used-car selling guide](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/utmutato-hasznalt-auto-eladasahoz/) | 2026 | Extras and specifications, 12-photo upload in described workflow, history documents, and price/package context | Documented |
| [Effective advertisement tips](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/igy-hirdess-a-hasznaltauto-hu-n-a-sikeres-jarmuhirdetes-titka-5-percben/) | 2026 | Equipment can be ticked in checkboxes; good photographs and accurate descriptions matter | Documented |
| [Price evaluation update](https://garazs.hasznaltauto.hu/ha-autot-adnal-el/realis-aron-hirdetned-az-autod-igy-segit-az-uj-arertekeles-a-hahu-n/) | 21 Oct 2026 | New price-assessment guidance: below, within or above the typical asking-price level for comparable vehicles | Company announcement |
| [2026 product recap](https://garazs.hasznaltauto.hu/kereskedoknek/uj-felulet-app-arertekeles-ennyi-minden-valtozott-a-hahu-n-2026-ban/) | Nov 2026 | Confirms refreshed public browsing surfaces and a price-assessment feature in listing creation | Company announcement |
| [Public service / package entry](https://www.hasznaltauto.hu/kepcsomagok) | Publicly accessible | Public routes towards private seller and package information | Public |

**Current access limitation:** The listing guide states that logging in is required to submit an ad. The publicly fetched site also displayed an automated verification message. No logged-in listing form was inspected or submitted.

**Caution on prices:** The 2025 walkthrough explains a three-day display of uploaded photos on the free package and describes longer display through paid photo packages. It should not be treated as a verified current quote for a specific 2026 listing. The official terms and purchase screen govern actual costs.

**Screenshot evidence:** The 2025 step-by-step guide contains owner-published screenshots of basic vehicle fields, photo sorting/captions, package choices and confirmation. They are *historical illustrated documentation*, not screenshots independently captured from the current 2026 application.

## mobile.de — Germany

| Source | Publication / context | What it supports | Evidence |
| --- | --- | --- | --- |
| [Public sell-car page](https://www.mobile.de/verkaufen/auto) | Publicly accessible | Separate listing vs dealer-direct sale paths; make, model, registration and mileage entry fields | Public |
| [How to describe an advert](https://www.mobile.de/magazin/artikel/richtig-inserieren-35776) | 9 Nov 2024 | Equipment list, pictures, detailed written description; maintenance, repairs, repainting and accidents | Documented, with article illustrations |
| [Used-car listing guide](https://www.mobile.de/magazin/artikel/gebrauchtwagenverkauf-auto-inserieren-13368) | 2026 | Listing sequence, photographs, private seller packages and durations | Documented |
| [Official selling/safety guide](https://www.mobile.de/sicherheit/guide-and-tips/sicher-verkaufen) | Public guidance | Price comparisons, vehicle history, paperwork, flaws and photo preparation | Documented |
| [Private-seller products](https://www.mobile.de/service/pricelistConsumer) | Public pricing/product page | Basic, Standard and Premium products, visibility options and extra images | Public |
| [Public listing start](https://www.mobile.de/verkaufen/a/fahrzeug/start?i=listing) | Entry route | Advert-start URL can be reached, but its interactive content was not readable to the research tool | Not verified beyond URL |
| [Authentication route](https://www.mobile.de/verkaufen/a/meinfahrzeug/?lang=de) | From an official article CTA | Redirects to mobile.de login in the public browsing context | Public route behavior |

**Current access limitation:** The complete seller editor was not accessible as a readable public form, and the article's listing CTA led to authentication. No actual car ad was created or submitted.

## Relevant WCAG 2.2 Criteria

[W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/)

- **1.4.3 Contrast (Minimum):** normal text needs adequate contrast.
- **2.1.1 Keyboard:** core functions must be operable by keyboard.
- **2.4.7 Focus Visible:** keyboard focus must be visible.
- **2.5.7 Dragging Movements:** provide an alternative to drag-only interactions.
- **2.5.8 Target Size (Minimum):** ensure control targets have sufficient area/spacing.
- **3.3.1 Error Identification:** explain detected input errors.
- **3.3.2 Labels or Instructions:** clearly label required information.

These are **future evaluation criteria**, not competitor accessibility findings. The logged-in editors of either competitor were not tested for WCAG compliance.

## UX Conclusions for AutoPiac

The highest-confidence design lessons are to retain a clear guided flow, keep equipment separate from condition/history, guide photographs before upload, avoid confusing optional paid promotions with mandatory steps and consider nonblocking market-price guidance later. AutoPiac currently demonstrates clickable equipment and one front-left-fender condition selector, but does not save the listing data.

**Unresolved research:** Live authenticated competitor screenshots, complete keyboard review, real error recovery, real photo upload behaviour, test duration and participant-observed issues. These should be collected only if the course specifically requires a hands-on competitor audit.

## Independent User-Review Sources — Added 22 November 2026

I also reviewed publicly posted Hungarian and German comments about seller costs, photo visibility, vehicle data auto-fill, editing/categorization and authentication issues, plus positive app/site experiences. The dated examples, source URLs and confidence notes are in [Public User-Review Evidence](competitor-user-review-evidence-2026.md).

The review sources include Reddit's [Használtautó.hu photo-package discussion](https://www.reddit.com/r/CartalkHungary/comments/1qfi94t/komolyan_20000_ft_hogy_k%C3%A9peket_rakhassak_fel/), [mobile.de auto-filled gearbox complaints](https://www.reddit.com/r/automobil/comments/1mjt5rp), [mobile.de vehicle-category dispute](https://www.reddit.com/r/LegaladviceGerman/comments/1u0d2if/agbversto%C3%9F_be_mobilede/), [Használtautó.hu App Store feedback](https://apps.apple.com/hu/app/haszn%C3%A1ltaut%C3%B3/id1201640871), and [mobile.de Trustpilot feedback](https://de.trustpilot.com/review/www.mobile.de).

**These are testimonials and public commentary, not a direct live-editor accessibility audit or verified defects.**
