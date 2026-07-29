# Smart-AID — documentation

> [!NOTE]
> **This documentation is a general overview, by design.** It explains what was considered, what was decided and why — it does not publish the specification itself. Module catalogues, complete rule sets, thresholds, mapping tables and internal matrices are deliberately withheld, beyond what the main README already illustrates (see [`NOTICE.md`](../NOTICE.md)). If a page here feels high-level, that is a disclosure decision, not a lack of depth.

## Status convention

Every document opens with one of six labels, and no document mixes two without saying so:

| Label | Meaning |
|---|---|
| `DESIGNED` | The thinking exists: architecture, rules, models, decisions |
| `DOCUMENTED` | Written down, versioned, and internally traceable |
| `IMPLEMENTED` | Running code exists |
| `TESTED` | Tests were actually executed, with recorded results |
| `DEPLOYED` | Running in public, at a URL anyone can open |
| `PLANNED` | Declared intention — nothing more is claimed |

Where a component reached `IMPLEMENTED` or beyond through the academic team rather than the author's own commits, the row says **(team)**. That distinction is load-bearing: see [`NOTICE.md`](../NOTICE.md) §5.

## Contents

### 01 — The ecosystem *(the main project)*

| Document | What it covers |
|---|---|
| [Overview](./01-ecosystem/overview.md) | What TalentTrack + Smart-AID is, the human problem, the actors, and the safety canon that governs everything |
| [Status matrix](./01-ecosystem/status-matrix.md) | The real state of every component, with the six labels |

### 02 — Governance *(how the work is kept honest)*

| Document | What it covers |
|---|---|
| [Methodology](./02-governance/methodology.md) | The hybrid lifecycle, gates, and the ICONIX discipline |
| [Decisions](./02-governance/decisions.md) | The architecture decision records and the practice behind them |
| [Research & verification](./02-governance/research-and-verification.md) | The research series, its three-layer protocol, and the verification passes |

### 03 — Alan & Aura *(the conversational companion)*

| Document | What it covers |
|---|---|
| [The companions](./03-alan-aura/companions.md) | Who Alan and Aura are, and the rule that binds them |
| [Safety approach](./03-alan-aura/safety-approach.md) | The safety design in plain terms — and the honest boundary of what it is *not* |

### The boundary — deliberately not published

The quality-and-risk apparatus, the construction roadmap, the research programme's protocol and the wearable specification exist in the internal corpus and are **deliberately not published** beyond the overview the main README already gives. What is missing here is withheld, not pending. Access for review purposes is available on request.

---

*Part of [Smart-AID](../README.md) · © All rights reserved — see [LICENSE](../LICENSE).*
