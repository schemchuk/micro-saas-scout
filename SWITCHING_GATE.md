# Switching Feasibility & Switching Destination Gate (§8)

## Candidate — Tax Practice Client Document/Engagement Workflow Portal

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

---

## Candidate 5 — eBay/Etsy Cross-Listing & Listing-Template Management

**Buyer:** Long-tenured eBay/Etsy power sellers and small multichannel resellers who pay monthly for a listing-management/template subscription.

**Special circumstance:** InkFrog (dominant incumbent, Wix-owned) announced shutdown April 29, 2026, effective June 1, 2026 — a forced migration event for all its users, on top of voluntary dissatisfaction-driven switching that was already occurring.

**Scope note:** this task is pure fact-finding for §8 (lock-in, portability, procurement, alternative availability, switching destination). No product decision is made here.

---

### 1. Lock-in

InkFrog's own shutdown email (April 29, 2026, quoted verbatim by both the company-facing press and by sellers who forwarded it into the eBay Community) offered exactly two things: CSV export of listing data until May 31, 2026, and a prorated refund of unused billing days. Nothing else. No template-HTML export, no bulk-image export, no named migration partner.

Two lock-in mechanisms independently confirmed:
- **Image hosting.** The CSV export contains image *URLs* pointing at InkFrog's own CDN (`imgs.inkfrog.com`), not the image files. Named eBay Community user **Mathias7** (primary, ~2026-05-07): *"I can download an account csv with my listing data... but there's no image download/backup option. I hate how you get locked into tools like this, independent image hosting separate from the listing tool is more important than ever."*
- **Template self-containment.** Per Frooition's retrospective (vendor blog — Frooition sells a paid "Listing Rescue" service, so treat the framing as self-interested, but the technical mechanism is independently plausible and consistent with community accounts): live eBay listing HTML built with InkFrog templates referenced InkFrog-hosted images/CSS/cross-sell scripts. When InkFrog's servers went dark June 1, every listing using those templates broke simultaneously — not gradually.

No evidence was found describing eBay/Etsy marketplace **API re-authorization** itself as a friction point (open gap, not confirmed either way).

### 2. Data portability

InkFrog itself provided only the bare CSV (text fields), executed clumsily in practice — eBay Community user **moo_cow_corner** (primary, ~2026-06) describes having to export the "Library" (drafts) separately from the main CSV, 50 listings at a time, page by page, to be sure nothing was missed.

Because InkFrog provided no image export, third parties filled the gap **unprompted**, before shutdown: SpareDollar/"Rescue" (built post-announcement by InkFrog co-founder Tomas Salas), Nembol, and a hobbyist tool "newpad.app" all pulled images via the CSV's URLs while InkFrog's CDN was still live. Named users confirm this worked: **saturdaystoys** (primary, ~2026-05): *"Over 10,000 inkFrog listings... and over 60,000 accompanying photos... DONE within 30 minutes."* But this "Rescue" step is a holding platform, not a live listing tool, and **jim1024** (primary) asks, unanswered in-thread, whether sold/unsold library history was fully captured — genuinely unresolved.

Critically, the task's hypothesis about eBay-API-direct import is **confirmed true, for two of the three named vendors**: LitCommerce's own product page describes CSV import *and* separately a paste-based "Import from InkFrog" template re-import. FolderLister's own page documents an explicit **eBay-API path that needs no InkFrog export at all**: "Open Manage Listings, let your active eBay listings load, and use Add selected." 3Dsellers (a real, frequently-named destination, though outside the original three) works the same way per a secondary comparison source, consistent with named user **myshoppingtree**'s own account of switching to it. No InkFrog-specific import feature was found for Sixbit (unconfirmed). This means *active* eBay listings can often be reclaimed without any InkFrog cooperation — a genuine reduction in switching cost versus a typical SaaS-to-SaaS migration. It does **not** rescue InkFrog-hosted template design/CSS or description images not already resolved on eBay's own CDN.

### 3. Contractual/procurement friction

