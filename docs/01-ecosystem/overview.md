# The ecosystem: TalentTrack + Smart-AID

> **Status:** `DOCUMENTED` — the ecosystem exists as a governed documentary corpus. Its one buildable slice, the conversational companion, is `DEPLOYED` as an academic MVP built by the team. This page is a general overview; the module catalogue and internal specifications are not public.

## What it is

**TalentTrack + Smart-AID** is a two-sided ecosystem designed around one conviction: organisational well-being technology only deserves to exist if it can never be turned against the people it claims to serve.

- **TalentTrack** is the organisational side — talent, performance and workplace context.
- **Smart-AID** is the human side — emotional well-being, delivered as non-clinical support.

The two sides share a domain, but they are separated by design: well-being data is structurally barred from feeding evaluation, ranking or sanction. That separation is not a policy promise — it is written into the architecture, the data rules and the requirements.

## The human problem

Occupational stress is one of the least well-served problems in applied technology. The World Health Organization estimates that 15 % of working-age adults were living with a mental disorder (2019 estimate) and that 12 billion working days are lost each year to depression and anxiety (WHO, *Mental health at work*, 2022); in Colombia, 2024 press coverage of consultancy findings, echoed by the Ministry of Labour, put close to 80 % of workers describing elevated stress (El Tiempo, 2024) — a sector-report figure, treated as signal rather than statistic. Conventional responses — workshops, leaflets, campaigns — offer no personalisation, no continuity, and no capacity to act at the moment it matters.

At the same time, conversational AI has entered this space faster than its safety engineering. The ecosystem's founding premise is that **emotional safety outranks engagement**, and that this must be enforced architecturally.

## Who is in it

The domain model recognises several distinct kinds of actor — individual users, organisational roles (management, human resources), citizens outside any organisation, mental-health professionals, health-network administration, and platform administration. Their **coexistence is precisely why the non-punitive rule is structural**: the moment an employer role and a well-being record live in the same system, "we won't use this against you" has to be an architectural fact, not a terms-of-service sentence.

## The shape of it

The ecosystem is specified as a deliberately bounded set of modules with declared priorities — a small MVP core, a second wave, and optional extensions. The conversational module, the current priority, decomposes into **25 internal submodules** supported by **14 external modules** and **17 cross-cutting domains**.

The catalogue itself — which modules, how they decompose, how they relate — is part of the internal specification and is not published. What matters here is the discipline: **everything ambitious is classified as extended scope, not commitment**, and the buildable slice is kept deliberately narrow. That slice is no longer only an expression on paper: it was built and deployed as an academic MVP, and its public home is the [Alan & Aura academic repository](https://github.com/jonatan8254/alan-aura-academico).

## The safety canon

A minimum canon governs every artefact in the corpus. It is published here in full because it is a declaration of limits, not of design:

1. **No clinical over-claim.** The system does not diagnose, does not deliver therapy, and does not handle emergencies autonomously.
2. **Granular, revocable consent** — consent precedes any data capture and any conversation.
3. **Minimisation.** The language model receives a bounded profile capsule, never raw history, questionnaire items, journals or biomarkers.
4. **Non-punitive use.** Well-being data can never feed evaluation, ranking or sanction.
5. **Minimal disclosure**, with graduated levels, and **anti-re-identification** in any aggregate view.
6. **No critical route is ever blocked by payment status.**
7. **Emotional safety outranks engagement** — always, in every trade-off.
8. **Adults only (18+)** for the MVP: a hard block rather than a soft warning, and never a registration of minors. In the build it rests on self-declaration with immediate sign-out, not on identity verification.

## Where the work is

| Layer | Where |
|---|---|
| The bounded, buildable slice — analysis, design **and the deployed MVP**, public | [`alan-aura-academico`](https://github.com/jonatan8254/alan-aura-academico) · [live](https://alan-aura-academico.vercel.app) |
| The governed corpus: domain canon, quality model, risk apparatus, audit pipeline | Private macro-repository — described in the [status matrix](./status-matrix.md), available on request |

---

*Back to [documentation index](../README.md).*
