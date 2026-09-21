# Research Baseline

This document is a synthesis of `CONTEXT.md`, `AGENTS.md`, `STRATEGY.md`, `LESSONS_FROM_V2.md`, `RESEARCH.md`, and `DECISION.md` as they exist today. It does not add new facts, select a marketplace, or propose a niche. Where a statement is not a direct paraphrase of a project file, it is marked **[Interpretation]**.

No market research has been performed to produce this document. `RESEARCH.md` and `DECISION.md` currently contain only their templates — zero candidates have been logged yet. This is itself a fact about project state, not an interpretation.

---

## 1. Project Objective

Per `CONTEXT.md`:

- Find and validate a micro-SaaS opportunity a **solo developer** can realistically launch and sell.
- The project is explicitly **not** primarily about "finding a niche." It is about finding a small, concrete business problem where:
  1. people already spend time or money on the problem;
  2. existing solutions are unsatisfactory, fragmented, expensive, or operationally painful;
  3. a narrow product can solve the problem materially better;
  4. there is a realistic path to discovery without cold outreach;
  5. first paying customers can be reached before a large implementation effort.
- Operating constraints: solo developer, ~€0 research budget, near-zero validation budget, **no cold outreach as the default acquisition method** (inbound/organic discovery is required, though limited direct interaction for validation/interviews/support is allowed).
- Core question, verbatim: *"Where is there a repeated, monetized problem with visible dissatisfaction and a credible path from discovery to first payment?"* — explicitly **not** "what niche has low competition?"
- The prior project (`nishe_scout/`, confirmed to exist as a sibling directory) is archived. Its research may be consulted, but **its assumptions must not automatically govern this project.**

---

## 2. Research Strategy

Per `STRATEGY.md` and `AGENTS.md`:

- **Strategic shift from `nishe_scout`:** that project ran `marketplace → keyword sweep → competitor count → scoring → repeat`. This project inverts the starting point: `Pain → Existing spending → Existing solution → Dissatisfaction → Wedge → Distribution → Validation → Build`.
- **Central constraint:** no cold outreach — not "no marketing." Inbound channels (search/SEO, communities, directories, comparison pages, educational content, public tools, launch platforms, ecosystem/integration discovery, non-mass referral) are allowed, but the channel must fit the problem; a channel is not chosen merely because it's available.
- **Opportunity criteria** (STRATEGY.md): Problem, Buyer, Existing spending, Dissatisfaction, Wedge, Distribution, Payment, Feasibility — a candidate becomes interesting when *most* of these are true, not when a score crosses a threshold.
- **Validation hierarchy** (strongest to weakest, STRATEGY.md): actual payment → pre-order/deposit → strong request from identifiable buyer with clear existing spend → repeated comparison/switching evidence → repeated workaround behavior → repeated problem reports with buying context → search/discovery interest → general opinions/theoretical market size. A weaker signal cannot compensate for failure at a higher-order gate.
- **Process rules** (AGENTS.md): every research task must resolve to KEEP/TEST/KILL/BLOCKED/INCONCLUSIVE; no open-ended phases; no scoring theater; timebox each hypothesis against 5 quick questions (real pain? willingness to pay? solo-buildable? discoverable without cold outreach? cheaply testable?); stop researching a candidate the moment it fails a critical question.
- **Documentation discipline:** `RESEARCH.md` holds one compact record per candidate (problem/buyer/existing solution/spending/dissatisfaction/wedge/distribution/payment evidence/feasibility/support risk/validation experiment/evidence with source+observation+interpretation/decision). `DECISION.md` is a decision log whose stated purpose is **"to prevent circular research"** — each entry records the specific question being decided, evidence, reasoning, and next action (or "Stop"). Killed hypotheses are not reopened without materially new evidence.

### What has been explicitly rejected / ruled out

From `LESSONS_FROM_V2.md`, the following are **not carried forward as valid methodology or as facts**:
- The Atlassian-Marketplace-first strategy as a starting point.
- Endless keyword sweeps.
- Arbitrary/weighted scoring systems.
- Competitor counts used as standalone evidence of opportunity.
- The assumption that "the next research phase will reveal the answer."
- "Research first, build later" treated as an unlimited process.
- The claim that first-time/single-app marketplace vendors *cannot* achieve organic discovery — a counterexample was observed in v2, so this blanket claim is false.
- The opposite claim, that marketplace cold-start distribution *reliably works* — the counterexample was not common or well-evidenced enough to establish this either.
- Static/non-browser scraping results for client-side-rendered marketplace search — v2 found these can be misleading (identical results returned for different queries).

