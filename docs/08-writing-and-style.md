# 08. Writing and style

## Language and conventions

- UK English (analyse, modelling, behaviour, optimisation). Set your spell-checker before you start.
- No em dashes. Use commas, colons, semicolons or full stops.
- SI units with a space between number and unit (15 m/s, 300 K, 2.5 MPa). Use the same decimal convention throughout.
- Define every symbol at first use and collect them in a nomenclature list. Check dimensional consistency in every equation.
- Numbers: write out one to nine in prose unless they carry a unit; use numerals from 10.
- Tense: present for established knowledge ("the LBM recovers the Navier-Stokes equations in the low-Mach limit"); past for what specific studies did ("Smith et al. measured..."); future for your plan ("the solver will be verified against...").

## Sentences and paragraphs

- One idea per paragraph; first sentence states it, the rest support it.
- Lead with the point. "Air-core diameter is under-predicted by 15% in [ref]" beats "In the study by [ref], it was found that there was an under-prediction of the air-core diameter of approximately 15%".
- Prefer active voice for what you will do ("I will implement..." or "The study will implement..."; check your Department's preference on first person). Passive is fine for established procedure.
- Cut hedges that carry no information: "it is important to note that", "in order to", "the fact that". Keep hedges that carry real uncertainty: "preliminary results suggest".
- Short words where they exist: use, not utilise; show, not demonstrate (unless you mean a formal demonstration).

## Figures and tables

- Every figure and table is referred to in the text before it appears, and the text says what the reader should see in it.
- Vector formats (PDF, SVG) for plots and diagrams; raster only for photographs.
- Legible at single-column width: axis labels at least 8 pt in the final document, with units.
- Colour-blind-safe palettes (viridis, Okabe-Ito). Do not rely on colour alone; vary line style or markers.
- Captions are self-contained: a reader looking only at the figure and caption should understand it.
- Reproduced figures carry a citation in the caption.

## The title

Formula that usually works: *[What you will do] of [the system] using [the method]: [the distinguishing scope]*.

"Prediction of air-core formation in hydrocyclones using a multiphase Lattice Boltzmann model: validation across the industrial operating range."

Avoid: "A study of", "An investigation into", "Towards", and anything that promises a "novel framework" before you have one.

## The abstract

Write it last. Five sentences: context, gap, aim, method, expected contribution. No citations, no undefined acronyms.

## Tools

- LaTeX on Overleaf is the Lab default for the final document. Use the Department's class or template if one exists; otherwise `templates/proposal-template.tex` is a starting point.
- Markdown is fine for early drafts and for this repository. Pandoc converts Markdown to LaTeX if you want to move later.
- Keep the proposal in version control. Tag the submitted version (`git tag v1.0-submitted`). You will want to know exactly what you promised.

Next: `09-common-mistakes.md`
