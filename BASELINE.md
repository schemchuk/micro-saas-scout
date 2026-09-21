# Research Baseline (v2 — patched per BASELINE_AUDIT.md)

This document synthesizes `CONTEXT.md`, `AGENTS.md`, `STRATEGY.md`, `LESSONS_FROM_V2.md`, `RESEARCH.md`, and `DECISION.md`, and incorporates the fixes accepted from `BASELINE_AUDIT.md`. It does not add new market facts, select a marketplace, or propose a niche. Where a statement is not a direct paraphrase of a project file, it is marked **[Interpretation]**. The full rationale for every change in this revision is in `BASELINE_PATCH.md`.

No market research has been performed to produce this document. `RESEARCH.md` and `DECISION.md` currently contain only their templates — zero candidates have been logged yet.

---

## 1. Project Objective

Per `CONTEXT.md` (unchanged from v1):

- Find and validate a micro-SaaS opportunity a **solo developer** can realistically launch and sell.
- Not primarily about "finding a niche." About finding a small, concrete business problem where: (1) people already spend time or money on it; (2) existing solutions are unsatisfactory, fragmented, expensive, or operationally painful; (3) a narrow product can solve it materially better; (4) there is a realistic path to discovery without cold outreach; (5) first paying customers can be reached before a large implementation effort.
- Operating constraints: solo developer, ~€0 research budget, near-zero validation budget, no cold outreach as the default acquisition method. Limited direct interaction for validation/interviews/support is allowed.
- Core question, verbatim: *"Where is there a repeated, monetized problem with visible dissatisfaction and a credible path from discovery to first payment?"*
- The prior project (`nishe_scout/`, confirmed present as a sibling directory) is archived; consultable, but its assumptions must not automatically govern this project.

---

## 2. Research Strategy

Unchanged from v1, per `STRATEGY.md` and `AGENTS.md`:

- **Strategic shift from `nishe_scout`:** inverts the old `marketplace → keyword sweep → competitor count → scoring → repeat` loop, starting from pain instead of a platform.
- **Central constraint:** no cold outreach — not "no marketing." Inbound channels only, and the channel must fit the problem.
- **Opportunity criteria** (STRATEGY.md): Problem, Buyer, Existing spending, Dissatisfaction, Wedge, Distribution, Payment, Feasibility — interesting when *most* are true, not when a score crosses a threshold.
- **Validation hierarchy** (strongest to weakest): actual payment → pre-order/deposit → strong request from identifiable buyer with clear existing spend → repeated comparison/switching evidence → repeated workaround behavior → repeated problem reports with buying context → search/discovery interest → general opinions/theoretical market size. A weaker signal cannot compensate for failure at a higher-order gate.
- **Process rules** (AGENTS.md): every research task resolves to one of the canonical decision states (§3 below); no open-ended phases; no scoring theater; timebox each hypothesis; stop researching a candidate the moment it fails a critical question.
- **Documentation discipline:** `RESEARCH.md` holds one record per candidate; `DECISION.md` exists "to prevent circular research." Killed hypotheses are not reopened without materially new evidence.

**What is not carried forward from `nishe_scout`** (LESSONS_FROM_V2.md, unchanged from v1): the Atlassian-first strategy, endless keyword sweeps, arbitrary scoring, competitor counts as standalone evidence, "the next phase will reveal the answer," unlimited "research first," the blanket claim that new marketplace vendors can't get organic discovery (a counterexample existed), and the opposite blanket claim that marketplace cold-start reliably works (the counterexample wasn't common/well-evidenced enough). **[Interpretation, unchanged]** The marketplace cold-start question stays a genuine unknown in both directions.

---

## 3. Candidate Status Vocabulary (canonical — resolves the v1 contradiction)

Two prior formulations conflicted: `AGENTS.md` §1 / `DECISION.md` used `KEEP / TEST / KILL / BLOCKED / INCONCLUSIVE`; `RESEARCH.md`'s template used `DISCOVERY / VALIDATION / KEEP / KILL / BLOCKED / INCONCLUSIVE` (no `TEST`, with `DISCOVERY`/`VALIDATION` undefined elsewhere).

**Resolution:** `AGENTS.md`/`DECISION.md` carry more normative weight — they are process rules, not a record template — so their vocabulary is canonical.