No evidence of an annual contract or minimum-term clause blocking InkFrog cancellation was found; the shutdown email's promise of a per-day prorated refund is itself evidence InkFrog ran rolling/monthly billing. The forced shutdown makes this question largely moot for InkFrog, as expected.

A different, unexpected friction point surfaced on the **destination** side: **saturdaystoys** (primary, ~2026-05) reports a "meltdown" trying to cancel a 3Dsellers trial: *"Customer service is managed only by a 'bot'... Tried to cancel my 7-day trial subscription... but failed... They now claim it's impossible to cancel today."* This is real onboarding/cancellation friction, but it belongs to a destination vendor, not to leaving InkFrog.

### 4. Integration/workflow rebuild

Evidence is mixed and split by path taken:
- **Template/design rebuild:** substantial unless routed through LitCommerce's specific InkFrog-template importer (vendor claim, not independently confirmed by a first-person account praising *that specific feature*) or a pre-shutdown rescue tool.
- **Item-specifics mapping:** one genuine first-person positive account — **lit1213** (primary, voluntary-switch thread): *"Personally I use folderlister... Re-use profiles with pre set item specifics... works very well for my big Collection of postcards."*
- **Image hosting:** recoverable only if a CSV+image rescue was done before May 31, 2026, or if photos already resolved on eBay's own CDN.
- **Cross-listing sync/automation rebuild:** no first-person account found either way (gap).
- Outcomes range from **easy** (**myshoppingtree**, primary, 24-year seller, 3Dsellers: *"the migration has been a very positive experience... a fairly easy transition"*) to **abandoned rather than migrated** (**funfactorychannel**, primary, 10-year InkFrog user: *"I am giving up on the photo and data. I will just retake pictures and re-search as needed."*). **Rating: moderate for basic listing continuity (via eBay-API re-import), substantial/lossy for full-fidelity template+image migration without proactive rescue action.**

### 5. Forced vs. voluntary

**Voluntary** (eBay Community thread "Inkfrog alternatives?", original post dated **2022-11-29**, confirmed via page metadata — years before the shutdown): organic complaint *"inkfrog has so many issues now I can't even list correctly."* Destinations named: LitCommerce, Sixbit, FolderLister. Caveat for honesty: the specific *replies* recommending these tools are dated ~May 2026 — after the April 29 shutdown announcement — so they cannot be cleanly certified as untainted by shutdown urgency, even though the original complaint clearly predates it.

**Forced** (thread "Inkfrog to shut down," started directly in response to the shutdown email): a **different and wider** destination set — SpareDollar/Rescue, 3Dsellers, Nembol, SixBit, sellsetgo, ResaleOS. LitCommerce and FolderLister are notably **absent** here. Forced migrators show more acute image/data-loss anxiety and more destination-onboarding friction (3Dsellers cancellation meltdown above) than the voluntary thread's brief "pretty smooth for syncing so far" (**andy.johns_4**).

A second, independent forced-migration data point, different incumbent, same pattern: LitCommerce Trustpilot review dated **2026-09-20** (primary): *"We were a long term user of Codisto Linq/Marketplace Connect, which suffered what can only be described as a catastrophic failure on 6/8/26... almost a month had passed with no ability to push products onto E-Bay... after making some tweaks to the data structure in Shopify... within a week of pressing the big green 'GO' button, we are fully operational."* Confirms the "catastrophic incumbent failure → forced migration → LitCommerce, ~1 week to operational" pattern outside InkFrog specifically (this reviewer is Shopify + marketplace-apps, not a classic InkFrog template user, so it corroborates the general pattern more than it measures InkFrog-specific rebuild cost).

### 6. Switching destination pattern

LitCommerce, FolderLister, Sixbit, 3Dsellers, Nembol, SpareDollar are all **small/specialist vendors** — none is an entrenched dominant incumbent, and none of the observed destinations is Wix's own tooling, eBay's/Etsy's own native listing tools, or another major platform. This is the **opposite** of the BASELINE.md §8 "distribution/entry risk" trap: switchers are moving *away* from a dominant incumbent toward multiple small, competing specialist tools, which is a more favorable signal for a new solo-built entrant than churn between two giants would be. Gap: no direct search was run for whether any meaningful fraction of InkFrog's base migrated to a major platform's built-in tools instead.