**[Interpretation]** The net effect of the marketplace lesson is a genuine unknown, not a resolved fact in either direction: marketplace cold-start entry is neither proven impossible nor proven viable. Any future research must test the actual acquisition path rather than assume either extreme.

---

## 3. Evidence Chain

The task specifies this chain: `Pain → Existing expenditure/workaround → Existing solution → Dissatisfaction → Switching/replacement signal → Narrow wedge → Organic distribution path → Validation → Build`.

**Note on chain variants:** the project files contain three related but non-identical formulations of this chain — `STRATEGY.md` (`Pain → Existing spending → Existing solution → Dissatisfaction → Wedge → Distribution → Validation → Build`), `AGENTS.md` §3 (`Problem → Buyer → Existing spending/effort → Existing solution → Observable dissatisfaction → Product wedge → Discovery channel → First payment`), and the one requested above. They describe the same underlying process but differ in node count and endpoint (some end at "Build," `AGENTS.md` ends at "First payment," and `AGENTS.md` is the only one to make "Buyer" an explicit node). This is flagged under Contradictions below rather than silently merged.

| Stage | Strong evidence | Weak evidence | Not evidence |
|---|---|---|---|
| **Pain** | Recurring, specific complaints (frequency/cost stated) from multiple independent people | A single anecdote calling something "annoying" | Researcher's own intuition that a workflow "must" be painful |
| **Existing expenditure / workaround** | Identifiable amount currently paid, or a documented recurring manual workaround (spreadsheet, contractor, script) with real time cost | "I wish there were a tool for this," with no indication of current spend/effort | A large theoretical market-size figure |
| **Existing solution** | A named competing product/process, confirmed via primary source (product page, user statement, review) | Assuming a solution category exists because it's plausible | Absence of a dedicated tool, read as a "gap" (AGENTS §2 explicitly bars this move) |
| **Dissatisfaction** | Repeated complaints specifically about an existing **paid** solution; documented comparison shopping | A single negative review | Small review/install count of a competitor (explicitly barred, AGENTS §2 and §4) |
| **Switching / replacement signal** | Direct accounts of migrating from tool A to tool B; explicit "we're looking to replace X because Y" | A single "does anyone know an alternative to X" post | A feature request alone — see distinction below |
| **Narrow wedge** | A specific, solo-buildable subset of the problem that maps directly onto a documented dissatisfaction | A vague "AI wrapper" or "dashboard" idea with no link to a specific dissatisfaction | N/A — this is a design decision, not a claim that needs external evidence |
| **Organic distribution path** | A named channel where problem-aware buyers already search/gather, *plus* some indication an unknown/small vendor can get discovered there | "We could do SEO," asserted with no evidence anyone searches for this | Marketplace category listing existing, read as proof of discoverability (LESSONS_FROM_V2 marketplace lesson); app/listing counts read as market-size proof |
| **Validation** | Actual payment, pre-order, or deposit | Waitlist signups, "I would pay for that" statements | Social-media likes/upvotes alone |
| **Build** | N/A — execution stage | N/A | Beginning here before validation gates clear is itself a rule violation (AGENTS §6) |

**On feature requests vs. switching intent [Interpretation, resolving an apparent tension]:** `AGENTS.md` §4 lists "clear requests for a missing capability" as strong evidence in general, while the task brief separately warns against "confusing feature requests with switching intent." Read together: a feature request is strong evidence of *dissatisfaction* (someone is unhappy enough with the status quo to ask for change), but it is **not**, by itself, evidence of *switching intent* (willingness to leave the current vendor). Treating a feature request as proof someone will switch products collapses two different stages of the chain into one and should not be done.

---

## 4. Evidence Standards

### Concept glossary (per the task's explicit instruction not to collapse these)