- **Decision states (the only vocabulary used for a candidate's standing at any gate or at the end of a research task):** `KEEP / TEST / KILL / BLOCKED / INCONCLUSIVE`, as defined in `DECISION.md`.
- **`DISCOVERY` is retained, but demoted to a lifecycle *phase* marker, not a decision state.** It means: "logged in `RESEARCH.md`, not yet evaluated against any gate." Every candidate starts in `DISCOVERY` and must receive a decision state (most immediately from the Payment Plausibility Gate, §6) before further evidence is gathered on it.
- **`VALIDATION` is retired as a status.** What it referred to — "a cheap commercial experiment is running" — is exactly what `TEST` already means in `DECISION.md`. Keeping both invited exactly the kind of silent divergence this reconciliation is meant to prevent.
- `RESEARCH.md`'s template `Status` line is updated to match (see `BASELINE_PATCH.md`, item 9).

This is the only status vocabulary used anywhere in this document, including for every new gate introduced below. No numeric scores, weights, or rankings are introduced anywhere in this revision.

---

## 4. Evidence Chain (canonical)

Three non-identical chain formulations existed in v1 (`STRATEGY.md`, `AGENTS.md` §3, and the original task brief). This revision adopts **one canonical chain**, built to preserve every distinction the audit found materially important:

```
Pain
 → Buyer (user ≠ budget owner, stated explicitly)
 → Existing spending (tiered — §5)
 → Existing solution (must be PAID — §7 Free-Incumbent Trap)
 → Payment Plausibility Gate (§6 — early, cheap, desk-research only)
 → Dissatisfaction (must tie to the paid solution above)
 → Switching intent
 → Switching feasibility (§8 — lock-in, procurement, contracts, alternative availability, switching destination)
 → Wedge
 → Distribution (§9 — operationalized, per-candidate)
 → Validation (payment-shaped experiment)
 → Build (execution — out of the research chain, unchanged from v1)
```

**Why stages are not merged, and why one is:**
- `Buyer`, `Existing spending`, `Existing solution`, `Dissatisfaction`, `Switching intent`, `Switching feasibility`, `Wedge`, `Distribution`, `Payment` (= the Payment Plausibility Gate), and `Validation` are each kept as distinct nodes because each answers a genuinely different question and none can substitute for another (STRATEGY.md's non-substitutability rule, extended).
- The **Free-Incumbent Trap is deliberately not a separate node.** It is a qualifying requirement on the *evidence accepted* at the `Existing solution` stage, not new sequential information — a free incumbent doesn't add a step, it disqualifies what would otherwise have passed that step. Giving it its own node would suggest it happens "after" existing-solution evidence is gathered, when in fact it changes what counts as evidence at that stage.
- **Source Classes A and B (§10) are not chain stages at all.** They are two parallel evidence-gathering streams that feed multiple stages (mainly Existing spending, Existing solution, Dissatisfaction, Switching intent). Treating them as sequential nodes would misrepresent them as a gate to pass rather than an input-diversification requirement.
- `Payment Plausibility` (early, category-level, desk research) and `Validation` (late, candidate-specific, real experiment) are kept as two separate nodes on purpose — per the audit, they answer different questions ("does anyone pay for this category of solution, from anyone" vs. "will this specific buyer pay us"), and collapsing them was the single biggest weakness identified (payment checked too late).

### Evidence table (updated stages only — unchanged stages keep their v1 definitions)

| Stage | Strong evidence | Weak evidence | Not evidence |
|---|---|---|---|
| **Pain** | Recurring, specific complaints (frequency/cost stated) from multiple independent people | A single anecdote calling something "annoying" | Researcher's own intuition |
| **Buyer** | Named role that experiences the pain **and** a named/identifiable role that can authorize payment, stated explicitly even when they are the same person | A guess at "who probably decides" | Assuming a large organization implies an accessible, self-serve buyer |
| **Existing spending** | See tiered standard, §5 | See tiered standard, §5 | See tiered standard, §5 |
| **Existing solution** | A named, **currently paid** competing product/process, confirmed via primary source | A free tool used as if it were "the solution" (see §7 — this now fails the stage, not just weakens it) | Absence of a dedicated tool read as a "gap" |
| **Payment Plausibility Gate** | See §6 | See §6 | See §6 |
| **Dissatisfaction** | Repeated complaints specifically about the paid solution identified above; documented comparison shopping | A single negative review; complaints about price from users who have never paid | Small review/install count of a competitor; complaints about a free tool with no paid solution in the picture |
| **Switching intent** | Direct accounts of migrating from tool A to tool B; explicit "we're evaluating replacing X because Y," with a stated outcome | A single "does anyone know an alternative to X" post | A feature request alone; a reliability complaint alone (motive for change, but also a trust barrier against an unknown small vendor — record both, don't collapse) |
| **Switching feasibility** | See §8 | See §8 | See §8 |
| **Wedge** | A specific, solo-buildable subset of the problem tied to a documented dissatisfaction that survived §8 | A vague idea with no link to a specific dissatisfaction | N/A — design decision |
| **Distribution** | See §9 | See §9 | See §9 |
| **Validation** | Actual payment, pre-order, or deposit | A waitlist **is no longer accepted as the terminal validation form** — see §6; it may still be used as an earlier, weaker signal | Social-media likes/upvotes alone |
| **Build** | N/A — execution | N/A | Starting before validation clears (AGENTS §6) |

**Feature requests vs. switching intent (unchanged from v1, still holds):** a feature request is strong evidence of dissatisfaction, not of switching intent. These remain separate concepts.

**Reliability complaints (new nuance from the audit):** a complaint about an incumbent's reliability is simultaneously (a) a strong motive for switching and (b) evidence *against* easy capture by an unknown small vendor, because if even the established player failed, buyers are likely to trust *another established player* more than a solo newcomer. Record both effects; do not treat it as unambiguously positive for the candidate.

---

## 5. Existing Spending — Tiered Standard (tightened per audit)

`STRATEGY.md`'s original definition ("money, labor, time, or workaround effort") is too broad to gate on directly. It is replaced with an explicit strength hierarchy. **A candidate needs at least one Strong-tier item to pass this stage; Medium/Weak tiers alone are insufficient.**

| Tier | Category | Minimum evidence required |
|---|---|---|
| **Strong** | Money paid for software/service with a visible price point | A recurring purchase decision exists (subscription, renewal) at an identifiable price |
| **Strong** | Contractor/freelancer expenditure | Evidence of actual invoices/engagements, not a one-off favor |
| **Medium** | Recurring internal labor / manual workaround (e.g., spreadsheet process) | Time cost **estimated by the affected person themselves**, not by the researcher, *and* some sign the person already tried to solve it with money (a paid template, a tool they evaluated, a job posting) |
| **Weak** | Internal scripts/tools built by the sufferer | Usually free labor with no buyer behind it; on its own, insufficient |
| **Not evidence** | Lost revenue / opportunity cost | This is a narrative, not observed behavior. **Excluded entirely as evidence for this stage.** |

**Rule:** if the only available evidence is "time" or a workaround, the stage does not pass unless there is also a sign of latent payment behavior (someone already tried to buy their way out of the problem). Time saved and lost revenue, asserted without this behavioral corroboration, do not satisfy Existing Spending.

---

## 6. Payment Plausibility Gate (new — moves payment earlier)

**Problem this closes:** the original chain checked willingness-to-pay last, after the most expensive research (dissatisfaction/switching mining) was already done. The riskiest assumption in the whole project — *will anyone pay an unknown solo vendor* — was tested last instead of first.

Placed **immediately after `Buyer` + `Existing spending` + `Existing solution`, before dissatisfaction mining begins.** This is desk research (checking public pricing pages and public purchase mentions), not a paid experiment — it stays inside the "~€0 research" budget from `CONTEXT.md`.

The gate distinguishes three questions that must not be collapsed into one:

1. **Is money spent anywhere in the category?** — Visible self-serve pricing: the category has at least a few paid options with published prices, sold self-serve (not exclusively via enterprise sales calls).
2. **Can the identified buyer purchase independently?** — Procurement mode: the buyer can decide and pay without a procurement process, security certification, or vendor-approval workflow gating the purchase. If the category's purchases are dominated by procurement, this directly triggers the existing `STRATEGY.md` hard veto on procurement-heavy/certification-dominated markets — this candidate should be **KILL**ed here, not carried forward on the strength of later dissatisfaction evidence.
3. **Is there precedent that this buyer type buys from small/unknown vendors?** — Some visible instance of this buyer type using or mentioning a small/lesser-known vendor's tool (not necessarily in this exact category).

**Decision rule (no scoring — qualitative, per-check):**
- Check 1 or 2 fails outright (no paid options exist at all in the category, or purchases are structurally procurement-gated) → **KILL**, consistent with the existing hard veto this reinforces.
- Check 3 is simply not found → **not a kill.** Absence of an observed small-vendor precedent is *unknown*, not disproof (same "absence ≠ negative evidence" principle applied at the Distribution stage, §9). Record as **BLOCKED/INCONCLUSIVE** pending evidence from Source Class B (§10), and do not proceed to expensive dissatisfaction mining until this is resolved one way or the other.
- All three checks pass → candidate may proceed to Dissatisfaction with status **DISCOVERY** still open, i.e. this gate clears the candidate for further (expensive) research, it does not itself grant `KEEP`.

**Consequence for Validation (§4 table):** the first real validation experiment must be **payment-shaped** — deposit, pre-order, or paid pilot. A waitlist alone answers "is this interesting?", which is rank 7 on the Validation Hierarchy, not "will you pay?", which is rank 1–2. `RESEARCH.md`'s "Validation experiment: cheapest test" field must specify a payment-shaped test; a waitlist-only plan does not satisfy the Validation stage.

---

## 7. Free-Incumbent Trap (new — closes a loophole, not a new universal rule)

v1's Dissatisfaction row said the existing solution is "**ideally** tied to a paid solution" — the word "ideally" made this optional. The audit is right that the project files do not support a blanket claim that free-incumbent problems are worthless (that would be inventing a new fact); what they do support is the existing, already-accepted principle that spending must be real and redirectable (`STRATEGY.md` Existing Spending criterion) and that a large theoretical/free user base is explicitly listed as *weak* evidence (`AGENTS.md` §4).

**Gate, stated precisely:** "the problem is connected to a paid ecosystem" is not sufficient by itself. If the buyer identified in the `Buyer` stage primarily uses a **free** incumbent and does not independently pay for anything addressing this problem, the `Existing solution` stage **fails** (not "weakens") unless there is clear, specific evidence of monetization the researcher can point to — e.g., the same buyer already pays for a paid add-on, a paid tier, or a paid third-party tool that plugs the same gap. Absent that, the candidate is **BLOCKED** at this stage, not carried into dissatisfaction mining on the strength of complaint volume alone.

This directly prevents the "FP1" pattern from the audit: a huge free incumbent, massive complaint volume, and a large waitlist, with no one who has ever paid for anything in the category.

---

## 8. Switching Feasibility & Switching Destination (new stage)

**Problem this closes:** "I want to leave X" was previously accepted as switching intent on its own. Wanting to switch and being able to switch are different claims.

Once Switching intent evidence exists, it must additionally be checked against:

- **Lock-in:** is data portable? Are there deep integrations that would need to be rebuilt?
- **Procurement/contractual constraints:** is the buyer free to choose a new vendor, or bound by a contract term, an internal approval process, or a compliance requirement?
- **Realistic alternative availability:** does a viable alternative exist at all, or is switching intent purely aspirational?

If switching is prohibitively difficult on any of these axes, the signal is **downgraded from "switching intent" back to "dissatisfaction"** — it still counts as dissatisfaction evidence, but it does not advance the candidate past this stage on its own.

**Switching destination check (new, required):** for any switching evidence used, record *where the switchers actually went*. If observed migrations consistently move between two or more already-entrenched incumbents, this must be recorded explicitly as a **distribution/entry risk**, not reinterpreted as an opportunity — churn existing in a category says nothing about whether a new, unknown, solo-built entrant can capture any of it. This directly closes the "FP3" pattern from the audit (real pain, real switching, but switchers only ever move between incumbents).

---

## 9. Distribution Evidence — Operationalized (tightened)

v1 already contained the concept "evidence of successful entry by a new/small vendor" but did not define an operational test for it. This revision defines one. A proposed distribution channel is **not accepted as distribution evidence** on the basis of general plausibility statements such as "SEO could work," "we could post on Reddit," "there is a marketplace," or "we could create content" — these remain explicitly insufficient, as in v1.

**A channel counts as distribution evidence for a specific candidate only if at least one of the following is true, recorded per-candidate (not assumed once for the whole project):**

1. An **observed case within the last 12 months** of a small/unknown vendor acquiring customers through that specific channel, with the mechanism identified (e.g., "found via this specific community thread," "found via this directory listing").
2. A **structurally newcomer-friendly channel mechanism**, with its rules verified from a reliable source — e.g., a marketplace's "new apps" feed, an integration directory with regular turnover, a template gallery that surfaces new entrants. "Structural" claims must cite where the mechanism/rules were verified, not be asserted from general familiarity with the platform.

In addition, before either of the above is accepted:
- The channel's actual rules must be checked (self-promotion bans, moderation posture, how ranking/surfacing works).
- A concrete, currently-live venue within the channel must be named (a specific community, a specific search query with visible current activity, a specific category) — not a category of channel in the abstract.

**Freshness applies here too:** evidence older than ~12 months is treated as historical, not current — see §11.

**Ordering rule (reinforces the non-substitutability principle already in v1):** a candidate must not receive `KEEP` on the strength of strong pain/dissatisfaction evidence while Distribution is still unverified. "Distribution unknown" is not the same as "distribution fine" — it must be recorded as an open gate, not silently passed.

---

## 10. Two Source Classes for Domain Discovery (new)

**Problem this closes:** relying only on public complaints as a discovery method systematically surfaces domains whose buyers post publicly (dev tools, marketing software, design tools) and systematically misses domains where the pain is real and paid but the buyers don't post (logistics, manufacturing, offline services, regulated industries, non-English-speaking markets). This is a sampling bias in the research method itself, not a fact about which domains have real problems.

**Two source classes must be used, not one:**

**A. Dissatisfaction / switching sources** (as in v1): reviews, comparison discussions, migration stories, public complaints, communities.

**B. Spending / behavioral sources** (new): visible pricing pages, hiring demand (job postings describing recurring operational work), recurring contractor/freelancer demand, procurement/tender evidence where accessible, paid template/service marketplaces, and other observable evidence that money or dedicated labor is already allocated to the problem.

The purpose of Class B is **not** to search everything — it is to prevent the specific failure of turning "no public complaints found" into "no problem exists." **Explicit rule: absence of public complaints (Class A) = unknown, not negative evidence.** A quiet domain must not be killed for lack of complaint volume alone; it must be checked against Class B before any decision is recorded.

**Required per-candidate note:** for every candidate sourced primarily from Class A, record whether the buyer is someone who posts publicly at all. If not, treat all Class A signal strength for that candidate as provisional and actively seek Class B corroboration before weighting it.

---

## 11. Signal Freshness & Source Hygiene (new)

For every piece of evidence recorded as important to a decision, record:

- **Source date** (when the underlying content was published/posted).
- **Observation date**, if different from source date.
- **Primary or secondary** (the affected person's own account, vs. a summary/aggregator/consultant account).
- **Independence** — is this a genuinely separate source, or the same complaint cross-posted or syndicated across multiple pages? Count independent sources, not page count or mention count.
- **Freshness** — behavioral signals older than roughly 12 months are marked **stale** and are not treated as current evidence of an ongoing problem (a complaint about an issue the vendor fixed a year ago should not still be counted).
- **Derivation check** — note if multiple pages appear to derive from the same underlying source (e.g., syndicated content, scraped/rewritten "alternative to X" pages); these do not count as multiple independent signals.

**"Alternative to X" pages, specifically:** treated as **lead sources only** — evidence that an SEO/affiliate operator believes there's search volume for this query — not as evidence of buyer demand or switching behavior, unless independently corroborated by a primary community or first-person source.

---

## 12. Domain-Selection Rule — Do Not Overfit to Loud Domains (new)

Explicit rule, to counter the bias introduced by Class A sourcing alone (§10):

- **Public complaint volume is not a proxy for market attractiveness.**
- A domain with few public complaints but strong Existing Spending / Payment Plausibility evidence (§5, §6) **remains eligible** — it is not penalized for being quiet.
- A domain with many public complaints but weak spending/payment evidence **remains unproven** (`INCONCLUSIVE`, not `KEEP`) — complaint volume alone does not clear the Existing Spending or Payment Plausibility gates.

---

## 13. Hard Veto Gates (unchanged structure, cross-referenced to new gates)

Three distinct strengths, still not to be collapsed into one:

**True vetoes (avoid unless evidence is exceptional)** — `STRATEGY.md` business-model boundaries: large outbound sales teams; enterprise products with long procurement cycles; markets where trust/security certification dominates initial sales; generic AI wrappers with no differentiated workflow; ad-budget-dependent economics; ideas a major platform could trivially ship natively. **The Payment Plausibility Gate (§6, check 2) and the Free-Incumbent Trap (§7) are earlier, cheaper operationalizations of these same underlying vetoes** — they let a candidate fail this class of problem before expensive research, rather than only at the end.

**Risk flag, explicitly not a veto** — `AGENTS.md` §10 support-heavy products (24/7 expectations, complex integrations, disproportionate compliance burden, frequent per-customer config, high-touch onboarding, difficult migration). Stated plainly in the source: "not an automatic rejection... a major risk."

**Process-level stop rules:** the `DECISION.md` Global stop rule (repeated failure across candidates → change a strategic assumption, don't just search more); no reopening `KILL` without materially new evidence; no premature building (AGENTS §6); no scoring theater (AGENTS §7) — reaffirmed: nothing in this revision introduces scores, weights, or rankings.

---

## 14. Research Failure Modes (extended)

**Carried forward from v1 (unchanged):**
1. Mistaking low competition for opportunity.
2. Reading an empty marketplace/category as proof of demand.
3. Treating complaints as willingness to pay.
4. Treating one positive review, or a competitor's low review/install count, as proof of an accessible market.
5. Confusing feature requests with switching intent.
6. Assuming marketplace search visibility equals new-vendor discoverability.
7. Using vendor marketing claims as independent evidence.
8. Assuming app/listing counts prove market size.
9. Prematurely selecting a platform or marketplace.
10. Starting from a product idea and searching for justifying evidence.
11. Collapsing a platform-native feature gap with a durable wedge.
12. Data-collection method failure (static fetch against client-rendered UIs).
13. Generalizing a domain-specific kill reason into a universal claim.
14. Manufacturing false precision with scoring systems.
15. Letting an unresolved candidate justify another open-ended research phase.
16. Reopening a `KILL` without new evidence, or discarding new evidence because a similar idea was killed before.

**New, from `BASELINE_AUDIT.md`:**
17. **Vocal-minority bias** — complaint volume scales with the incumbent's total user base, not with market accessibility to a newcomer; the loudest domains are often the ones whose market a solo vendor can least reach.
18. **Non-buyer voices** — free-tier users, students, and hobbyists complain the loudest and never convert to paying customers.
19. **SEO-manufactured demand** — an "alternative to X" page's existence proves an SEO operator's interest in that query, not buyer switching behavior (see §11).
20. **Affiliate distortion** — comparison sites rank by commission; a "top 10 alternatives" listing is not evidence of real switching.
21. **Survivorship bias in migration stories** — successful migrations are the ones that get written up (often by the winning vendor or a consultant selling migrations); abandoned or failed switching attempts are invisible, systematically overstating how easy switching is.
22. **Recency decay** — stale complaints about long-fixed issues remain indexed and searchable; treating them as current evidence overstates present dissatisfaction (see §11 freshness rule).
23. **Enterprise/SMB mismatch** — enterprise-user complaints do not imply solo/SMB willingness to pay self-serve.
24. **Platform effects on visibility** — community moderation rules, self-promo bans, and platform ranking shape which discussions are even visible, independent of the underlying problem's real prevalence.
25. **False independence from cross-posting** — the same complaint posted in three communities is one signal, not three (see §11).
26. **Geography/language bias** — English-language-source-only research makes non-English-speaking markets systematically invisible, even where the underlying pain and spending are real.
27. **Domain-selection bias toward loud domains** — see §10/§12; relying only on Class A sources systematically favors domains whose buyers already post publicly.

---

## 15. Current Unknowns (updated)

Resolved since v1 (see `BASELINE_PATCH.md` for detail): the status-vocabulary contradiction (§3) and the chain-formulation contradiction (§4) are now reconciled.

Still genuinely open:
- No candidate, problem area, marketplace, or niche has been selected. `RESEARCH.md` and `DECISION.md` remain at zero logged candidates/decisions.
- Whether the `nishe_scout/` archive contains reusable evidence outside its Atlassian-specific focus has not been assessed.
- The marketplace cold-start question remains genuinely open in both directions — not resolved by this revision, and not claimed to be.
- Whether any specific domain will actually clear the new Payment Plausibility Gate or Free-Incumbent Trap is, by design, unknown until real domains are examined — this baseline intentionally does not pre-judge that.

---

## 16. Recommended Next Research Question

The v1 question targeted dissatisfaction/switching sources only, domain-agnostically, with a research-method verification requirement — directionally correct per the audit, but missing four things: a requirement that surfaced signals concern a *paid* incumbent with *switching feasibility* checked, a non-complaint (Class B) source requirement, a per-domain distribution note, and a freshness requirement. This revision folds in all four.

**Revised next question:**

> Using two parallel source classes — (A) dissatisfaction/switching sources: reviews, comparison discussions, migration stories, public complaints, communities; and (B) spending/behavioral sources: visible pricing, hiring demand, recurring contractor/freelancer demand, procurement/tender evidence where accessible, and other observable evidence of money or dedicated labor already allocated to a problem — what repeatable and verifiable method can surface a set of candidate problem domains where: the incumbent solution is demonstrably **paid** (not free), the switching/dissatisfaction signals found are no older than ~12 months, and each surfaced domain carries a first-pass note on which channel a problem-aware buyer might discover a new entrant through (without yet verifying that channel per §9)?
>
> For each surfaced domain, record: source class(es) used, whether the buyer segment posts publicly at all, and source dates — but do **not** run the Payment Plausibility Gate, Switching Feasibility check, or Distribution verification yet. Those apply per-candidate once a specific domain is selected for deeper research, not during this discovery pass.

This keeps the discovery pass cheap and domain-agnostic (no niche or marketplace is named), while making sure its raw output isn't pre-contaminated by free-incumbent noise, stale signals, or single-source-class bias — the specific failure modes (§14, items 17–27) that would otherwise resurface at the next gate anyway, just later and more expensively.

---

## BASELINE CONFIDENCE

**Well established:**
- Project objective and its rejection of "low-competition niche" as the goal.
- The no-cold-outreach constraint and allowed-channel list.
- The ten-node canonical evidence chain (§4) and its non-substitutability principle.
- The three-tier veto structure (true veto / risk flag / process stop-rule), now including the Payment Plausibility Gate and Free-Incumbent Trap as early operationalizations of the existing true vetoes.
- The Existing Spending tiered standard (§5) and the exclusion of lost revenue/opportunity cost as evidence.
- The canonical status vocabulary (§3): `DISCOVERY` (phase) plus `KEEP/TEST/KILL/BLOCKED/INCONCLUSIVE` (decisions), with no scoring anywhere.
- The extended failure-mode list (§14), directly traceable to either the original project files or the audit's abstract false-positive walkthroughs.
- Current project state: zero candidates or decisions logged yet.

**Remains uncertain (deliberately, not by omission):**
- Whether marketplace-based distribution is viable for a cold-start solo vendor — still unresolved in both directions.
- Whether the `nishe_scout` archive holds any transferable evidence outside Atlassian.
- Whether any real domain will clear the Payment Plausibility Gate or the Free-Incumbent Trap — untestable without doing the market research this document deliberately does not perform.

**Must be verified before market research proceeds:**
- Confirm `RESEARCH.md`'s `Status` field has been updated to match §3 (done as part of this patch — see `BASELINE_PATCH.md`).
- Record acceptance of the revised next research question (§16) as a `DECISION.md` entry before any source is queried.
- When sources for the next research question are client-rendered, verify the research method actually observes what a human sees, per the LESSONS_FROM_V2 research-method lesson, before trusting the output.
