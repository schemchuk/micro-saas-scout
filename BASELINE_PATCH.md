# Baseline Patch Log

This document records what changed in `BASELINE.md` in response to `BASELINE_AUDIT.md`, why, and the effect on the research process. No market research was performed to produce this patch; no niche, marketplace, or product was selected or implied.

Format per item: **Audit finding → Change made → Reason → Effect on research process**, followed by a verdict (`ACCEPTED` / `MODIFIED` / `REJECTED`) with a short justification tied back to the original project files.

---

## 1. Payment Plausibility Gate

**Audit finding:** payment was checked last in the chain, after the most expensive research (dissatisfaction/switching mining) was already done. The riskiest assumption in the project — will anyone pay an unknown solo vendor — was tested last instead of first.

**Change made:** added a new gate (`BASELINE.md` §6) placed immediately after `Buyer` + `Existing spending` + `Existing solution`, before dissatisfaction mining. Three separately-recorded checks: (1) visible self-serve pricing exists in the category, (2) the buyer can purchase independently without procurement/certification gating, (3) precedent exists that this buyer type buys from small/unknown vendors. Check 1/2 failing → `KILL`. Check 3 absent → `BLOCKED/INCONCLUSIVE`, not `KILL` (absence isn't disproof).

**Reason:** `STRATEGY.md` already vetoes procurement-heavy/certification-dominated markets and lists "actual payment" as the strongest validation signal; this gate is a cheap, early, desk-research-only application of an assumption the project already holds, applied before the expensive stages instead of after them. It does not add a new business-model rule — it operationalizes existing ones earlier.

**Effect on research process:** a candidate can now be killed or blocked cheaply before any complaint-mining time is spent on it. The riskiest assumption is tested first, per the audit's cheap-falsification principle, which is itself consistent with `AGENTS.md` §5's timeboxing rule.

**Audit's 3-part proposal (self-serve pricing / independent buyer / small-vendor precedent) — evaluated against source files:**

- **ACCEPTED, with one modification.** Checks 1 and 2 are accepted as stated and tied directly to `STRATEGY.md`'s existing procurement/certification veto — well justified, not a new fact. Check 3 is accepted but **downgraded in consequence**: the audit's proposal did not specify what happens when no precedent is found; treating "not found" as an automatic fail would contradict the baseline's own "absence of public complaints = unknown" principle (§10) applied elsewhere, so this patch applies that same principle to check 3 (`BLOCKED/INCONCLUSIVE`, not `KILL`) for internal consistency.

---

## 2. Existing Spending — Tightened

**Audit finding:** `STRATEGY.md`'s definition ("money, labor, time, or workaround effort") is too broad; "time saved" and "lost revenue," asserted without behavioral corroboration, were being treated as equivalent to actual payments.

**Change made:** `BASELINE.md` §5 replaces the single definition with a five-tier hierarchy (paid software → contractor/freelancer spend → internal labor/workaround with self-estimated cost + latent payment behavior → internal scripts → lost revenue/opportunity cost, the last explicitly excluded as evidence). A candidate needs at least one Strong-tier item to pass.

**Reason:** the four categories the audit distinguishes are not equally strong evidence of a redirectable budget, and `STRATEGY.md` itself only ever names "actual payment" and "pre-order/deposit" as the top of its validation hierarchy — collapsing all four into one "existing spending" bucket contradicted the project's own stated preference ordering.

**Effect on research process:** "we spent time on this" or "this costs the business money" no longer passes the Existing Spending gate by itself; it requires either real money already changing hands, or a specific sign that the affected person already tried to pay their way out of the problem.

**Verdict: ACCEPTED.** The audit's hierarchy is a direct, consistent extension of `STRATEGY.md`'s already-stated validation hierarchy; no new fact was invented, only an existing preference ordering made explicit at an earlier gate.

---

## 3. Switching Feasibility

**Audit finding:** "I want to leave X" was accepted as switching intent without checking whether leaving was actually possible (lock-in, procurement, contracts, alternative availability). Also, the chain never asked where switchers actually go.

**Change made:** new gate (`BASELINE.md` §8) between Switching intent and Wedge. Checks lock-in/data portability, integration rebuild cost, procurement/contractual constraints, and realistic alternative availability. Signals that fail this check are downgraded from "switching intent" back to "dissatisfaction" rather than discarded. Added a required "switching destination" note: if observed switchers move only between entrenched incumbents, this is recorded as a distribution/entry risk, not an opportunity.

**Reason:** `AGENTS.md` §3 already requires a "credible discovery mechanism" and a full problem→payment chain per candidate; a switching signal that can't actually be acted on, or that only benefits other incumbents, does not satisfy that requirement even though it looks like strong evidence on the surface.

**Effect on research process:** switching evidence is now split into two questions (willingness and feasibility) that must both be answered, and every switching signal must be accompanied by a note on where the switch actually led.

**Verdict: ACCEPTED.** Directly closes a gap in `AGENTS.md` §3's existing requirement that a candidate identify a full, credible chain to payment — not a new principle, an unenforced part of an existing one.

---

## 4. Free-Incumbent Trap

**Audit finding:** the Dissatisfaction stage said an existing solution is "ideally" paid — an optional qualifier that let free-incumbent domains (huge complaint volume, no one who has ever paid) pass every stage up through Wedge before the missing budget became apparent.

**Change made:** `BASELINE.md` §7. "Existing solution" now requires the buyer to be someone who independently pays for something addressing the problem; a free incumbent alone fails this stage (not just weakens it) unless there's specific evidence of adjacent monetization (a paid tier, paid add-on, or paid third-party tool the same buyer already uses).

**Reason:** the audit is explicit that the project files do not support inventing a blanket "free incumbents are always worthless" rule, and this patch does not add one. It instead removes the word "ideally," aligning the Dissatisfaction/Existing-solution stages with two rules the project files already state: `AGENTS.md` §4 lists "a large theoretical market" as weak evidence, and `STRATEGY.md`'s Existing Spending criterion already requires money that can be redirected — a free incumbent has no such money by definition, unless shown otherwise.

**Effect on research process:** a domain dominated by a free incumbent no longer advances past the Existing Solution stage on complaint volume alone; it stalls at `BLOCKED` until specific monetization evidence is found.

**Verdict: ACCEPTED, precisely scoped.** The audit itself warns against inventing a universal rule the files don't support; this patch implements the gate exactly as scoped in the audit (a requirement, not a blanket domain disqualification) and no more broadly.

---

## 5. Second Source Class for Domain Discovery

**Audit finding:** relying only on public-complaint sources (Class A) systematically favors domains whose buyers post publicly and systematically misses domains where pain is real but buyers don't post (offline/regulated/non-English-speaking markets). "No public complaints found" was at risk of silently becoming "no problem exists."

**Change made:** `BASELINE.md` §10 formally defines two parallel source classes — A (reviews, comparisons, migration stories, complaints, communities) and B (pricing, hiring demand, contractor/freelancer demand, procurement/tender evidence, other observable spend/labor allocation) — and states explicitly: **absence of Class A evidence = unknown, not negative evidence.** Also requires a per-candidate note on whether the buyer segment posts publicly at all.

**Reason:** nothing in the project files privileges public complaints as the only valid evidence type — `AGENTS.md` §4's "strong evidence" list already includes non-complaint items like "recurring operational workarounds" and "active search/discovery behavior," which are naturally sourced from Class B-type evidence. The audit's fix makes explicit what was already implicit but under-operationalized.

**Effect on research process:** quiet domains are no longer automatically killed for lack of complaint volume; they must be checked against Class B before any kill decision. This also directly feeds the revised next research question (§16 below).

**Verdict: ACCEPTED.** Extends an evidence type already present in `AGENTS.md` §4 into an explicit, parallel sourcing discipline; does not introduce a new category of evidence the project files didn't already consider valid.

---

## 6. Distribution Evidence — Operationalized

**Audit finding:** the concept "evidence of successful entry by a new/small vendor" already existed in the v1 baseline glossary, but no operational test defined when a channel counted as verified. Statements like "SEO could work" or "there is a marketplace" could pass as distribution evidence by default.

**Change made:** `BASELINE.md` §9 requires, per-candidate, at least one of: (1) an observed case within the last 12 months of a small/unknown vendor acquiring customers through that exact channel, with the mechanism identified, or (2) a structurally newcomer-friendly channel mechanism with its rules verified from a reliable source. Also requires the channel's actual rules (self-promo bans, moderation, ranking) to be checked, and a concrete currently-live venue to be named, not a category of channel in the abstract. Adds an explicit ordering rule: a candidate must not get `KEEP` while Distribution is unverified.

**Reason:** this is a direct operationalization of a concept `LESSONS_FROM_V2.md` already established (marketplace presence ≠ new-vendor discoverability) generalized to all channels, not just marketplaces — consistent with, not contradicting, the existing marketplace lesson.

**Effect on research process:** "we could try X channel" no longer counts as distribution evidence for any candidate; distribution must be checked per-candidate with a named, current, rule-verified venue before a `KEEP` decision.

**Verdict: ACCEPTED.** Directly extends `LESSONS_FROM_V2.md`'s marketplace-specific finding to the general distribution concept already present in v1's glossary; no new channel-level facts were asserted.

---

## 7. Signal Freshness and Source Hygiene

**Audit finding:** the baseline had no freshness requirement (stale complaints about long-fixed problems stay indexed and get counted as current) and no independence check (the same complaint cross-posted across communities could be counted as multiple sources). "Alternative to X" pages were not flagged as a distinct, weaker evidence type.

**Change made:** `BASELINE.md` §11 requires, for important evidence: source date, observation date if different, primary/secondary classification, an independence check (cross-posted/syndicated content doesn't count as multiple sources), a ~12-month freshness threshold (older = "stale"), and a derivation check for pages that appear to share an underlying source. "Alternative to X" pages are explicitly downgraded to lead sources only, not demand evidence, unless independently corroborated.

**Reason:** this is a direct extension of `AGENTS.md` §8's existing fact/interpretation discipline ("state the observed fact, identify the source, distinguish inference... record uncertainty") — §8 already required sourcing rigor; this patch adds the specific dimensions (date, independence, derivation) that rigor requires in practice but that §8 left unspecified.

**Effect on research process:** evidence records must now carry dates and an independence/derivation note; volume of matching pages is no longer usable as a proxy for strength of evidence.

**Verdict: ACCEPTED.** A direct, specific extension of an evidentiary discipline (`AGENTS.md` §8) the project already committed to, not a new principle.

---

## 8. Do Not Overfit to Loud Domains

**Audit finding:** complaint volume was at risk of being read as a proxy for market attractiveness, which would systematically bias domain selection toward "loud" categories regardless of actual spending/payment strength.

**Change made:** `BASELINE.md` §12 states explicitly: complaint volume is not a proxy for market attractiveness; a quiet domain with strong Existing Spending/Payment Plausibility evidence remains eligible; a loud domain with weak spending/payment evidence remains `INCONCLUSIVE`, not `KEEP`.

**Reason:** this is a direct restatement of the non-substitutability principle already established in v1 ("a weaker signal cannot compensate for failure at a higher-order gate," `STRATEGY.md`) applied specifically to the complaint-volume vs. spending-evidence pairing the audit identified as most at risk of being silently substituted.

**Effect on research process:** a research agent cannot promote a candidate to `KEEP` on complaint volume alone, and cannot kill a quiet candidate for lack of complaint volume alone — both directions of the bias are closed.

**Verdict: ACCEPTED.** Restates an existing non-substitutability principle at a specific risk point; no new rule invented.

---

## 9. Reconcile Existing Contradictions

**Audit finding (inherited from `BASELINE.md` v1's own "Current Unknowns"):** (a) `RESEARCH.md`'s status field used `DISCOVERY/VALIDATION/KEEP/KILL/BLOCKED/INCONCLUSIVE` while `AGENTS.md`/`DECISION.md` used `KEEP/TEST/KILL/BLOCKED/INCONCLUSIVE`, with no stated relationship between `VALIDATION` and `TEST`; (b) three non-identical evidence-chain formulations existed across `STRATEGY.md`, `AGENTS.md` §3, and the original task brief.

**Change made:**
- **Status vocabulary (`BASELINE.md` §3):** `AGENTS.md`/`DECISION.md`'s vocabulary (`KEEP/TEST/KILL/BLOCKED/INCONCLUSIVE`) adopted as canonical, since these are process rules rather than a record template. `DISCOVERY` retained but redefined as a pre-decision lifecycle phase, not a decision state. `VALIDATION` retired — it duplicated what `TEST` already means in `DECISION.md`. `RESEARCH.md`'s `Status` line was edited to match.
- **Evidence chain (`BASELINE.md` §4):** one canonical 10-stage chain adopted (`Pain → Buyer → Existing spending → Existing solution → Payment Plausibility Gate → Dissatisfaction → Switching intent → Switching feasibility → Wedge → Distribution → Validation → Build`), explicitly explaining why the Free-Incumbent Trap and the two source classes are *not* separate nodes (see §4's "why stages are not merged" note).

**Reason:** a research protocol that contradicts itself on basic vocabulary invites exactly the kind of silent, ad-hoc reinterpretation the audit is trying to close everywhere else. Canonicalizing on the process-rule files (`AGENTS.md`/`DECISION.md`) rather than the record template (`RESEARCH.md`) follows the principle that rules governing behavior should take precedence over a template that merely records outcomes.

**Effect on research process:** every future candidate uses one status vocabulary and one chain, referenced consistently across `BASELINE.md`, `RESEARCH.md`, and `DECISION.md`.

**Verdict: ACCEPTED.** This item was explicitly commissioned by the task (not proposed by the audit as optional), and required a concrete choice rather than further flagging; no new facts were involved, only a reconciliation of existing, self-authored process rules.

---

## 10. Anti-Scoring Philosophy

**Audit finding:** none of the audit's proposed fixes required numeric scoring, but the risk existed that operationalizing gates like Payment Plausibility or Distribution could slide into weighted checklists.

**Change made:** every new gate in this patch (Payment Plausibility, Switching Feasibility, Free-Incumbent Trap, Distribution) uses the existing `KEEP/TEST/KILL/BLOCKED/INCONCLUSIVE` vocabulary and qualitative, per-check pass/fail/unknown reasoning — no numeric scores, weights, or rankings were introduced anywhere in this revision.

**Reason:** `AGENTS.md` §7 explicitly bars scoring theater; reusing the single existing decision vocabulary everywhere (rather than inventing gate-specific vocabularies) also directly serves item 9's reconciliation goal — one vocabulary, no new complexity.

**Effect on research process:** no change in decision mechanics; the same five-state vocabulary now simply gets applied at more, earlier points in the chain.

**Verdict: ACCEPTED (preserved, not modified).** No scoring was proposed by the audit and none was introduced.

---

## Next Research Question — Verdict on Audit's Recommendation

**Audit finding:** the v1 next research question was directionally correct (domain-agnostic, targets the dissatisfaction→switching gap, requires method verification) but incomplete: it didn't require surfaced signals to concern a *paid* incumbent, didn't check switching feasibility, didn't include a non-complaint (Class B) source requirement, and didn't require a per-domain distribution note or freshness bound.

**Change made:** `BASELINE.md` §16 folds in all four fixes: paid-incumbent requirement, ~12-month freshness bound, dual source-class requirement (A + B), and a first-pass (not yet verified) distribution note per surfaced domain. Explicitly scopes out running the Payment Plausibility Gate, Switching Feasibility check, or Distribution verification during this discovery pass — those apply per-candidate later, to keep the discovery pass itself cheap.

**Verdict: MODIFIED** (per the audit's own verdict on itself: "MODIFY... After these four fixes the question can be accepted. Before them, no.") — accepted with exactly the four modifications the audit specified, no more and no less.

---

# RESEARCH READY

**What is now fixed:**
- Payment plausibility is checked early and cheaply, before expensive dissatisfaction mining (§6).
- Existing Spending is tiered; time/lost-revenue alone no longer passes the gate (§5).
- Switching intent is separated from switching feasibility, and switching destination must be recorded (§8).
- Free-incumbent domains can no longer ride complaint volume past the Existing Solution stage without monetization evidence (§7).
- Domain discovery uses two parallel source classes; absence of public complaints is explicitly "unknown," not "no problem" (§10).
- Distribution evidence is operationalized per-candidate, with a 12-month recency bound and named, rule-verified venues (§9).
- Evidence hygiene (dates, independence, staleness, derivation) is required for important evidence (§11).
- Loud-domain bias is explicitly barred in both directions (§12).
- Status vocabulary and evidence chain are each canonicalized to one version, with the reasoning for what was merged and what wasn't made explicit (§3, §4).
- No scoring, weighting, or ranking exists anywhere in the methodology.

**What remains deliberately uncertain:**
- Whether marketplace-based distribution is viable for a cold-start solo vendor — still open in both directions; this patch does not resolve it because the source files don't support resolving it either way.
- Whether the `nishe_scout` archive contains any evidence transferable outside its Atlassian-specific scope — not assessed.
- Whether any real domain will actually clear the Payment Plausibility Gate or the Free-Incumbent Trap — cannot be known without doing the market research this document and this patch both deliberately withhold.

**Exact next research question to hand to the research agent:**

> Using two parallel source classes — (A) dissatisfaction/switching sources: reviews, comparison discussions, migration stories, public complaints, communities; and (B) spending/behavioral sources: visible pricing, hiring demand, recurring contractor/freelancer demand, procurement/tender evidence where accessible, and other observable evidence of money or dedicated labor already allocated to a problem — what repeatable and verifiable method can surface a set of candidate problem domains where: the incumbent solution is demonstrably **paid** (not free), the switching/dissatisfaction signals found are no older than ~12 months, and each surfaced domain carries a first-pass note on which channel a problem-aware buyer might discover a new entrant through (without yet verifying that channel per the Distribution gate)?
>
> For each surfaced domain, record: source class(es) used, whether the buyer segment posts publicly at all, and source dates — but do **not** run the Payment Plausibility Gate, Switching Feasibility check, or Distribution verification yet. Those apply per-candidate once a specific domain is selected for deeper research, not during this discovery pass.

This question names no niche, marketplace, platform, or product, and produces only a candidate-domain list with sourcing metadata — not a decision on any candidate.
