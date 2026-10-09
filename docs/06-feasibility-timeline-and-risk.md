# 06. Feasibility, timeline and risk

A committee can forgive an ambitious question. It will not forgive a plan that cannot be executed.

## Timeline

Use a Gantt chart (template in `templates/gantt-template.md`). Rules:

- **Work packages map to objectives.** One bar per objective, broken into tasks.
- **Milestones are deliverables**, not activities: "verified solver, report submitted", not "work on solver".
- **Writing is a task** with its own bars, starting early. Thesis chapters are drafted as results arrive, not in the final six months.
- **Build in contingency.** A realistic plan has 15 to 20% slack. If every bar ends the week before submission, the plan is fiction.
- **Include the fixed dates**: proposal defence, annual progress reports, conference deadlines, funding reporting, the registration window for examination.

Typical durations, MEng (two years) and PhD (three to four years), are given in the template. Adjust to your Department's rules.

## Cost realism for computational work

Estimate it and write it down:

```
cases x (cells or lattice sites) x time steps x cost per site-update / cores available = wall-clock
```

Add mesh independence (at least three meshes), re-runs after bugs (assume two), and post-processing. A plan that assumes every simulation runs once and works is not a plan. For ML, do the same with training runs: hyperparameter sweeps, seeds, ablations.

## Resources

State what you need and whether you have it:

| Resource | Need | Secured? | Source |
|---|---|---|---|
| Compute | e.g. 50 000 GPU-hours | Partly | UP HPC allocation, CHPC application pending |
| Software licences | e.g. commercial CFD package | Yes | Departmental licence |
| Experimental data | e.g. LDA dataset from [ref] | Yes | Published; author contacted for raw data |
| Funding | Bursary, running costs, conference travel | Yes / applied | NRF, Departmental, Lab |
| Supervision | Co-supervisor with ML expertise | Yes | Named |

## Risk register

Three to six risks, each with likelihood, impact and a mitigation that you control.

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Validation dataset unavailable at required resolution | Medium | High | Alternative dataset identified; fall back to code-to-code comparison with documented limitations |
| Multiphase model unstable at target density ratio | Medium | High | Begin at low density ratio; literature identifies stabilised collision operators to adopt |
| HPC allocation delayed | Low | Medium | Lab cluster sufficient for verification phase; defer parametric sweep |
| Training does not converge on full problem | High | Medium | Curriculum from 1D to 3D; ablation plan isolates failing component |

The mitigation column is the one the committee reads. "Monitor closely" is not a mitigation.

## Feasibility statement

Close the section with three or four sentences that say, in effect: the method exists, the data exists or can be generated, the compute is secured, the skills are in place or will be acquired by month X, and preliminary work shows the core step runs. That paragraph is what the committee is looking for.

Next: `07-ethics-data-and-ai-use.md`
