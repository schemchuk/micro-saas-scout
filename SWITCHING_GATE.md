# Switching Feasibility & Switching Destination Gate

## Scope

- **Date:** 2026-09-22
- **Method:** `BASELINE.md` §8, applied to the one candidate currently eligible for this gate per `PAYMENT_GATE.md`'s "Next Research" section. Desk research only — vendor ToS/policy/help-center pages fetched directly as primary sources; Capterra/G2/Reddit searched for independent reviewer or forum evidence. No users contacted, no product built.
- **Candidate tested:** Tax Practice Client Document/Engagement Workflow Portal.
- **Gates tested:** Switching Feasibility & Switching Destination (`BASELINE.md` §8) only.

## Buyer

Small US tax preparation/accounting firms (solo practitioners to small teams).

## Already-documented switching evidence (from `DISCOVERY.md`, carried forward)

≥7 named, dated Capterra reviewers on **TaxDome's own review page** describing a prior competitor (Canopy, SmartVault, ShareFile, Karbon, SafeSend, GoFileRoom, PracticeSuite, Keap, Onboardible) — flagged from the start as a destination-biased sample. One counter-example: Megan C. (Financial Cents' own Capterra page, Oct 2025) switched FROM TaxDome TO Financial Cents.

---

## 1. Lock-in

**Client-facing lock-in is real and vendor-acknowledged, not speculative.** Financial Cents' own migration guide (a competing vendor's content, but the most operationally specific source found) instructs firms switching off TaxDome to provide clients "step-by-step instructions... for logging into the new portal, submitting documents, or completing tasks" and to "share the timeline for migration, including... deadlines for document submissions" — i.e., the client relationship itself, not just internal ops, has to be actively re-anchored to a new URL/login. TaxDome's own migration-guidance page independently lists "Client disruption when introducing new systems or portals" as one of the top reasons firms *hesitate* to switch (stated in the context of switching TO TaxDome, but the friction is structurally symmetric for switching away).

The same Financial Cents guide flags **workflow automation as not cleanly portable**: it advises firms to "separate the data you need to migrate from the data you can archive or rebuild," explicitly naming "pipeline stages, automations, and historical activity logs" as the kind of setup that doesn't move with you.

**Gap:** no first-person reviewer account was found (TaxDome, Canopy, or SmartVault review pages) describing an actual disrupted client relationship post-switch (e.g., "clients couldn't find us" / "lost client logins"). The lock-in claim is vendor-stated, not buyer-confirmed.

---

## 2. Data portability

Distinguishing "documents downloadable" from "whole setup migratable" — the evidence cleanly separates:

