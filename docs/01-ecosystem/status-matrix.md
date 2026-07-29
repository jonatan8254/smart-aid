# Status matrix — what actually exists

> **Status:** `DOCUMENTED` — this page *is* the status declaration. Updated 2026-08-06.

The six labels are defined in the [documentation index](../README.md). The rule they enforce: **nothing is presented as more finished than it is.** Every figure below already appears in the main README; this page adds only the *where*.

Rows marked **(team)** were implemented by the four-person academic team under the author's lead and architecture — the author did not write the application code. The boundary is set out in [`NOTICE.md`](../../NOTICE.md) §5.

| Component | State | Where it lives |
|---|---|---|
| Ecosystem domain canon — with the conversational module decomposed into 25 internal submodules, 14 external modules and 17 cross-cutting domains | `DOCUMENTED` | Private corpus |
| Alan & Aura character system — 7-phase intervention cycle, 14 typified situations | `DOCUMENTED` | Private corpus |
| Conversational contract — hard clauses + personality traits | `DOCUMENTED`; enforced in the build by system prompts and output filters **(team)** | MVP-level version public in [`alan-aura-academico`](https://github.com/jonatan8254/alan-aura-academico) |
| Safety protocol — binary gate and deterministic fallback | `DEPLOYED` **(team)** — the gate runs before the model is called | Public in `alan-aura-academico` · live |
| Safety protocol — graduated S0–S5 triage scale | `DESIGNED` | Private corpus; **not** in the build |
| Evaluation harness — golden datasets, calibrated judge, release gates | `PLANNED` | Private corpus. **The honest gap:** the academic MVP shipped ahead of it |
| LLM architecture — four planes, two-speed loop, parallel guardian | `DESIGNED` | Private corpus |
| Requirements — 26 functional (26/26 traced, zero orphans), 10 non-functional, 10 quality | `DOCUMENTED` | Public in `alan-aura-academico` |
| Domain model & use cases — 16 classes and 17 relations, 14 use-case specifications | `DOCUMENTED` | Public in `alan-aura-academico` |
| Interface design — 16 screens, published as 21 self-contained mockup files | `DEPLOYED` **(team)** — built as 16 React screens behind 15 routed guards | Public in `alan-aura-academico` · live |
| Product application code — 13 REST routes over 14 functions | `DEPLOYED` **(team)** | Public in `alan-aura-academico` · live |
| Cloud infrastructure — 4 tables with 2 secondary indexes, versioned object storage, managed secrets, all as code | `DEPLOYED` **(team)** | Public in `alan-aura-academico` |
| Automated tests — 38 cases across 5 files, front end only | `TESTED` **(team)** — **the server has none** | Public in `alan-aura-academico` |
| Risk apparatus — 42 risks with RPN, 20 000-run ordinal Monte Carlo, 23 adversarial scenarios | `DOCUMENTED` | Private corpus |
| Test cases — 15 in Given/When/Then, tied to risks and gates | `DOCUMENTED`, **not executed as such** | Private corpus (test *planning* is also visible in `alan-aura-academico`) |
| Knowledge-graph tooling — ~36 Python scripts, verified rollback | `IMPLEMENTED` + `TESTED` | Private (methodology summarised here) |
| Wearable sensing architecture | `DESIGNED` | Redacted summary in the main README; specification private |
| Longitudinal research protocol (NeuroQuantIA) | `PLANNED` | Private, pre-publication |

Four things worth noticing:

- **The deployed rows are team work, and say so.** What is individually the author's is the design corpus above them — the canon, the requirements, the safety protocol, the architecture the build was made from.
- **`TESTED` covers the front end only.** 38 cases across error states and the safety path; the server has no automated tests, and that is a declared debt rather than an omission.
- **The safety protocol shipped narrow.** The deterministic gate is real and runs before the model — but it matches explicit signals, and the graduated scale stayed in the design. Both facts are stated where the capability is described.
- **The evaluation harness is the gap, and it is named as one.** It governs the product line's releases; the academic MVP is a course deliverable that shipped ahead of it.

---

*Back to [documentation index](../README.md).*
