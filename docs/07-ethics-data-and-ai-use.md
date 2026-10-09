# 07. Ethics, data management and the use of AI tools

## Ethics clearance

Engineering research that uses only simulation and published data normally requires an application to the Faculty of Engineering, Built Environment and IT (EBIT) Research Ethics Committee, even when the answer is "no human or animal participants". Do not assume exemption; confirm it. The UP Library's [Ethics Application Guide](https://library.up.ac.za/c.php?g=485435&p=11474672) walks through the process.

Flag in the proposal any of the following, since each triggers additional review:

- Human participants or personal data (surveys, interviews, usage logs). POPIA applies.
- Industrial data under NDA or third-party confidential data.
- Data from collaborations with external institutions (CERN, UJ, international partners) governed by their own agreements.
- Dual-use or export-controlled technologies.

## Research data management

The Library's [Research Data Management guide](https://library.up.ac.za/c.php?g=356288) sets out UP's expectations. In the proposal, cover:

- **What data** you will generate (simulation output, experimental logs, trained models, code) and roughly how much.
- **Where it lives** during the project and after (UP research data repository, UPSpace, Zenodo, institutional GitHub).
- **Naming and versioning** conventions.
- **Who may access it** and under what licence.
- **Retention**: UP requires research data to be retained for a defined period after completion; check the current policy.

A short data management plan (half a page) is enough for the proposal.

## Academic integrity

- Your proposal will be submitted through Turnitin. Similarity with your own prior work (e.g. an honours report) must be declared and cited.
- Paraphrase with understanding. If you cannot explain a paraphrased sentence without the source in front of you, you have not paraphrased, you have reworded.
- Every figure reproduced from a source carries a citation and, for publication, permission.

## Use of AI tools

The CERG-FLUX Lab (Fluids, Learning and Uncertainty in compleX systems) follows the [AI Research Guardrails](https://github.com/cerg-flux-lab/ai-research-guardrails). Read them before you write a word of your proposal. The summary:

**The viva test.** If you cannot defend a piece of work independently, without the conversation history, the AI did too much.

**Tier 1: your mind, your voice.** The proposal's argument, problem statement, research questions, methodology rationale, interpretation of literature and all scientific prose are yours. AI tools may explain a concept, ask you probing questions, flag an inconsistency, check a reference format or suggest a structure. They may not draft the prose, structure the argument or make research design decisions.

**Tier 2: your direction, AI drafting.** Administrative text (cover emails, ethics forms boilerplate) may be drafted by AI from your direction, provided you could have written it yourself.

**Tier 3: your specification, AI execution.** LaTeX plumbing, build scripts, plotting utilities, Gantt chart code and repository tooling may be produced by AI to your specification.

**Research code** is split: scientific logic (loss functions, boundary condition choices, physical reasoning behind parameters) is Tier 1; boilerplate is Tier 2 or 3.

**Disclosure.** Include a short statement in the proposal listing which AI tools were used and for what (e.g. "Claude was used for LaTeX formatting and reference-list checking; no scientific content was generated"). Do not list AI tools as co-authors or use `Co-Authored-By` trailers in commit messages. Check UP's current policy on AI use in postgraduate work, which may require a specific declaration form.

**References.** An AI-suggested reference is a search hint. It becomes a citation only once you have read the source and confirmed it says what you need.

Next: `08-writing-and-style.md`