- **TaxDome:** publishes only *import* documentation (help.taxdome.com/article/122-import; taxdome.com/migration-guidance) — "client records, documents, tags, pipelines, notes" moving **into** TaxDome. No vendor page describing export **out** of TaxDome was found. Individual documents are downloadable one at a time via the PDF viewer (download/print/seal/request-signature); no bulk/structured export tool for the whole portal is documented.
- **Canopy:** its own ToS §11(a) states Canopy "is not a provider of data back-up or archiving services" and the customer is "solely and exclusively responsible for backing up and archiving of all Client Content" — no export tool at all is documented.
- **SmartVault:** the only documented export is a **client list to CSV** (help.smartvault.com/hc/en-us/articles/16215985934359) — names/contacts, not documents or e-signature history. Its own cancellation help article instructs users to manually "download or back up your documents locally... before your subscription ends" via desktop/drive sync tools — a manual pre-cancellation scramble, not a formal export feature.
- **Financial Cents** (the one documented TaxDome switcher's destination): imports clients via CSV or QuickBooks Online sync; its own guide explicitly tells firms not to try to move everything, but to selectively rebuild.

**Conclusion:** documents can be manually downloaded/backed up from all three incumbents before leaving; **no vendor of the three, nor the one confirmed destination, documents migrating the whole client-portal configuration (automations, e-signature history, workflow templates) intact.** E-signature audit trails are viewable in-app (help.taxdome.com/article/232) but no export/download mechanism for the trail itself was found.

---

## 3. Contractual/procurement friction

Directly re-verified on each vendor's own current ToS/policy pages (all fetched 2026-09-22) — **all three incumbents have materially the same structure**:

- **TaxDome** — Refund Policy (taxdome.com/policies/refund-policy, modified 2026-05-06): *"TaxDome does not provide refunds or credits for any service, subscription plan, firm balance, or usage credit."* Plans are billed upfront for 1-, 2-, or 3-year terms; cancellation must be submitted up to 7 days before renewal, which only stops the *next* renewal — it does not exit the current prepaid term or refund unused time.
- **Canopy** — Terms of Service (getcanopy.com/terms-of-service, updated 2026-05-29), §10(d)–(e): auto-renews for "additional subscription terms of the same length"; *"cancellation shall not become effective until the expiration of your then-current subscription term"*; *"CANOPY DOES NOT PROVIDE REFUNDS OR CREDITS WITH RESPECT TO THE SERVICE OR ANY SUBSCRIPTION PLAN, INCLUDING FOR ANY PARTIALLY USED SUBSCRIPTION TERMS."*
- **SmartVault** — Terms of Service (smartvault.com/terms-of-service): *"During the Initial Term, you may not cancel the Agreement except as expressly permitted in these Terms (e.g. for breach by us)... Fees for the Initial Term are non-refundable."* Initial Term = 1 year for annual plans (1 month for monthly plans where offered); auto-renews unless cancelled ≥21 days before the renewal date.

**Conclusion:** this is a real, specific, vendor-confirmed switching barrier, exactly as flagged in the task. A dissatisfied firm mid-term is contractually stuck paying (and technically still has access) until the prepaid term ends — none of the three offers early termination or partial refund. This materially caps how fast "switching intent" seen in reviews can convert into "actual switching": it can only happen at renewal-date boundaries, not on demand.

---

## 4. Integration/workflow rebuild

Rated **substantial**, based on convergent (not single-source) evidence:

- TaxDome's own migration-guidance page (marketing content, but a specific operational claim): *"Most firms complete TaxDome implementation in 6–8 weeks"* even with a dedicated onboarding manager and paid professional services (from $299).
- Financial Cents' migration guide gives a concrete phased timeline for leaving TaxDome: Weeks 1–2 rebuild workflows/templates from scratch, Weeks 3–4 staff training, Month 2 migrate active clients/documents, Month 3 full rollout — roughly a **quarter**, and explicitly recommended to happen outside tax season "to minimize operational downtime."
- A Capterra reviewer (via search synthesis, Canopy page — not independently re-verified verbatim in this pass) described paying for two months while investing "an enormous amount of time and effort" getting everything set up on Canopy, only to be told the platform wasn't ready — illustrating real time/cost exposure during a platform transition in this category (this instance was adopting Canopy, not leaving it, but the magnitude is informative).
- A separate Canopy reviewer (same caveat on verbatim sourcing) reported deciding **not** to switch specifically because "clients are already used to the client portal" — direct evidence that client-facing rebuild cost actively suppresses switching, not just adds friction after the fact.

What needs rebuilding, per the above: client onboarding/engagement-letter templates, automated reminder/pipeline workflows, and client-facing portal access — all explicitly named as non-portable or requiring active client re-communication. Billing/e-signature *integrations* specifically were not directly evidenced either way (rated unknown, not assumed trivial).

---

## 5. Switching destination / survivorship bias check — the central finding

A dedicated search pass looked for **independent** evidence (i.e., not on TaxDome's own page) of firms leaving Canopy, SmartVault, ShareFile, Karbon, SafeSend, GoFileRoom, PracticeSuite, Keap, or Onboardible:

- Multiple differently-worded Reddit searches (`site:reddit.com r/taxpros ...`, `site:reddit.com r/accounting ...`, naming each competitor) returned **zero actual Reddit threads** — every result resolved back to Capterra/G2/press pages. This is a genuine negative result from several attempts, not an unexplored gap.
- Canopy's own Capterra review page: no named, dated reviewer was found stating they left Canopy for a named competitor. The only relevant signal (see §4) is a reviewer who considered SmartVault/Liscio but explicitly **did not switch**.
- SmartVault's own Capterra page: recent reviews (Jan 2026, Mar 2025, Nov 2024) are pricing/UX complaints ("price went up significantly," "a big disappointment") — recurring dissatisfaction, but none confirm a completed move to a named destination.
- No independent (non-vendor-hosted) account of switching away from any of the eight named competitors was located anywhere in this pass.

**Honest read:** after specifically searching for it, the switching-destination evidence for this candidate is still concentrated almost entirely on **vendor-hosted review pages of the destination vendor** — TaxDome's own page for the ≥7 switches-in, and Financial Cents' own page for the one switch-out. We have not found a single instance of switching evidence living somewhere neither vendor controls (no Reddit thread, independent blog post, or forum confirms it independently). This is stronger and more specific than the caveat Discovery originally flagged: it is not just "TaxDome's page is biased toward TaxDome as a destination," it is that **every piece of switching evidence for this whole candidate, on both sides, comes from some vendor's own review funnel** — a structural sampling limitation of the category, not just of one vendor.

Per `BASELINE.md` §8's destination rule: observed migrations run between already-entrenched incumbents (TaxDome, Canopy, SmartVault, ShareFile, Karbon are all established players), which must be recorded as a **distribution/entry risk**, not an opportunity — none of this evidence shows an unknown, solo-built entrant successfully capturing switchers, only established players trading customers with each other (plus the single Financial Cents exception, itself an established, funded specialist, not a solo-built product).

---

## Gate assessment against §8's decision rule

- Lock-in and contractual friction are **real and vendor-confirmed**, not merely aspirational complaints.
- Realistic alternative availability is **confirmed** (Financial Cents, verified in `PAYMENT_GATE.md` as a genuine self-serve destination with at least one named switcher).
- Switching is therefore **difficult but not prohibitive** — actual completed migrations are documented (with the caveats above), so the signal is not downgraded to "dissatisfaction only."
- The unresolved item is not whether switching is *possible* but whether it is *independently confirmed as common/easy outside vendor-controlled review pages* — it is not, per this search pass. This should be carried forward explicitly rather than smoothed over.

## Remaining unknowns

Whether any first-person account exists (anywhere) of a client being confused/lost during a firm's platform switch. Whether e-signature audit trails can be exported in bulk from any of the three incumbents (only in-app viewing was confirmed). Whether billing/payment integrations specifically survive a switch. Whether SmartVault's month-to-month option (implied by its cancellation help article's "billing cycle" language) is available to typical solo/small-firm customers or only some plans, given its ToS default is an annual "Initial Term." The two Canopy Capterra reviewer claims in §4/§5 were sourced via search-tool synthesis rather than independently re-verified against the live page character-by-character — flagged as a minor sourcing-reliability caveat, not treated as disqualifying since both are consistent with the directly-verified ToS/migration-guide evidence.

## Sources

- taxdome.com/policies/refund-policy (primary, TaxDome, page modified 2026-05-06, accessed 2026-09-22)
- taxdome.com/migration-guidance (primary, TaxDome, page modified 2026-03-23, accessed 2026-09-22)
- help.taxdome.com/article/122-import (primary, TaxDome Help Center, accessed 2026-09-22)
- help.taxdome.com/article/232-viewing-a-document-s-history-file-audit-trail (primary, TaxDome Help Center, accessed 2026-09-22, via search synthesis)
- taxdome.com/pdf-editor (primary, TaxDome, accessed 2026-09-22, via search synthesis)
- getcanopy.com/terms-of-service (primary, Canopy, page updated 2026-05-29, accessed 2026-09-22)
- smartvault.com/terms-of-service (primary, SmartVault, 2025 version PDF referenced, accessed 2026-09-22)
- help.smartvault.com/hc/en-us/articles/360051277373-Canceling-Your-SmartVault-Subscription (primary, SmartVault Help Center, accessed 2026-09-22)
- help.smartvault.com/hc/en-us/articles/16215985934359-Exporting-your-List-of-Clients-from-SmartVault (primary, SmartVault Help Center, accessed 2026-09-22, via search synthesis)
- financial-cents.com/resources/articles/top-taxdome-alternatives/ (primary but vendor-authored — Financial Cents, a competing vendor; last updated 2026-01-13, accessed 2026-09-22)
- capterra.com/p/150647/Canopy-Tax/reviews/ (primary, named/dated reviewers, accessed 2026-09-22)
- capterra.com/p/82811/SmartVault/reviews/ (primary, named/dated reviewers, via search synthesis, accessed 2026-09-22)
- capterra.com/p/186749/TaxDome/reviews/ (primary, carried forward from `DISCOVERY.md`)
- capterra.com/p/186837/Financial-Cents/ (primary, Megan C. review, carried forward from `PAYMENT_GATE.md`)
- Reddit r/taxpros, r/accounting (searched directly, multiple queries, no relevant independent threads found — negative result recorded, not an unexplored gap)

## Methodological Issues

None found. `BASELINE.md` §8's three-axis structure (lock-in, contractual/procurement, realistic alternative availability) plus its required switching-destination check were applied as specified; no contradiction with `BASELINE.md`/`DECISION.md` encountered.
