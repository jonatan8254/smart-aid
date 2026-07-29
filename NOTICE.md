# NOTICE

Legal and attribution notices for the **Smart-AID** design, documentation and MVP portfolio.
This file complements, and does not replace, [`LICENSE`](./LICENSE) — **© All rights reserved**.

> [!NOTE]
> **The absence of an open-source licence is deliberate.** This repository is published to be read and evaluated, not reused. GitHub will show "No license" in its sidebar; that is the intended state, not an oversight. What a reader may do, and how to request anything further, is set out in [`LICENSE`](./LICENSE).
>
> Note also that GitHub's Terms of Service allow any platform user to view and fork public repositories regardless of the owner's licence choice. That platform-level permission cannot be revoked by choosing full copyright, and forking on the platform grants no right to redistribute, adapt or use this work outside it.

---

## 1. Author and copyright

**Jonatan Estiven Sánchez Vargas** — author, originator and lead of the Smart-AID line of work.
Copyright © 2025–2026. **All rights reserved.**

Systems and Informatics Engineering, Universidad Nacional de Colombia — Facultad de Minas, Medellín.

---

## 2. No patent licence is granted

This repository publishes engineering **reasoning, architecture and design rationale**. It does **not** grant, and must not be construed as granting, any licence, immunity or right under any patent, utility model, industrial design or other industrial property right, whether existing or applied for in the future.

Industrial property rights over the wearable sensing device and its analytical method are **expressly reserved**.

The engineering of the wearable device is **not published in this repository at any level of detail**. Its sensing configuration, system architecture, transport and interoperability choices, component-level specifications, sampling-parameter set, electronic integration design and the standards set it is specified against are all **deliberately withheld** and remain unpublished. What appears here is limited to what the line is, what it is not, and how far it was taken.

---

## 3. Trademarks

The following names are used as project and product identifiers and are reserved by the author:

- **Smart-AID**
- **Smart-AID Anti-Stress**
- **Alan & Aura**
- **SpectroStress**
- **NeuroQuantIA**

No licence to use these names, marks or associated visual identity is granted. Third-party names, standards bodies and product names mentioned in this repository are the trademarks of their respective owners and are used for identification and citation only.

---

## 4. Third-party material — cited, never redistributed

This repository **cites** standards and literature by identifier, clause and year. It **does not reproduce or redistribute** any of them. No copy of any standard, book or licensed corpus is present in this repository, and `.gitignore` is configured to keep it that way.

Standards and frameworks referenced include, among others: ISO/IEC 25010:2023, ISO/IEC 25030, ISO/IEC 25022, ISO/IEC 25023, ISO/IEC 25024, ISO/IEC 25040, ISO/IEC/IEEE 15939, ISO/IEC/IEEE 12207, ISO/IEC/IEEE 16326, ISO 9001, ISO/IEC 90003, ISO 45001, ISO 45003, ISO/IEC 27001, ISO/IEC 27701, WCAG 2.2, PMBOK Guide (7th ed.), and the methodological works of Wiegers (requirements) and Rosenberg (ICONIX). Standards specific to the withheld device line are not enumerated here, per §2.

Colombian legal instruments are cited as public law: Ley 1581 de 2012, Decreto 1377 de 2013, Ley 1480 de 2011, Resolución 0312 de 2019, Circular Externa 002 de 2024 (SIC).

Anyone wishing to consult these works must obtain them from their rights holders.

---

## 5. Attribution of collective work

Smart-AID spans several academic courses at Universidad Nacional de Colombia — Facultad de Minas. The boundary between individual and collective work is stated explicitly, by line:

