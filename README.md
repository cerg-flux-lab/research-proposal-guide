# Writing a Good Research Proposal

A practical guide for MEng and PhD students of the **CERG-FLUX Lab (Fluids, Learning and Uncertainty in compleX systems)**, Department of Mechanical and Aeronautical Engineering, University of Pretoria.

This repository accompanies the UP Library's [Research Guide: Research Proposal](https://library.up.ac.za/c.php?g=485435&p=3333232). The Library guide tells you *what* a proposal must contain. This repository shows you *how* to write each part well, with examples drawn from computational and experimental engineering research: CFD, Lattice Boltzmann Methods, Scientific Machine Learning, detector thermofluids, and quantum technologies.

> A proposal is a map, not the journey. It must convince a reader that the question matters, that it is answerable, and that *you* can answer it with the time and resources available. It does not need the answer.

---

## How to use this repository

1. Read `docs/01-purpose-and-mindset.md` first. It is short and it reframes what you are actually being asked to do.
2. Work through `docs/02` to `docs/10` in order. Each chapter maps to a section of the proposal.
3. Copy a template from `templates/` into your own proposal repository and fill it in.
4. Before sending a draft to your supervisor, run `checklists/self-review-checklist.md`. Your supervisor will use `checklists/supervisor-review-checklist.md`, so you may as well pass it first.
5. Keep your proposal under version control. Commit early, commit often, and tag the version you submit.

## Repository structure

```
research-proposal-guide/
├── README.md
├── LICENSE                                  CC BY 4.0
├── resources.md                             UP Library, books, videos, UP templates
├── docs/
│   ├── 01-purpose-and-mindset.md            What a proposal is for
│   ├── 02-anatomy-of-a-proposal.md          Section-by-section map (UP Library outline)
│   ├── 03-problem-statement-and-questions.md
│   ├── 04-literature-review.md
│   ├── 05-methodology.md                    Computational and experimental methods
│   ├── 06-feasibility-timeline-and-risk.md
│   ├── 07-ethics-data-and-ai-use.md
│   ├── 08-writing-and-style.md
│   ├── 09-common-mistakes.md
│   └── 10-defending-your-proposal.md
├── templates/
│   ├── proposal-template.md                 Markdown skeleton
│   ├── proposal-template.tex                LaTeX / Overleaf skeleton
│   ├── one-page-concept-note.md             Write this before the full proposal
│   └── gantt-template.md                    Mermaid Gantt chart
├── checklists/
│   ├── self-review-checklist.md
│   └── supervisor-review-checklist.md
└── examples/
    └── worked-examples.md                   Weak versus strong, side by side
```

## The three questions every proposal must answer

| Question | Where it is answered |
|---|---|
| **Why** does this matter? | Background, rationale, research problem |
| **What** exactly will you do? | Aims, objectives, research questions, scope |
| **How** will you do it, and how do we know it will work? | Methodology, validation, timeline, risk |

If a reader cannot find a clear answer to all three within the first two pages, the proposal is not ready.

## Lab conventions that apply to proposals

- UK English. No em dashes.
- LaTeX on Overleaf is the Lab default for the final document; Markdown is fine for early drafts.
- SI units throughout. Define every symbol at first use.
- Figures in vector format where possible, legible at single-column width.
- Every citation must be one you have actually read. See `docs/07-ethics-data-and-ai-use.md` on the use of AI tools, which follows the Lab's [AI Research Guardrails](https://github.com/cerg-flux-lab/ai-research-guardrails).

## Contributing

Students and collaborators are welcome to open issues or pull requests: corrections, better examples, additional checklists. Keep the tone practical and the examples honest.

## Licence

Content is released under [CC BY 4.0](LICENSE). Attribute to the CERG-FLUX Lab (Fluids, Learning and Uncertainty in compleX systems), University of Pretoria.

Lab website: https://cerg-flux-lab.github.io/ | GitHub: https://github.com/cerg-flux-lab