### §8 downgrade decision

**Not downgraded.** Lock-in and portability friction are real but bounded and partially mitigable (CSV export exists; eBay-API-direct re-import bypasses InkFrog cooperation for live listings; multiple named forced *and* voluntary migrators completed switches, several rating the process easy). Procurement/contract friction is moot (forced shutdown, no restrictive terms found). Realistic alternatives clearly exist and have named, paying/active users. Switching destination is specialist vendors, not entrenched incumbents. **Switching feasibility is confirmed as real, not merely aspirational — this candidate advances past §8.**

### Remaining unknowns

Whether eBay/Etsy API re-authorization itself is a friction point; whether Sixbit has any InkFrog-specific import path; whether LitCommerce's template-importer is as smooth in practice as the vendor claims (no first-person account found praising that specific feature); whether any InkFrog users migrated to a major platform's native tools rather than a specialist vendor; whether SpareDollar's "Rescue" data (sold/unsold history) was ever confirmed complete.

---

## Sources

- InkFrog shutdown email, quoted verbatim, 2026-04-29 — primary (company communication), via [Value Added Resource](https://www.valueaddedresource.net/inkfrog-shut-down/) (accessed 2026-09-22) and cross-posted in [eBay Community: "Inkfrog to shut down"](https://community.ebay.com/forum/selling-57920/topic/inkfrog-to-shut-down-161100/) (accessed 2026-09-22).
- [eBay Community: "Inkfrog to shut down"](https://community.ebay.com/forum/selling-57920/topic/inkfrog-to-shut-down-161100/) — primary, first-person sellers (apmtrade, Mathias7, moo_cow_corner, funfactorychannel, saturdaystoys, barbie*ville, jim1024, myshoppingtree, nit2290, ellimac_34), dated ~2026-05 to ~2026-09 per thread metadata; accessed 2026-09-22.
- [eBay Community: "Inkfrog alternatives?"](https://community.ebay.com/forum/seller-tools-57919/topic/inkfrog-alternatives-441820/) — primary, original post 2022-11-29 (confirmed via page metadata), replies (andy.johns_4, ethanwalker_9, lit1213) dated ~2026-05; accessed 2026-09-22.
- [Frooition: "InkFrog Shutdown 2026: The Full Retrospective"](https://www.frooition.com/blog/inkfrog-templates-broken-ebay-listings/) — secondary, vendor blog with a commercial conflict of interest (sells "Listing Rescue"), published 2026-05-06, updated 2026-06-01; accessed 2026-09-22.
- [LitCommerce: "Migrate From InkFrog to LitCommerce"](https://litcommerce.com/inkfrog-to-litcommerce/) — vendor marketing page describing product mechanism, not switching-behavior evidence; accessed 2026-09-22.
- [FolderLister: "InkFrog Alternatives for eBay Sellers"](https://folderlister.com/inkfrog-alternative/) — vendor marketing page describing product mechanism; accessed 2026-09-22.
- [Trustpilot — LitCommerce review, "Superb App, highly recommended"](https://www.trustpilot.com/reviews/6ab002926dd5ed1ff61fe2fc) — primary, named account of Codisto Linq/Marketplace Connect failure and migration, dated 2026-09-20; accessed 2026-09-22.
- Trustpilot — Lingo Lohr (2026-02-17) and Shizonic (2025-11-17) LitCommerce reviews — primary, previously verified in `PAYMENT_GATE.md`, confirming paid status; re-cited here for the forced-vs-voluntary destination analysis.
- [ListPerfectly: "InkFrog Is Shutting Down"](https://listperfectly.com/selling/inkfrog-shutting-down-what-resellers-need-to-do/) — secondary, corroborates the image-URL-not-file CSV export caveat; accessed 2026-09-22.
