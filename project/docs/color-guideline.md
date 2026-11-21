# AutoPiac — Yellow & White UI Color Guideline

**Student:** Umut Can Birbir (DUJ3ZD)  
**Design file:** https://www.figma.com/design/Po5hpum1mNJ7VnfVc0FTmC  
**Date:** 2026-11-21  
**Status:** Visual palette applied to copied UI screens; final accessibility and visual QA pending.

## Rationale
The AutoPiac interface uses a warm yellow-and-white automotive-classifieds visual direction, inspired by a familiar Hungarian/Turkish online marketplace pattern rather than copying any competitor's logo or trade dress. The low-fidelity monochrome wireframes are preserved as evidence of process; the color exploration is a separate row of frames in the same Figma design document.

## Color Tokens

| Token | Hex | Usage |
| --- | --- | --- |
| Brand / Primary | `#FFD400` | Main buttons, step progress, actions |
| Brand / Yellow Pale | `#FFF7D8` | Helpful information cards and guidance |
| Brand / Yellow Soft | `#FFF0A8` | Success / special emphasis surfaces |
| Brand / Gold Border | `#E7CA63` | Highlighted cards and accents |
| Brand / Gold Text | `#775700` | Colored status and progress labels |
| Surface / White | `#FFFFFF` | Main form screens, inputs, cards |
| Surface / Warm | `#FFFDF8` | Optional page backgrounds |
| Text / Primary | `#1F1F1F` | Headings, labels and yellow CTA text |
| Text / Secondary | `#6D675C` | Descriptions and placeholders |
| Border / Neutral | `#D5D0C4` | Text field outlines and secondary buttons |
| Border / Error | `#B42331` | Invalid fields and error messages |
| Progress / Upcoming | `#E8E5DF` | Incomplete steps |

## UI Usage Rules

- **Primary action:** yellow background with dark text. Avoid white text on yellow due to insufficient contrast.
- **Secondary action:** white background with neutral border and dark text.
- **Progress:** yellow completed stages and neutral upcoming stages.
- **Information boxes:** light yellow surface, warm border, dark content.
- **Inputs:** white fields, neutral border and visible labels.
- **Validation:** dark red text and border, supported by explicit field-level instructions.
- **White space:** keep most screen area white; use yellow for decisions, progress and highlights.

## Figma Layers

**Original low-fidelity section:** 9 initial grayscale wireframe frames.  
**Color exploration section:** 9 cloned frames prefixed `COLOR /`, starting with node `9:2` and vehicle details `9:20`.

The colored frame set has buttons linked to corresponding colored screens. There are demonstration-specific links for photo requirements and missing-field error states. Like the monochrome prototype, inputs are illustrative Figma layers — not HTML inputs.

## Remaining Checks

- [ ] Final human visual inspection of all nine screens.
- [ ] Evaluate text and UI-component contrast ratios in final design.
- [ ] Confirm focus, hover and disabled states when building reusable components.
- [ ] Conduct actual user tests and document observed issues.
- [ ] Compare before/after screens in the final course presentation.