- **Competition** — the number/maturity of existing vendors serving a problem. On its own, says nothing about demand in either direction. `AGENTS.md` §2 explicitly bars treating low competition as proof of demand.
- **Demand** — people wanting the problem solved. Distinguished from *existing spending*: wanting something solved is not the same as currently paying or working around it.
- **Existing spending** — money, labor, time, or workaround effort *currently* allocated to the problem. This is the first hard behavioral filter in the chain (STRATEGY.md's Opportunity Criteria).
- **Dissatisfaction** — observable unhappiness with the *current* approach to the problem, ideally tied to a paid solution.
- **Switching intent** — a stated or observed willingness to move from the current solution to an alternative. Stronger than dissatisfaction alone; a subset of the Validation Hierarchy's "repeated direct evidence of comparison or switching" (rank 4).
- **Distribution** — the mechanism by which problem-aware buyers can find the product without cold outreach. `AGENTS.md` §3 makes this a required part of every hypothesis, not an afterthought.
- **Evidence of successful entry by a new/small vendor** — direct evidence that an unknown vendor specifically (not an established player) can acquire customers through the proposed channel. `LESSONS_FROM_V2.md` is explicit that this is different from, and not proven by, the channel simply existing or being searchable.

These seven concepts are treated in the project files as independently necessary and non-substitutable — strength on one does not compensate for absence of another (STRATEGY.md: "A weaker signal cannot compensate for failure at a higher-order gate").

### Fact/interpretation discipline (AGENTS §8)

For every important claim recorded during research: state the observed fact, name the source, separate inference from the source's own statement, and record uncertainty. A source's opinion must never be promoted to an established fact.

---

## 5. Hard Veto Gates

The project files distinguish gates of different strength. Collapsing them would violate the task's own instruction to keep concepts separate.

**True vetoes (avoid unless evidence is exceptional)** — `STRATEGY.md`, Business-model boundaries:
- Products requiring large outbound sales teams.
- Enterprise products with long procurement cycles.
- Markets where trust/security certification dominates initial sales.
- Generic AI wrappers with no differentiated workflow.
- Economics that depend on large paid-ad budgets.
- Ideas a major platform could trivially ship natively as a feature.

**Explicitly *not* a hard veto — a risk flag** — `AGENTS.md` §10, support-heavy products (24/7 operational expectations, complex integrations, disproportionate compliance burden, frequent per-customer configuration, high-touch onboarding, difficult migration work). The source text states plainly: *"This is not an automatic rejection, but it is a major risk for a solo developer."* It must not be treated as equivalent to the business-model boundaries above.

**Process-level stop rules (govern the research process itself, not candidate selection):**
- `DECISION.md` Global stop rule: if research repeatedly shows no candidate satisfies `pain + buyer + money + dissatisfaction + wedge + distribution`, the response is to change a strategic assumption — not to run more searches.
- Killed hypotheses (`KILL` decisions) are not reopened absent materially new evidence (AGENTS §9, DECISION.md).
- No premature building: no production code, full architecture, or polished MVP before a hypothesis survives validation (AGENTS §6).
- No scoring theater: explicit evidence and hard gates only, no weighted scores (AGENTS §7).

---

## 6. Research Failure Modes

Modes explicitly named or directly implied by the project files:

1. **Mistaking low competition for opportunity** (AGENTS §2, LESSONS_FROM_V2).
2. **Reading an empty marketplace/category as proof of demand** — the absence-of-tool trap (AGENTS §2 combined with the marketplace lesson).
3. **Treating complaints as willingness to pay** — complaints about a paid tool are strong evidence of *dissatisfaction*, not automatically of a *new vendor's* ability to capture the switch.
4. **Treating one positive review, or a competitor's low review/install count, as proof of an accessible market** (AGENTS §4 explicit; LESSONS_FROM_V2 explicit).
5. **Confusing feature requests with switching intent** — see the glossary distinction above.
6. **Assuming marketplace search visibility equals new-vendor discoverability** — LESSONS_FROM_V2's central marketplace lesson.
7. **Using vendor marketing claims as independent evidence** — violates the fact/interpretation discipline (AGENTS §8) and RESEARCH.md's preference for primary sources and direct customer behavior over summaries/opinion.
8. **Assuming app/listing counts prove market size** — explicitly rejected as a success criterion (DECISION.md: a large list of niches or many competitor profiles does not equal project success).
9. **Prematurely selecting a platform or marketplace** before confirming the marketplace itself is the proposed distribution channel (AGENTS §2).
10. **Starting from a product idea and searching for justifying evidence** — the inverse of the entire strategic shift described in `STRATEGY.md` and `CONTEXT.md`'s "core question" framing.
11. **Collapsing a platform-native feature gap with a durable wedge** — STRATEGY.md's veto against ideas a major platform can ship natively.
12. **Data-collection method failure** — using static/non-browser fetching against client-rendered marketplace search UIs and treating the (possibly identical/misleading) output as real data (LESSONS_FROM_V2's research-method lesson).
13. **Generalizing a domain-specific kill reason** (e.g., an Atlassian-specific reason a wedge failed) into a universal claim about all marketplaces or domains.
14. **Manufacturing false precision with scoring systems** instead of explicit evidence and hard gates (AGENTS §7).
15. **Letting an unresolved candidate justify another open-ended research phase** rather than stopping per the timebox rule (AGENTS §5, LESSONS_FROM_V2 strategic lesson).
16. **[Interpretation, additional]** Reopening a `KILL`ed hypothesis on the same evidence that killed it, or, conversely, discarding a genuinely new signal because a superficially similar idea was killed previously — both violate AGENTS §9/DECISION.md's reopening rule in opposite directions.

---

## 7. Current Unknowns

- No candidate, problem area, marketplace, or niche has been selected. `RESEARCH.md` and `DECISION.md` contain only their templates — zero logged candidates or decisions exist as of this baseline.
- Whether the `nishe_scout/` archive (confirmed present as a sibling directory) contains reusable evidence outside its Atlassian-specific focus has not been assessed in this baseline.
- The marketplace cold-start question remains genuinely open in both directions (see §2 above) — not evidence either that marketplace channels work or that they don't.
- **Terminology inconsistency [flagged, not resolved]:** `RESEARCH.md`'s candidate `Status` field uses `DISCOVERY / VALIDATION / KEEP / KILL / BLOCKED / INCONCLUSIVE`, while `AGENTS.md` §1 and `DECISION.md`'s decision states use `KEEP / TEST / KILL / BLOCKED / INCONCLUSIVE`. `RESEARCH.md` has no `TEST` state and introduces `DISCOVERY`/`VALIDATION` as pre-decision states not defined anywhere else. It is not stated in the files whether `VALIDATION` (RESEARCH.md) and `TEST` (AGENTS.md/DECISION.md) are meant to be the same state under different names. This should be reconciled before candidates start moving through the pipeline, to avoid inconsistent status tracking.
- The three evidence-chain formulations (§3 above) are not literally identical across files; it is not stated whether this is intentional (different granularity for different purposes) or drift.

---

## 8. Recommended Next Research Question

Not a niche, and not a marketplace selection. Per the strategic shift, the chain's weakest-evidenced and most differentiating stage relative to `nishe_scout`'s methodology is **dissatisfaction → switching signal**, combined with the unresolved **method-validity** lesson (§ "Research-method lesson," LESSONS_FROM_V2).

**Proposed next question:**

> Across general-purpose sources where buyers describe abandoning or wanting to abandon a *paid* tool they currently use (e.g., review platforms with "switched from" data, "alternative to X" community threads, public churn/complaint discussions), what repeatable and *verifiable* method can surface multiple candidate problem domains — so that domain selection is driven by observed switching/dissatisfaction behavior, rather than by picking a marketplace or product category first?

This question:
- targets existing spending + existing solution + dissatisfaction + switching signal directly, the stages the old methodology skipped;
- stays domain-agnostic — it does not commit to a marketplace, platform, or niche;
- has a built-in check against LESSONS_FROM_V2's research-method lesson, by requiring the method itself to be verified (e.g., confirming a source isn't client-rendered in a way that produces misleading static-fetch results) before it's used to generate candidates;
- produces an output (a short list of dissatisfaction/switching signals with sources) that can be logged as `DISCOVERY`/candidate entries in `RESEARCH.md` without yet requiring a KEEP/TEST/KILL decision on any specific niche.

---

## BASELINE CONFIDENCE

**Well established (directly stated in project files, low ambiguity):**
- The project's objective and its explicit rejection of "find a low-competition niche" as the goal.
- The no-cold-outreach constraint and the allowed-channel list.
- The core evidence chain concept and the seven-concept glossary (competition/demand/spending/dissatisfaction/switching/distribution/new-vendor-entry-evidence) as independently necessary, non-substitutable signals.
- The business-model hard vetoes and their "unless evidence is exceptional" override clause.
- The support-heavy risk flag being explicitly *not* an automatic veto.
- The failure modes drawn directly from `nishe_scout`'s documented experience.
- Current project state: zero candidates or decisions logged yet.

**Remains uncertain:**
- Whether marketplace-based distribution is viable for a cold-start solo vendor — genuinely unresolved in the source files, not just unresearched by this baseline.
- Whether `RESEARCH.md`'s `VALIDATION`/`DISCOVERY` statuses are synonymous with `AGENTS.md`/`DECISION.md`'s `TEST` state, or represent an intentionally finer-grained pipeline.
- Whether the `nishe_scout` archive contains any evidence transferable outside its original Atlassian-specific scope.

**Must be verified before market research proceeds:**
- Reconcile the status vocabulary between `RESEARCH.md` and `AGENTS.md`/`DECISION.md` so candidates are logged consistently.
- Decide (and record as a `DECISION.md` entry) whether the next research question above is accepted as stated, before any source is queried.
- If any source used to answer the next research question is client-side rendered, confirm the research method actually observes the same data a human user would see, per the LESSONS_FROM_V2 research-method lesson, before trusting its output.
