# Brendan Daly

**Applied AI and the economics of AI adoption.**

I build decision systems where the rules are explicit, the evidence is checkable, and a person stays accountable for the call. Alongside that I study where AI is actually being used across the labour market, and what that says about adoption.

From Cork, Ireland · based in South Bend, Indiana · [dalyventures.com](https://www.dalyventures.com/)

---

## Research

**[ai-wages](https://github.com/brdaly/ai-wages)** · Research · MIT

Where generative AI is actually used across the wage distribution. Joins the Anthropic Economic Index to BLS occupational wages and contrasts observed use with a decade of predicted-automatability forecasts. They are close to mirror images: observed exposure rises with wages, predicted automatability falls.

One command reproduces every number and figure from the committed public data, and CI re-runs the analysis on every change.

---

## Governed AI systems

Each of these separates deterministic rules, evidence, and model output. Each fails closed when the evidence is missing rather than guessing. Each keeps a human confirmation step on the consequential decision.

**[RealInsight](https://github.com/brdaly/RealInsight)** · Candidate

Bounded decision support for first-time home buyers. Deterministic extraction preserves exact source excerpts, a versioned rule engine owns every fit and coverage calculation, and the optional AI step is limited to drafting questions for the listing agent. The visitor must confirm the extracted facts before anything is evaluated. Next.js on Cloudflare Workers and D1.

**[Hot-Wheels-Agent](https://github.com/brdaly/Hot-Wheels-Agent)** · Candidate

Collector workspace built around a rights-governed media registry and a source register where every reference carries a retrieval date and an expiry. When a source goes stale the application refuses to promote new claims from it, and a scheduled job fails until the source is re-verified. Deterministic priority scoring, owner-only access with row-level security.

**[racing-intelligence](https://github.com/brdaly/racing-intelligence)** · Labs/Prototype

Evidence-governed publication board that separates current publication status from historical performance, and pauses rather than presenting archived prices as live.

Status tiers follow the definitions in [SUPPORT.md](https://github.com/brdaly/.github/blob/main/SUPPORT.md): Production, Candidate, Labs/Prototype, Research, Historical.

---

## How I build

- **Rules own decisions; models supply observations.** Scoring and gating logic is versioned code, never a prompt.
- **Evidence carries provenance and an expiry date.** Sources are registered, dated, and re-reviewed on a cadence that CI enforces.
- **Fail closed.** Missing identity, missing evidence, or an unresolved match yields "verify first", not a confident answer.
- **Reproducible by default.** Locked dependencies, pinned actions, and audit plus lint plus typecheck plus tests on every change.

---

## Technology

Next.js · React · TypeScript · Node.js · Cloudflare Workers and D1 · Supabase · Drizzle ORM · Python · GitHub Actions

---

Repositories from 2019 to 2023, covering machine-learning coursework, tokens, and NFT contracts, are kept as historical reference.