| Line of work | Attribution |
|---|---|
| **Conception and direction** — idea, vision, business rules, ecosystem, verbal models, functional and non-functional requirements, planning, architecture, methodological tailoring, the Alan and Aura characters, quality requirements documentation, and the Monte Carlo risk simulation and its analysis | Individually authored and continuously led by the author |
| **Implementation Plan** (Software Quality course) | Collective deliverable of a four-member team. Named contributions by teammates: black-box and white-box test cases, user-story extraction with Planning Poker estimation, the development contract, and supporting diagrams |
| **Alan & Aura Académico** (Software Product Design and Construction course) — analysis, design **and the deployed MVP** | Collective deliverable of a four-member team, with the author as lead, architect, specifier and writer. **The author did not write the application code.** Construction credits, as published in that repository and contrasted against its history: the server, its infrastructure as code and the implementation of the 16 screens, **Santiago Bedoya García**; the client's planning and foundations — scaffolding, base components, design tokens, API layer, session and routing — **Luis Fernando Montoya Rodríguez**; the design class model, **Santiago Eusse Gil**. Published separately at `github.com/jonatan8254/alan-aura-academico` |
| **Smart-AID Anti-Stress** (Engineering Project Structuring and Evaluation course) | Collective deliverable of a **six-member team**, with the author as originator, director and researcher — responsible for the problem statement, state of the art, proposed solution, technical design and the main axis of the work, with sustained involvement in the economic study. Teammates are credited as a team; individual names are withheld pending their authorisation |

No individual is named **as a contributor to the work** without their name already being public in a repository they co-authored, or without their explicit authorisation. Teammates are therefore credited as teams, by course, until each has been asked.

This is distinct from the **Acknowledgements** section of the README, which thanks family and teaching staff for their support. Gratitude is not an attribution of authorship, and no one named there is presented as a contributor to, or as endorsing, this work. Any person named there will be unnamed on request.

---

## 6. No institutional endorsement

Affiliation with Universidad Nacional de Colombia, Facultad de Minas, and with the research communities named in this repository, is stated as **context and participation**. It does **not** constitute institutional endorsement, certification, sponsorship or commercial backing of Smart-AID or of any product derived from it.

---

## 7. Not a medical device — no clinical claims

Smart-AID is designed as **non-clinical technology for emotional well-being**. Nothing in this repository may be read as a claim that any component diagnoses, treats, prevents or monitors any disease or condition, nor that any regulatory clearance or registration has been obtained.

No clinical validation has been performed. No research participant data has been collected and no study has been executed. No performance figure in this repository is a measured result of the author's own system: anything that reads as performance is a **design target**, a **projection**, or a **citation from published literature**, and carries that marking wherever it appears. Figures that describe the corpus or the build itself are counts of artefacts, routes, screens or tests — verifiable directly for the public artefacts, and on request for the private corpus.

The deployed MVP referenced in this repository is a **university course deliverable**, not a released service. It has no formal evaluation harness, its safety check matches explicit signals only, and its age limit rests on self-declaration rather than verification. Those limits are stated in the README and declared in the MVP's own repository.

---

## 8. Own visual assets

`assets/banner.svg` and `assets/badges.svg` are original works created for this repository, and like everything else here they are **all rights reserved**. Both are self-contained SVG: this repository loads **no image from any external host**, so nothing here can break or be tracked because a third-party service changed.

`assets/diagrams/domain-model.svg` and `assets/diagrams/use-cases.svg` are hand-authored SVG renderings of the PlantUML domain and use-case models published in the `alan-aura-academico` repository, reused here by their author.

`assets/screens/` contains the author's own browser renders of mockup files already published in `alan-aura-academico`. They depict design mockups, not a running product, and are captioned as such wherever they appear.

`assets/diagrams/ecosystem-diagram.png` and `assets/diagrams/two-speed-loop.png` are raster renders of the two Mermaid diagrams in this README. GitHub renders those diagrams natively from source, so these images are not used here; they exist so the same content can be published on platforms whose Markdown renderer does not support Mermaid.

`assets/photos/alan.jpg` is a personal photograph by the author of his dog Alan, **the emblem of the Smart-AID application**. All rights reserved; the image is not licensed for any use, and copyright metadata is embedded in the file itself. The character identity it represents is part of the reserved "Alan & Aura" brand (see §3).

`assets/logo/` contains the NeuroQuantIA visual identity, an original work of the author. It is **included for the documentation phase** — the pages covering the research programme — and is deliberately not displayed in the README, whose visual identity is Smart-AID's rather than NeuroQuantIA's.

---

*Last reviewed: 2026-08-06.*
