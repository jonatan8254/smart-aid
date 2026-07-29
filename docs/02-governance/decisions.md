# Decisions — recorded, reversible, and owned

> **Status:** `DOCUMENTED` — three formal architecture decision records plus a running decision log. This page states what was decided and how; the full records (conditions, evidence, legal analysis) are internal.

## The practice

Every consequential decision in this project is recorded with the same anatomy:

- the **decision** and its status (recommended → adopted → adopted-operationally-pending-external-validation);
- the **evidence** it rests on;
- the **alternatives rejected, each with its reason**;
- the **negative consequences accepted** — every real decision has some;
- and **explicit reversal conditions**: what observation would reopen it.

One rule keeps the register honest: *if it is not in the register, it is not decided.* And a decision that required external validation says so on its face, rather than borrowing certainty it does not have.

## The three architecture decision records — of the **macro project**

> [!IMPORTANT]
> **Two decision series share the same numbers.** The three below belong to the **macro project** and govern the Smart-AID product line. The academic MVP repository keeps **its own five** — technical stack, reversion to serverless, no backup of personal data, immediate deletion, infrastructure tooling — under the same `ADR-00X` identifiers and with entirely different content. When citing one, name which series it belongs to.

**ADR-001 — the LLM architecture.** Adopts a governed reference architecture for the conversational release **under binding conditions** rather than as-is. The conditions concern data residency treated as a deployment variable, protection against vendor lock-in, a mandatory evaluation harness before any user exposure, and the order of construction — the deterministic crisis fallback before any feature. Alternatives (building a custom orchestrator, a thin wrapper, third-party SaaS, postponing) were each rejected with recorded reasons.

> Where this stands against the build: the construction-order condition held — the conversational endpoint never shipped without its gate. The **harness condition did not**: it governs the product release, and the academic MVP shipped ahead of it. Recorded here rather than elsewhere, because a decision register that only lists the conditions you met is not a register.

**ADR-002 — adults only.** The MVP is **18+, with a hard block** — not a soft warning. No parental-consent path exists because no minors are registered at all. An institutional mode for adolescents is recorded as a *declared future door, explicitly not a commitment*. The decision is adopted operationally and marked as pending professional legal validation — that pending status is part of the record, not a footnote. In the build the block is enforced by self-declaration with immediate sign-out, **not** by identity verification.

**ADR-003 — bilingual by design.** Spanish (Colombia) and English are treated with **full parity across every dimension**, under a per-language rule: no language is ever exposed to users without its own evaluation assets and its own green gates. Language, culture and jurisdiction are kept as separate concerns rather than collapsed into "translation". The reconstruction phase inherits this: artefacts are born bilingual, not translated late.

## The running log

Below the ADRs sits a running log of scoped decisions — extraction of the academic subproject into its own repository, data-boundary precisions, naming rules, scope closures. The public MVP package carries its own visible slice of this log — **53 recorded decisions and 5 architecture decision records** by the time it shipped — which is the easiest place to see the practice working: [`alan-aura-academico`](https://github.com/jonatan8254/alan-aura-academico).

## Why this matters more than any single decision

Any project can claim good judgement. A decision register with rejected alternatives, accepted costs and reversal conditions is **falsifiable judgement** — a reviewer can disagree with a decision and still verify that it was made responsibly.

---

*Back to [documentation index](../README.md) · Related: [Methodology](./methodology.md).*
