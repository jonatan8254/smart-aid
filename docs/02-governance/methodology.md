# Methodology — a lifecycle with brakes

> **Status:** `DOCUMENTED`, applied to the documentary work and, since August 2026, to a build. This page describes the approach in general; the step-by-step procedure and gate criteria are internal.

## The hybrid lifecycle

The project runs a **hybrid cycle: iterative delivery inside a V-shaped discipline, with explicit gates between phases.** Sprints produce artefacts; gates decide whether the next phase may open. A gate is a *verifiable condition*, not a meeting — if the condition is not met, the phase does not open, no matter how much momentum there is.

That mechanism held where it mattered most. When the build finally happened, **the conversational endpoint never existed without its safety gate** — both landed in the same commit, and the gate runs *before* the model is called rather than filtering what it returns. The order was the whole point: a fallback added afterwards is a patch, not a design.

The same honesty requires the other half. The **evaluation harness** that the methodology places before user exposure is not built. It governs the product line's releases; the academic MVP — a course deliverable, on a course deadline — shipped ahead of it. That gate is open, and it is named as open in the [status matrix](../01-ecosystem/status-matrix.md) rather than quietly dropped.

## The ICONIX discipline

Analysis and design follow **ICONIX by increments**: domain model → use cases → textual specifications → robustness → sequence → classes. Two habits matter more than the notation:

- **Classes and database design come *after* robustness and sequence analysis** — the data model is earned from behaviour, not sketched first and defended later.
- **Every increment closes with traceability**: each requirement must reach at least one objective, one rule and one planned test, and orphans are checked mechanically, not by inspection. The public MVP package demonstrates the result — 26/26 functional requirements traced, zero orphans.

## Measurement over adjectives

Quality is not described; it is targeted. Quality requirements are anchored to **specific characteristics of ISO/IEC 25010:2023** — including its *safety* characteristic family — and each carries a measurable target defined through a **goal-question-metric** derivation. The targets themselves are design targets, not measurements, and are labelled as such wherever they appear.

Risk runs on the same principle: a maintained register with quantified priority numbers, stress-tested through **ordinal Monte Carlo simulation** and **adversarial scenario injection** — asking not "what could go wrong?" but "what happens to the ranking of what could go wrong when our estimates are themselves wrong?"

## Verbal models before diagrams

Every subsystem is first written as a **verbal model** — structured prose with a fixed set of required traits, versioned like code, with a ratchet rule: a new version may refine, never silently drop. Diagrams come after the words are stable. This is the single most distinctive habit of the corpus, and the reason a purely documentary project can be audited at all.

## What is deliberately not here

The step-by-step procedure, the per-gate criteria, the trait checklist of the verbal-model standard, and the internal phase queue are part of the working specification and are not published.

---

*Back to [documentation index](../README.md) · Related: [Decisions](./decisions.md).*
