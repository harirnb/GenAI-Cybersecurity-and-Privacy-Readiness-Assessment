# GenAI Readiness — A Practical Cybersecurity & Privacy Assessment Framework for Australian SMEs

> A lightweight, evidence-based self-assessment that tells an organisation how ready it actually is to use Generative AI safely — not just what a policy document says.

![Status](https://img.shields.io/badge/status-Part_A_complete-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## The problem

Australian organisations are adopting GenAI tools faster than they're building the governance to manage them — by early 2026, adoption among SMEs had already passed 44%, while ownership, data controls, and oversight lag behind (National AI Centre, 2026). Existing guidance (NIST, OAIC, OWASP, ISO/IEC 42001) is comprehensive but fragmented — there's no simple, repeatable way for an organisation to answer basic questions like *who owns AI risk here*, *what's actually in use*, and *what should we fix first*.

## The evidence

- National AI Centre data shows adoption is outpacing formal governance, and guidance itself concedes that practices need to flex by organisation size — meaning "shadow AI" use is often a capability gap, not just a discipline problem.
- OWASP's LLM risk list (prompt injection, sensitive information disclosure, excessive agency) sits alongside traditional cyber fundamentals that haven't gone away — least privilege, logging, incident response.
- Three independent gap-analysis methods (NIST CSF current-vs-expected state, a likelihood×impact matrix, and a Five Whys root-cause trace) converge on the same conclusion: organisations lack a measurable, repeatable way to assess GenAI readiness.

## The solution

A 30-question readiness assessment across six domains, each question traceable to a named source (NIST CSF 2.0, NIST AI RMF, OAIC, OWASP, National AI Centre, ISO/IEC 42001). Scores run 0–4 per control, but self-reported scores alone aren't trusted:

- **Evidence caps** — without supporting evidence, a score can't exceed 1; with partial evidence, it caps at 3. Full marks require verified evidence.
- **Critical control gates** — six controls (AI owner, AI inventory, data classification, role-based training, supplier review, incident response) act as gates. Weak performance on any of these blocks an organisation from reaching "Managed" or "Optimised," regardless of the average score.
- **Weighted domains** — Governance, Privacy, and Cybersecurity are weighted highest (20% each), reflecting where the evidence shows the greatest organisational risk sits.

Output is a management-facing report: overall score, maturity band (Ad hoc → Basic → Managed → Optimised), domain breakdown, weakest controls, and six prioritised, owner-tagged recommendations.

## Tech stack

- HTML / CSS / JavaScript — static, client-side only
- No backend, no database, no cloud dependency (Part A prototype)

## Setup

```bash
git clone https://github.com/<your-username>/<project-slug>.git
cd <project-slug>
# open index.html directly in a browser — no build step, no server required
```

## Project roadmap

Part B (~300 hours, 10 weeks): reconfirm scope and source register → refine the 30-question control library → finalise scoring/weighting/gates → build and test the browser-based prototype → evaluate against two synthetic organisational scenarios and expert reviewer feedback → refine and hand over.

See the [project board](../../projects) for the current backlog and Sprint 1.

## Ethics, privacy and responsible AI

Guided by the ACS Code of Professional Conduct, the Australian Privacy Principles, and the NIST AI RMF (Govern, Map, Measure, Manage). The central ethical tension — security visibility vs. employee privacy — is handled by design: the framework only rewards monitoring that is documented, proportionate, and transparent, not monitoring that simply collects more data. The prototype itself runs entirely in-browser: no organisational data is uploaded, stored, or retained.

## Sustainability

As a static, locally-run web app with no model training and no cloud dependency, the prototype's compute and data footprint is minimal by design. The interface is built against WCAG 2.2 guidance (clear labelling, keyboard navigation, responsive layout).

## Documents

- [Proposal PDF](./docs/proposal.pdf)
- [Project Charter](./docs/charter.md)
- [Risk Register](./docs/risk-register.md)
- [RACI Matrix](./docs/raci.md)
- [Methodology](./docs/methodology.md)

## Contact

Hari Ranabhat — ranabhathari0@gmail.com

## Acknowledgements

Academic supervisor and industry panel (PROF909, Skyline Higher Education). AI Use Statement: see Appendix E of the proposal for tools, purposes, and verification approach.
