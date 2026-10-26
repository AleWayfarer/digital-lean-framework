# Digital Lean Framework (DLF)

**Less complexity, more results.**

The Digital Lean Framework applies lean thinking to the human and digital processes of organizations outside manufacturing: IT and digital service delivery, cybersecurity, leadership and people development, AI adoption, and the transformation programs that cut across them.

DLF is an **application layer for lean thinking, not a new school of thought**. It carries the full lean vertical (values → principles → methods → tools) into digital work, and it gives practitioners a way to check that the vertical holds. If a tool cannot be traced back to a principle and a value, it is lean theater.

🇮🇹 [Leggi in italiano](README.it.md) · 🌐 [DLF v2.4 on a page](https://AleWayfarer.github.io/digital-lean-framework/)

---

## The framework in one minute

**Law Zero: process before technology.** First simplify, then digitize, then automate. Never the other way around.

| Layer | What it contains |
|---|---|
| **4 cultural values** | Teamwork · Communication · Frugality and waste elimination · Continuous improvement |
| **5 pillars** | 1. Law Zero · 2. Internal customer-supplier chain · 3. Three Laws of Flow + Efficiency Matrix · 4. Direct and indirect needs + three sources of inefficiency · 5. Flow visibility and anomaly management (digital Jidoka) |
| **5 operating principles** | VALUE → STREAM → CLEAN → FLOW → KAIZEN |
| **9 digital muda** | Overprocessing · Waiting · Overproduction · Defects · Motion · Inventory · Transport · Unused Talent · Perfection Trap |
| **Digital Lean Index (DLI)** | Composite 0–100 score: 0–30 Critical · 31–55 Struggling · 56–75 In progress · 76–100 Excellent, read against the reachable frontier, not an ideal |
| **Efficiency Matrix** | Flow × resource quadrants: Desert · Islands · Ocean · Perfect State. Only the Desert must always be left; the target quadrant is a strategic choice |
| **Sprint Kaizen** | Two-week improvement cycles with a mandatory **Lean Test**: orphan tool, cosmetic method, strategy adrift |
| **Application surface** | 4 operational tracks (IT and Digital Service Delivery, Cybersecurity, Leadership & People, AI Adoption) + 1 transversal layer (Digital Transformation Programs) |

## What is in this repository

```
digital-lean-framework/
├── docs/                    DLF on a page (EN + IT), published with GitHub Pages
├── framework/
│   ├── it/                  Canonical edition (Italian): master framework, Operating Guide, 4 operational assets
│   └── en/                  English edition
├── skills/
│   ├── claude/              Lean Advisor skill for Claude (lean-advisor-en, lean-advisor)
│   └── gemini/              Lean Advisor as a Gemini Gem (EN, IT)
├── CHANGELOG.md · CITATION.cff · LICENSE.md
```

| Asset | Version | Purpose |
|---|---|---|
| Digital Lean Framework | 2.4 | Manifesto, architecture, pillars, principles, DLI, application by track |
| Operating Guide | 1.4 | Step-by-step application: assessment, sprints, Law Zero workflow, muda checklist |
| DLI Assessment | 2.4 | Step 0 → Step 6 assessment path, DLI formulas and thresholds |
| Muda Checklist | 2.3 | Diagnostic questions, scoring and indirect needs for the 9 muda |
| Sprint Kaizen | 2.2 | Rituals, templates and the Lean Test |
| Law Zero Workflow | 2.1 | Decision workflow with three paths (A: not digitized · B: remediation · C: human processes) |

PDF and Word editions, including figures, are attached to each [release](../../releases).

## The Lean Advisor (AI skill)

The Lean Advisor is an operational AI companion that walks a practitioner through a DLI assessment, a muda scan, a Sprint Kaizen, a Law Zero decision, or a DLI calculation, one step at a time and always against the framework text.

Available in English and Italian, for Claude (custom skill) and Gemini (Gem). Install instructions in [skills/README.md](skills/README.md).


## License

DLF — Digital Lean Framework © 2026 Alessio Setaro, licensed under [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/).

You may share the material with attribution, for non-commercial purposes, without modifications. Commercial use, adapted versions, translations, and training or consulting offerings built on DLF require written permission. See [LICENSE.md](LICENSE.md).

## Feedback

Field reports, questions and errata are welcome through [Issues](../../issues). The framework text is maintained by the author only, so pull requests are not accepted: see [CONTRIBUTING.md](CONTRIBUTING.md).

## Author

**Alessio Setaro** · Digital Lean Advisory · [LinkedIn](https://www.linkedin.com/in/alessiosetaro/)

If you reference DLF in your work, please cite it (see [CITATION.cff](CITATION.cff)).
