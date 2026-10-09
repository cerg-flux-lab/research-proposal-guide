# 03. Problem statement, research questions and objectives

This is the most important page of the proposal. Committees read it first and judge everything else against it.

## The problem statement

One paragraph. It must contain, in this order:

1. **Context**: the specific setting (not the whole field).
2. **The gap**: what is not known, not possible, or not reliable.
3. **The consequence**: why the gap matters, to whom.

A useful test: could a committee member read your problem statement aloud and the room would understand exactly what the thesis is about? If it needs the rest of the document to make sense, it is not finished.

**Weak:** "Multiphase CFD is important in many industries but remains challenging."

**Strong:** "Air-core formation in hydrocyclones governs separation efficiency, yet Navier-Stokes solvers with interface-capturing require empirical tuning of the interface model and fail to predict air-core diameter within 15% across the operating range reported by [refs]. No published study has established whether a Lattice Boltzmann multiphase model can predict air-core onset and diameter without case-specific tuning."

The second version names a quantity, a failure mode, a number, and a missing study. Every clause is checkable.

## Research questions

Convert the gap into one primary question and, at most, three secondary ones. Good research questions are:

- **Answerable** with the method you propose and the data you can obtain.
- **Falsifiable**: there is an outcome that would count as "no".
- **Bounded**: parameter ranges, geometries, regimes are stated.
- **Not yes/no questions** unless the yes/no is itself the contribution.

**Weak:** "Can machine learning improve CFD?"

**Strong:** "Within what range of Reynolds number and training data volume does a physics-informed neural network reproduce the lid-driven cavity velocity field to within 2% L2 error of a mesh-converged finite-volume solution, and at what fraction of the finite-volume wall-clock cost?"

## Aim versus objectives

- **One aim.** The aim is the research question rephrased as an intention. "To establish whether..." or "To quantify the...".
- **Three to five objectives.** Each objective is a deliverable step towards the aim. Each must be verifiable: a reader should be able to tick it off.

Use the SMART test on each objective: Specific, Measurable, Achievable, Relevant, Time-bound. The timeline chapter supplies the T.

| Weak objective | Why it fails | Strong objective |
|---|---|---|
| Develop an LBM solver | Not measurable; "develop" has no end point | Implement a D3Q19 LBM solver with a free-energy multiphase model and verify it against the Laplace law and the Rayleigh-Taylor benchmark to within 1% of published reference data |
| Study the effect of turbulence | No variable, no range, no metric | Quantify the sensitivity of predicted air-core diameter to inlet velocity (5 to 15 m/s) and spigot diameter (10 to 25 mm) using a validated model |
| Compare with experiments | Which experiments, which quantity, what tolerance | Validate predicted tangential velocity profiles against the LDA measurements of [ref] at three axial stations, reporting error with experimental uncertainty bands |

## Scope and delimitations

State explicitly what you will **not** do. This protects you in the viva. Common delimitations in computational work: fixed geometry, isothermal flow, Newtonian fluid, single hardware target, no experimental campaign of your own. A delimitation is a choice you justify; a limitation is a weakness you acknowledge. Keep them separate.

## Hypotheses

Not every engineering thesis needs a formal hypothesis, but if your question has a predicted answer, state it. "It is hypothesised that the LBM model will predict air-core diameter within 5% without tuning, because the interface emerges from the mesoscopic model rather than from an imposed reconstruction." The "because" is what makes it a hypothesis rather than a guess.

Next: `04-literature-review.md`
