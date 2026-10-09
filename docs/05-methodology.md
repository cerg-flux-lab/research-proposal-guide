# 05. Methodology

The UP Library outline frames methodology as research design, sampling, data collection and data analysis. Those labels come from the social sciences. The table below translates them for computational and experimental engineering, which is where most CERG-FLUX Lab (Fluids, Learning and Uncertainty in compleX systems) work sits.

| Library heading | Computational research | Experimental research | SciML / ML research |
|---|---|---|---|
| Research design | Solver choice, physical models, numerical scheme, why this fidelity | Rig design, measurement principle, why this configuration | Architecture, loss formulation, physics constraints, baseline models |
| Sampling | Benchmark cases, geometries, parameter ranges, design of experiments | Operating points, replicates, test matrix | Training / validation / test splits, data generation strategy |
| Data collection | Hardware, run protocol, output quantities, storage | Instrumentation, calibration, sampling rates, logging | Data pipeline, provenance, augmentation |
| Data analysis | Verification, validation, grid convergence, UQ | Uncertainty analysis, statistical treatment, repeatability | Metrics, ablations, generalisation tests, error analysis |

## Research design: justify, do not just describe

The question the committee asks is not "what will you use?" but "why that?". For every major choice give the alternative you rejected and the reason.

- *Why LBM rather than finite volume for this problem?* (e.g. interface emerges from the mesoscopic model; local collision operator parallelises well on GPU.)
- *Why a PINN rather than a surrogate trained on CFD data?* (e.g. sparse data regime; need for physically consistent predictions off the training manifold.)
- *Why RANS rather than LES at this stage?* (e.g. parametric sweep of 200 cases; LES reserved for validation at three points.)

If you cannot give the reason, you have not chosen the method; you have inherited it.

## Verification and validation

Computational proposals are routinely returned for lacking a V&V plan. State it explicitly, using the standard vocabulary (Roache; Oberkampf and Roy; ASME V&V 20):

- **Code verification**: does the code solve the equations correctly? Method of manufactured solutions, comparison with analytical solutions (Poiseuille, Couette, Taylor-Green vortex, Laplace law for multiphase).
- **Solution verification**: is the discretisation error quantified? Grid or lattice convergence study, time-step independence, iterative convergence criteria. Name the method (e.g. Richardson extrapolation with the grid convergence index per Celik et al. 2008).
- **Validation**: does the model represent reality? Comparison against experimental data *with experimental uncertainty bands*. Name the dataset now. "Validation against experimental data" with no dataset named is a red flag.
- **Uncertainty quantification**: which inputs are uncertain, and how will their effect on outputs be estimated?

For ML and SciML work, the equivalents are: unit tests on the loss and physics residuals; convergence with respect to collocation points and network width; held-out test sets drawn from outside the training distribution; comparison against a classical solver of known accuracy; and ablations that show which component is responsible for the result.

## Cases and parameter ranges

Define the test matrix now. A table of cases (geometry, boundary conditions, dimensionless numbers, mesh size, expected wall-clock cost) does three things: it bounds the scope, it feeds the timeline, and it shows the committee you have thought about cost.

## Data collection and management

- Hardware: which machine, how many cores or GPUs, access arrangements (UP HPC, CHPC, Lab cluster, cloud credits).
- Software: name, version, licence. State whether you will develop, extend or use as-is.
- Storage: where raw results live, naming convention, backup. Link this to the Research Data Management section in chapter 07.
- Reproducibility: version control for code and input files; container or environment specification; a run log.

## Preliminary results

If you have any, include them. A single verified result (a Poiseuille profile from your own LBM code, a loss curve from a PINN on a toy problem, a calibration plot from your rig) is the strongest feasibility evidence you can offer. Label it clearly as preliminary.

## Quality of research

The Library outline asks for this as a separate section. For engineering it means: how will a reader trust your results? Answer with your V&V plan, your treatment of uncertainty, your reproducibility measures, and your plan for peer review (conference paper at month X, journal submission at month Y).

Next: `06-feasibility-timeline-and-risk.md`
