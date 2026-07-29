# The safety approach — and its honest boundary

> **Status:** `DEPLOYED` in its narrow MVP form — the deterministic gate runs in the shipped build, ahead of the model. The graduated scale and the evaluation harness remain `DESIGNED` and `PLANNED` respectively. This page explains the approach in plain terms. The MVP-level protocol is public in [`alan-aura-academico`](https://github.com/jonatan8254/alan-aura-academico); the full internal scale and rule set are not.

## Three decisions, in plain terms

**1. The risk check runs *before* the model speaks.**
Most conversational systems generate a reply and then filter it. Here, every incoming message is screened first — and on a turn that trips the check, **the language model never produces the reply at all**. A deterministic, locally computed fallback answers instead: containment, and a referral to configurable help resources. Because that path involves no model and no network call to a provider, **it keeps working when the provider is down** — which is precisely the moment it must not fail. It is also, by decision record, the *first* component to be built.

**2. Personality never outranks safety.**
Warmth is how the system speaks; it is never a reason the system may say something. Both companions operate under identical limits, and in safety mode the personality yields entirely — no humour, no metaphors, no play.

**3. The model receives a capsule, not your history.**
The language model is given a **bounded profile capsule** — a handful of self-reported fields with versioned metadata — plus the current exchange. It never receives prior sessions, questionnaire items, journals, biomarkers, identities or organisational data. Conversations are **not persisted**: when a session closes, its content is discarded. What the model never receives, no prompt attack can leak, and what is never stored, no breach can expose.

## The honest boundary — what this is *not*

The public MVP-level protocol states its own limits, and they are worth repeating here because omitting them would be the very over-claim this project refuses:

- It is **not a clinical classifier** and produces no diagnosis of risk.
- It detects **explicit** danger signals; it does **not** detect implicit, ambiguous or concealed danger — a declared limitation, not an oversight.
- It does **not replace emergency services or professionals**; its whole job in a crisis is containment and handover to humans.
- The MVP check is **binary, not graduated** — the graduated severity scale exists in the internal design, and elevating to it is recorded as future work, not claimed as present capability.

Declaring the boundary is part of the design canon: honesty about reduction is a requirement, not an apology.

## Why this order of construction

The founding premise is that a language model improvising in a sensitive conversation is a hazard. Every decision above follows from taking that premise seriously: constrain first, converse second — and make the constraint survive the failure of everything else.

---

*Back to [documentation index](../README.md) · Related: [The companions](./companions.md).*
