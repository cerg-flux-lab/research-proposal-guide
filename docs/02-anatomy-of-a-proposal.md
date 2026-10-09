# 02. Anatomy of a proposal

The UP Library's generic outline is reproduced in the left column. The right columns say what each section must achieve and how long it typically runs in an engineering MEng or PhD proposal. Your Department's current template and page limit override this table.

| UP Library outline | What it must do | Typical length |
|---|---|---|
| **Working title** | State the subject, the method and the scope in one line | 1 line |
| **Background / rationale** | Take the reader from the field to the specific problem | 0.5 to 1.5 pages |
| **Literature review** | Establish what is known, what is contested, and where the gap is | 2 to 6 pages |
| **Research problem** | State the gap precisely, in one paragraph that can be quoted | 1 paragraph |
| **Justification, aims and objectives** | Say why closing the gap matters; give one aim and three to five measurable objectives | 0.5 to 1 page |
| **Methodology: research design** | Describe the approach (computational, experimental, hybrid) and why it suits the question | 1 to 3 pages |
| **Methodology: sampling / cases** | For engineering: benchmark cases, geometries, parameter ranges, datasets | 0.5 to 1 page |
| **Methodology: data collection** | Solver, hardware, instrumentation; how results are generated and stored | 0.5 to 1 page |
| **Methodology: data analysis** | Verification, validation, uncertainty quantification, metrics | 0.5 to 1 page |
| **Quality of research** | How you will know the results are trustworthy | 0.5 page |
| **Ethical considerations** | Ethics clearance, data management, AI tool use | 0.5 page |
| **Timeline and resources** | Gantt chart, milestones, compute, funding, risks | 1 page |
| **Bibliography** | Only sources you have read, in the Department's required style | as needed |

## The logical chain

Each section must hand a baton to the next:

```
Background -> Literature -> Gap -> Question -> Objectives -> Method -> Validation -> Timeline
```

A proposal fails when a link is missing. The commonest missing links are:

- Literature that never arrives at a gap (a summary, not an argument).
- Objectives that are not traceable to the question.
- A method with no validation plan.
- A timeline that ignores the method's real cost (mesh independence studies, training runs, experimental commissioning).

Test it: for every objective, point to the sentence in the literature review that motivates it, the paragraph in the methodology that delivers it, and the bar in the Gantt chart that schedules it. If any pointer is missing, fix the proposal, not the pointer.

## Front and back matter

Depending on the template you may also need: declaration of originality, abstract (write it last), nomenclature, lists of figures and tables, and appendices for preliminary results. Nothing essential goes in an appendix.

Next: `03-problem-statement-and-questions.md`
