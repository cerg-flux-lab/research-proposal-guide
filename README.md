# Writing a Good Research Proposal

A practical guide for MEng and PhD students of the **CERG-FLUX Lab (Fluids, Learning and Uncertainty in compleX systems)**, Department of Mechanical and Aeronautical Engineering, University of Pretoria.

This repository accompanies the UP Library's [Research Guide: Research Proposal](https://library.up.ac.za/c.php?g=485435&p=3333232). The Library guide tells you *what* a proposal must contain. This repository shows you *how* to write each part well, with examples drawn from computational and experimental engineering research: CFD, Lattice Boltzmann Methods, Scientific Machine Learning, detector thermofluids, and quantum technologies.

> A proposal is a map, not the journey. It must convince a reader that the question matters, that it is answerable, and that *you* can answer it with the time and resources available. It does not need the answer.

---

## A proposal is a plan

Treat the proposal as a plan for the research, not as a document written to satisfy a committee. Without a plan, research stagnates: months pass on reading, tinkering and half-started simulations with no clear sense of what is finished and what is next. A written plan tells you, and your supervisor, what the next step is and how you will know when it is done.

The plan is not set in stone. The research **will** pivot as you progress. A method will fail to converge, the literature will reveal a result you did not know about, the experiment will need redesigning, or an unexpected finding will prove more interesting than the one you set out to find. That is normal, and it is not a failure of the proposal.

A plan is still better than no plan. When you have a proposal, a pivot is an informed decision: you can see which objectives are affected, what the change costs in time, and what still holds. Without one, a pivot is just drift. Write the proposal so that it can be revised, and revise it when the research changes.

## Perfect enough, not perfect

Your supervisor would rather see an imperfect proposal they can give feedback on than a perfect one they never see. A draft that sits on your machine for three months while you polish it produces no feedback, no direction and no progress. A rough draft sent in week three produces all three.

The aim is **perfect enough**: the argument is there, the sections exist, the objectives are stated, and the gaps are marked honestly as gaps. Send that. Feedback on a flawed draft is cheap and fast. Rewriting a polished draft that went in the wrong direction is neither.

In practice: send the one-page concept note before you have anything else. Send each draft as soon as it is complete enough to be read end to end, with a note on where you are unsure. Commit and tag each version so the history of the revisions is visible. The proposal will change after approval anyway, so do not spend the effort before approval trying to make it final.

## From proposal to dissertation: Chapters 1 and 2

An approved proposal is not filed away. It becomes the first two chapters of your dissertation or thesis, and most of its remaining sections map onto later chapters.

| Proposal section | Becomes | What changes |
|---|---|---|
| Background and rationale | Chapter 1 (Introduction): context and motivation | Tightened and rewritten for a reader who will go on to read the whole thesis |
| Problem statement and gap | Chapter 1: problem statement | Sharpened in light of what you actually found and where you pivoted |
| Aims, objectives, research questions | Chapter 1: aims and objectives | Revised to match the work that was done, not the work that was planned |
| Scope and limitations | Chapter 1: scope and delimitations | Updated honestly; new limitations added |
| Expected contribution | Chapter 1: contribution and thesis outline | Written as actual contributions, with a chapter-by-chapter roadmap |
| Literature review (2 to 6 pages) | Chapter 2 (Literature Review) | Expanded substantially in breadth, depth and currency; see below |
| Methodology | Chapter 3 (and often 4) | Expanded from a plan into a full account of what was done and why |
| Timeline, risk, resources | Nowhere | Project management, not thesis content |

### Grounding versus depth

The proposal and Chapter 1 must be **grounded** in the literature. Every claim about why the problem matters and what is missing must rest on cited work, and the gap must look inevitable by the time the reader reaches it. But grounding is not the same as a review. In the proposal, and again in Chapter 1, the literature appears in service of the argument: a paragraph or two per theme, the seminal and closest works only, and a pointer forward to Chapter 2 for the rest. A reader with no access to Chapter 2 should still be able to follow Chapter 1 and accept its problem statement.

Chapter 2 is a different kind of document. It is the examiner's evidence that you command the field, and it is judged on **depth**:

- **Breadth.** The field, the adjacent fields you draw methods from, and the benchmarks and standards you validate against. The proposal review covers the direct path to your gap; Chapter 2 covers the territory around it.
- **Critical engagement.** For each major work: what was done, under what assumptions, what it showed, what it did not show, and why that matters for your research. Summary is not enough. Every subsection should still end with a "However, ..." that leads somewhere.
- **Synthesis.** Comparison tables of methods, assumptions, benchmarks and reported accuracy. These are the parts of Chapter 2 that examiners read most carefully.
- **Currency.** Updated to the date of submission. Work published after your proposal was approved must be found, read and placed. For a three- or four-year PhD, that is often a large fraction of the chapter.
- **Length.** Typically several times the proposal review. The 40 to 80 sources of a PhD proposal usually become well over a hundred that each do work in the argument.

Do not paste the proposal review into Chapter 2 and add to it. Rewrite it. The proposal argued for the gap you intended to fill; Chapter 2 argues for the gap you did fill, and after the pivots described above the two are rarely the same. Keep the funnel structure from `docs/04-literature-review.md`, but let the funnel be wider at the top and much longer in the middle.

A useful test for the two chapters: if a reader who does not know the field can follow Chapter 1 on its own, it is grounded. If a reader who knows the field well learns nothing from Chapter 2, it is not deep enough.

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
