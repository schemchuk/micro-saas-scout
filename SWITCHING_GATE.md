# Switching Feasibility & Switching Destination Gate

## Scope

- **Date:** 2026-09-22
- **Method:** `BASELINE.md` §8, applied per Task 06. Desk research only — vendor ToS/policy/help-center/migration-guide pages fetched directly as primary sources for lock-in, portability, and contract terms; Capterra/G2/Trustpilot/eBay Community/Reddit searched for independent, named, dated switching evidence. No users contacted, no product built, no wedge designed.
- **Candidates tested:** the four candidates currently `PASS` in the corrected `PAYMENT_GATE.md` — Insurance Commission Reconciliation; Multichannel E-Commerce Accounting Reconciliation; Tax Practice Client Document/Engagement Workflow Portal; eBay/Etsy Cross-Listing & Listing-Template Management.
- **Gates tested:** Switching Feasibility & Switching Destination (`BASELINE.md` §8) only — lock-in, data portability, contractual/procurement friction, integration/workflow rebuild, actual switching evidence, and switching destination.
- **Gates explicitly NOT tested:** the blocked Construction Subcontractor candidate (excluded per task scope); Distribution Evidence (`BASELINE.md` §9); any wedge design, product decision, TAM/SAM/SOM, or validation/preorder activity.

---

## Candidate 1 — Insurance Commission Reconciliation

### Buyer
Independent US P&C/multi-line insurance agencies — finance/operations staff (bookkeepers, controllers, agency principals/administrators) reconciling monthly carrier commission statements.

### Existing solution
Commission Tracker, Commission Wizard, AgencyBloc AMS+ (a full agency management system, not a standalone commission tool).

### Lock-in
- **Commission Tracker:** no proprietary data format or AMS integration found (SourceForge's integrations listing for the product shows none, consistent with the absence of any integration claim on the vendor's own site) — primary/vendor + secondary/aggregator, accessed 2026-09-22.
- **Commission Wizard:** a real, vendor-documented cumulative lock-in mechanism exists, distinct from mere tenure — the vendor's own site states: "Upload your agency management system (AMS) export once and save it for future use... the system already knows the column mappings," and "By the tenth carrier, the system recognizes 90%+ of columns automatically" (commissionswizard.com, primary, accessed 2026-09-22). This means a user accumulates a carrier-mapping library over time that a competing tool would not have. This vendor is not the destination in either documented switch below, so it does not block the switches actually evidenced, but it is a relevant category-level finding.
- **AgencyBloc AMS+:** lock-in derives from the breadth of the system (CRM, policies, quoting, QuickBooks/Zapier integrations, open API — secondary sources: Zapier, SourceForge/Slashdot) rather than from the commission module specifically. No proprietary commission-data format was found.

### Data portability
- **Commission Tracker's own Cancellation Policy** (primary, commission-tracker.com/cancellation-policy/, accessed 2026-09-22): "Upon cancellation, all of your Content will be removed from the Software," and recommends exporting reports before cancelling because "this information cannot be retrieved once your account is canceled" — no grace period.
- **Commission Wizard's own Terms of Service** (primary, commissionswizard.com/terms, accessed 2026-09-22): "You may request export of your data within 30 days of termination," and "You retain all rights to the data you upload" — a materially softer policy than Commission Tracker's.
- **AgencyBloc:** no ToS/legal page was reachable (repeated 404s). A Custom Report builder can export "commission discrepancies with all the carrier information" (primary, agencybloc.com), but this is a selective report, not a full data export; an open API exists per secondary sources but was not confirmed for commission data specifically.
- Distinguishing the two claims explicitly: data (reports) can be exported from all three to varying degrees, but **no source for any of the three documents exporting/importing the carrier-mapping rules themselves** — the reconciliation "setup," not just the raw data, is not shown to be portable.

### Contract / procurement friction
- **Commission Tracker:** "month-to-month-no-contract" per its own pricing page URL and copy (primary); $120 flat signup fee applies regardless.
- **Commission Wizard:** "No setup fees, implementation fees, or long-term contracts" (primary, pricing page).
- **AgencyBloc:** no dollar figures or contract terms published; a claim of a "12-month commitment... enforced if you cancel early" appears only in a secondary SEO blog (unlockedcrm.ai, published 2026-07-02) that itself cites unofficial "customer quotes shared... in 2025–2026," not an AgencyBloc-published document. No Capterra reviewer was found confirming an early-termination fee. **Unconfirmed by primary source** — recorded as a gap, not as a finding.

### Integration / workflow rebuild
For the AgencyBloc AMS+ → Commission Tracker switch specifically: no first-person account of the migration mechanics was found. Structurally, since Commission Tracker has no native AMS integration, an agency would need to manually export from AgencyBloc's Custom Report builder and re-import into Commission Tracker on an ongoing basis, and would need to rebuild carrier-matching rules from zero in the new tool. **Rating: unknown/moderate** — based on structural inference (absence of integration), not a direct migration account; no hours/costs are stated anywhere and none are estimated here.

### Actual switching evidence
- **Manual Excel → Commission Tracker:** "Ben T.," President/Financial Services (Capterra, dated Aug 2024 — flagged >12 months old): "After 1,000 sales in Excel, the matrix slowed down to a crawl" — an actual, completed, first-person move, not a feature request or "alternative to X" mention.
- **AgencyBloc AMS+ → Commission Tracker:** "Kathy B.," agency administrator (Capterra, dated Sept 2026): switched citing cost and ease of use — actual, first-person, dated within the freshness window.
- Both are individual named reviewers describing a completed transition with a stated reason, meeting the bar for actual switching evidence (not dissatisfaction alone).

### Switching destinations
Both documented switches land on **Commission Tracker**, which is itself a small/specialist vendor (flat low-cost pricing tiers, no broad integration suite, narrow product scope) — not a dominant incumbent. Pattern: manual workflow → paid specialist (Excel case); incumbent full-platform (AMS) → narrower specialist tool (AgencyBloc case). Neither documented switch moves between two large, entrenched incumbents.

### Feasibility assessment
Switching appears realistically feasible for a small independent agency: both observed destinations (Commission Tracker, and Commission Wizard as an alternative) are no-contract, low-cost-entry, self-serve tools, and two real, dated, first-person completed switches are documented — one from a fully manual workflow, one from a competing paid platform. The main open risks are category-level rather than switch-specific: Commission Wizard's cumulative carrier-mapping lock-in (relevant to future switching away from Commission Wizard, not to the switches evidenced here) and Commission Tracker's own no-grace-period data deletion on cancellation (relevant to a future agency wanting to leave Commission Tracker, again not to the evidenced switches). Neither rises to a structural barrier that would make the two documented moves themselves infeasible.

### Gate result
**PASS**

### Remaining unknowns
AgencyBloc's actual contract/early-termination terms (only secondary-source claims found, no primary AgencyBloc document). The actual step-by-step mechanics of an AgencyBloc → Commission Tracker migration (no first-person account found). Whether Commission Wizard's cumulative-mapping lock-in would materially slow a future switch away from it, since it wasn't the destination in either evidenced case.

---

## Candidate 2 — Multichannel E-Commerce Accounting Reconciliation

### Buyer
Small-to-mid multichannel e-commerce sellers (roughly 100–20,000+ orders/month) and the bookkeepers/accountants who manage their books on Xero/QuickBooks Online.

### Existing solution
A2X, Link My Books, Dext Commerce, Taxomate, Tradebox/"Blocks."

### Lock-in
The marketplace/accounting API connections themselves are **not** the lock-in point: A2X's own help docs describe disconnecting via Settings > Connections as a normal self-service action, and Link My Books' own migration guide has sellers simply reconnect the same marketplace (Amazon, etc.) and accounting (Xero/QuickBooks) accounts to the new tool via standard OAuth re-authorization. The real lock-in is **accumulated configuration**: chart-of-accounts mappings, tax-rate rules, and COGS/tracking-code setups, since "each tool's own transaction-categorization logic" differs (e.g. A2X's rule structure vs. Link My Books' "10 top-level categories," per Link My Books' own migration guide, primary). Historical settlement postings already sent to Xero/QuickBooks remain in the ledger as-is — they are not migrated, only the go-forward process changes. No proprietary technical lock-in was found for Dext Commerce or Taxomate specifically (no vendor documentation located describing export/import blockers for either).

### Data portability
No evidence was found of either vendor exporting/importing raw historical settlement-reconciliation data in a structured, competitor-compatible file. Both vendors frame switching as "reconnect + remap," not "export/import." A2X's support docs (primary, support.a2xaccounting.com) tell cancelling users to "export any data you wish to retain before cancelling," since accounts and data are deleted 90 days after cancellation — a generic backup mechanism, not a Link-My-Books-compatible migration file. **Link My Books publishes a formal migration guide** ("How to migrate from A2X to Link My Books," help.linkmybooks.com/en/articles/8272311, primary) and offers a **free migration service** where its own staff manually transfer settings/mappings for the customer — direct evidence this friction point is real and well-known enough that a vendor competes on removing it, not evidence that it doesn't exist.

### Contract / procurement friction
- **A2X:** month-to-month billing, cancel anytime via self-serve UI, no stated minimum term, non-refundable but no cancellation penalty (support.a2xaccounting.com, primary).
- **Link My Books:** per its own Terms of Service (linkmybooks.com/terms-of-service, primary) and billing help page (help.linkmybooks.com/en/articles/6083796, primary), subscriptions run in 1- or 12-month terms with auto-renewal; cancellation must be submitted before the renewal date, effective at end of the paid period, no refund of the current period — no long-term lock-in contract, but a minor wrinkle: an annual-plan subscriber who cancels mid-term forfeits the remainder of that term.

### Integration / workflow rebuild
Per Link My Books' own migration guide (primary): reconnect sales channels and accounting software (a few clicks), then manually copy account mappings from A2X's "Accounts & Taxes" page into Link My Books' simplified category structure, fine-tune under "Account & Tax Mappings," and separately rebuild COGS/product-group/tracking-code setups if used. The guide explicitly warns of a **duplicate-posting risk** if both tools post overlapping settlement periods during cutover, and prescribes a clean-cutover sequence (stop A2X auto-posting, manually post the last few settlements from Link My Books, then resume automation). **Rating: moderate** — a bounded, vendor-documented procedure, realistically hours to about a day for a straightforward setup, longer with multiple tax jurisdictions or tracking codes; not weeks of reconciliation work, but not trivial either. No independent first-person account of the mechanics of a specific A2X→Link My Books migration was found (the cited reviewers document reasons for switching, not a blow-by-blow of the migration itself) — this is a gap, not an assumption of ease.

### Actual switching evidence
- A2X → Link My Books: Aaron J., Director/Retail (Aug 2026, Capterra): "switched from A2X — Pricing was more competitive and... the user interface is far superior."
- Dext Commerce → Link My Books: Jenny B., Owner/Consumer Goods (Jun 2025, Capterra): "it was more fiddly."
- Tradebox/"Blocks" → Link My Books: Steven P., Director/Retail (Apr 2026, Capterra): "more expensive and overly complicated in comparison."
- Link My Books → Taxomate: Mo K. (May 2025, Capterra): "sync is accurate... support incredibly responsive."
All four are named, dated, first-person accounts explicitly describing a completed move with a stated reason — not generic price/UI complaints without a confirmed migration, and not "alternative to X" marketing content.

### Switching destinations
A2X (founded 2014, ~12,000+ customers, widely described as the category's established leader) is the more entrenched incumbent; Link My Books (founded 2017, smaller Capterra review count) was the smaller specialist challenger winning switches on price/UI. **Material finding:** Visma (a large European accounting-software group) acquired Link My Books in January 2025 (globenewswire.com, primary press release, dated 2025-01-28). So the observed pattern is "incumbent → specialist," but the specialist is no longer fully independent — it now sits inside a larger platform, which is a relevant destination-pattern fact, not a switching-feasibility failure. Taxomate remains a smaller, lower-priced, independent "seller-led" alternative — a second specialist tier below both A2X and (now Visma-owned) Link My Books.

### Feasibility assessment
Switching between these tools is operationally feasible for the identified small-to-mid seller: reconnecting marketplace/accounting APIs is standard self-serve OAuth, no meaningful contractual lock-in exists, and the real friction (rebuilding account mappings/tax rules) is bounded, documented, and — in Link My Books' case — actively reduced by a vendor-provided free migration service. Four distinct, named, dated, first-person completed switches are documented across different source products, all converging on a specialist destination. The main caveat is that the specialist destination (Link My Books) has itself now been absorbed into a larger corporate group, a fact worth carrying forward as a destination-pattern observation.

### Gate result
**PASS**

### Remaining unknowns
No vendor-published migration guide was found for Dext Commerce ↔ A2X or any path directly involving Taxomate. No independent (non-vendor) first-person account of migration time/effort exists — the most detailed procedural evidence comes from Link My Books itself, which has an incentive to make switching-in look easy. No quantified data on how many total sellers have completed switches (only qualitative reviewer counts).

---

## Candidate 3 — Tax Practice Client Document/Engagement Workflow Portal

### Buyer
Small US tax preparation/accounting firms (solo practitioners to small teams) — owners, partners, bookkeepers, staff accountants.

### Existing solution
TaxDome, Canopy, SmartVault (all previously confirmed demo-gated at purchase in `PAYMENT_GATE.md`); Financial Cents (the confirmed self-serve destination).

### Lock-in
Client-facing lock-in is real and **vendor-acknowledged**, not speculative. Financial Cents' own migration guide (a competing vendor's content, but the most operationally specific source found — financial-cents.com/resources/articles/top-taxdome-alternatives/, primary, last updated 2026-01-13) instructs firms leaving TaxDome to give clients "step-by-step instructions... for logging into the new portal, submitting documents, or completing tasks" and to "share the timeline for migration, including... deadlines for document submissions" — the client relationship itself, not just internal operations, has to be actively re-anchored to a new URL/login. TaxDome's own migration-guidance page (primary, taxdome.com/migration-guidance) independently lists "client disruption when introducing new systems or portals" as a top reason firms *hesitate* to switch (stated about switching TO TaxDome, but the friction is structurally symmetric for switching away). The same Financial Cents guide flags workflow automation as not cleanly portable, explicitly naming "pipeline stages, automations, and historical activity logs" as data to "archive or rebuild," not migrate. **Gap:** no first-person reviewer account (on any of the three incumbents' review pages) was found describing an actually-disrupted client relationship post-switch — the lock-in claim is vendor-stated, not buyer-confirmed.

### Data portability
- **TaxDome:** publishes only *import* documentation (help.taxdome.com/article/122-import; taxdome.com/migration-guidance, both primary) — no page describing export **out** of TaxDome was found. Individual documents are downloadable one at a time via the PDF viewer; no bulk/structured whole-portal export tool is documented. E-signature audit trails are viewable in-app (help.taxdome.com/article/232) but no export/download mechanism for the trail itself was found.
- **Canopy:** its own Terms of Service §11(a) (getcanopy.com/terms-of-service, primary, updated 2026-05-29) states Canopy "is not a provider of data back-up or archiving services" and the customer is "solely and exclusively responsible for backing up and archiving of all Client Content" — no export tool at all is documented.
- **SmartVault:** the only documented export is a client list to CSV (help.smartvault.com, primary) — names/contacts, not documents or e-signature history. Its own cancellation help article instructs users to manually download/back up documents locally before subscription end — a manual pre-cancellation scramble, not a formal export feature.
- **Conclusion:** documents can be manually downloaded/backed up from all three incumbents before leaving, but no vendor of the three, nor the confirmed destination (Financial Cents), documents migrating the whole client-portal configuration (automations, e-signature history, workflow templates) intact. This is "data can be exported," not "the operational system can be migrated" — the distinction the task asks to preserve.

### Contract / procurement friction
Directly verified on each vendor's own current ToS/policy pages (all accessed 2026-09-22) — all three incumbents share materially the same structure:
- **TaxDome** (Refund Policy, primary, modified 2026-05-06): "TaxDome does not provide refunds or credits for any service, subscription plan, firm balance, or usage credit." Plans are prepaid for 1-, 2-, or 3-year terms; cancellation only stops the *next* renewal, not the current prepaid term.
- **Canopy** (Terms of Service §10(d)–(e), primary, updated 2026-05-29): auto-renews for equal-length terms; "cancellation shall not become effective until the expiration of your then-current subscription term"; no refunds "including for any partially used subscription terms."
- **SmartVault** (Terms of Service, primary): "During the Initial Term, you may not cancel the Agreement except as expressly permitted... Fees for the Initial Term are non-refundable"; Initial Term = 1 year for annual plans, auto-renews unless cancelled ≥21 days before renewal.
**This is a real, vendor-confirmed, primary-sourced barrier**: a dissatisfied firm mid-term is contractually committed (and retains access) until the prepaid term ends — none of the three offers early termination or partial refund. This caps how fast switching intent can convert into an actual switch: only at renewal-date boundaries, not on demand.

### Integration / workflow rebuild
Rated **substantial**, based on convergent evidence from multiple sources:
- TaxDome's own migration-guidance page states "most firms complete TaxDome implementation in 6–8 weeks," even with a paid onboarding manager (from $299).
- Financial Cents' migration guide gives a phased timeline for leaving TaxDome: weeks 1–2 rebuild workflows/templates from scratch, weeks 3–4 staff training, month 2 migrate active clients/documents, month 3 full rollout — roughly a **quarter**, explicitly recommended to happen outside tax season.
- A Canopy reviewer (sourced via search-tool synthesis, not independently re-verified character-by-character on the live page — flagged as a minor sourcing caveat) reported paying for two months while investing "an enormous amount of time and effort" setting up Canopy before concluding the platform wasn't ready — informative on magnitude even though this describes adopting Canopy, not leaving it.
- A separate Canopy reviewer (same sourcing caveat) explicitly decided **not** to switch because "clients are already used to the client portal" — direct evidence that client-facing rebuild cost actively suppresses switching, not merely adds friction after the decision is made.
What needs rebuilding: client onboarding/engagement-letter templates, automated reminder/pipeline workflows, client-facing portal access. Billing/e-signature *integrations* specifically were not directly evidenced either way (rated unknown, not assumed trivial).

### Actual switching evidence
≥7 named, dated Capterra reviewers, all on **TaxDome's own review page**, describing a prior competitor before choosing TaxDome: Jenifer V. (Aug 2025, from Canopy — UI complaint), Joe K. (Oct 2025, from SmartVault and monday.com), Nancy A. (Jul 2025, from Progress ShareFile), Peggy B. (Dec 2025, from Karbon), Ivette C. (Dec 2025, from SafeSend, GoFileRoom, and PracticeSuite simultaneously), Andrew S. (Oct 2025, from Keap), Lakisha W. (Feb 2026, from Onboardible). One counter-example on **Financial Cents' own review page**: Megan C. (Oct 2025), switched FROM TaxDome TO Financial Cents. All are named, dated, first-person, and describe a completed move — meeting the bar for actual switching evidence, not dissatisfaction alone.

**Central caveat — survivorship/destination bias, directly investigated:** a dedicated search pass looked for *independent* (non-destination-vendor-hosted) evidence of firms leaving Canopy, SmartVault, ShareFile, Karbon, SafeSend, GoFileRoom, PracticeSuite, Keap, or Onboardible. Multiple Reddit searches (r/taxpros, r/accounting, naming each competitor) returned **zero** relevant threads — a genuine negative result after real effort, not an unexplored gap. Canopy's and SmartVault's own Capterra pages show dissatisfaction (pricing/UX complaints) but no reviewer confirming a completed move to a named destination. **Every piece of switching evidence for this entire candidate, on both sides, is hosted on some vendor's own review funnel** — TaxDome's page for the ≥7 switches-in, Financial Cents' page for the 1 switch-out. This is a stronger and more specific finding than Discovery's original caveat: it is not merely "TaxDome's page is biased toward TaxDome," it is that the category's entire switching-evidence base is vendor-funnel-concentrated.

### Switching destinations
TaxDome, Canopy, SmartVault, ShareFile, and Karbon are all established, entrenched players. Per `BASELINE.md` §8's explicit rule, observed migrations between already-entrenched incumbents must be recorded as a **distribution/entry risk**, not reinterpreted as an opportunity. Financial Cents is the one exception in the data — an established, funded specialist vendor, not a solo-built product, but smaller than TaxDome.

### Feasibility assessment
This candidate presents a genuinely mixed picture rather than a clean pass or fail. On one hand: real, named, dated, first-person completed switches are documented on both sides (≥7 in, 1 out), data can be manually downloaded before leaving, and a viable, independently-confirmed self-serve destination exists (Financial Cents). On the other hand: contract terms are a real, primary-source-confirmed barrier that gates switching to renewal-date boundaries; the rebuild is substantial (6–8 weeks to ~3 months, per the vendors' own numbers) and includes real client-facing disruption risk (vendor-acknowledged, and shown to actively deter at least one reviewer from switching at all); and — the specific risk this task asked to investigate — every piece of switching evidence, without exception, comes from a destination vendor's own review funnel, with a dedicated independent search finding zero corroboration elsewhere. This combination — real but timing-gated and costly feasibility, plus a switching-evidence base that could not be independently corroborated despite deliberate effort to do so — falls short of a clean PASS.

### Gate result
**BLOCKED / INCONCLUSIVE**

### Reason
Meaningful switching signals genuinely exist (≥7 dated, named, first-person completed migrations), but destination/independence evidence is insufficient: 100% of the switching evidence for this candidate is hosted on a destination vendor's own review page, and a dedicated search for independent corroboration (Reddit, competitor review pages) returned nothing. Combined with real, primary-source-confirmed contract-timing and substantial-rebuild friction, this does not meet the bar for PASS, but neither does it meet the bar for KILL — switches are documented as actually happening, just not independently verifiable as representative of ease-of-leaving specifically. This is not a structural-barrier KILL; it is an evidentiary-sufficiency BLOCKED/INCONCLUSIVE.

### Remaining unknowns
Whether any first-person account exists anywhere of a client being confused/lost during a firm's platform switch. Whether e-signature audit trails can be bulk-exported from any of the three incumbents (only in-app viewing confirmed). Whether billing/payment integrations specifically survive a switch. Whether SmartVault's month-to-month option (implied by its cancellation help article) is available to typical solo/small-firm customers, given its ToS default is a 1-year Initial Term.

---

## Candidate 4 — eBay/Etsy Cross-Listing & Listing-Template Management

### Buyer
Long-tenured eBay/Etsy power sellers and small multichannel resellers who pay monthly for a listing-management/template subscription.

### Existing solution
InkFrog (Wix-owned, dominant incumbent — announced shutdown April 29, 2026, effective June 1, 2026); LitCommerce, FolderLister, Sixbit as named destinations; 3Dsellers, Nembol, SpareDollar/"Rescue" as additional destinations surfaced specifically in the forced-migration thread.

### Lock-in
InkFrog's own shutdown email (April 29, 2026, quoted verbatim by both independent trade press and sellers who forwarded it into the eBay Community) offered exactly two things: CSV export of listing data until May 31, 2026, and a prorated refund of unused billing days — nothing else (no template-HTML export, no bulk-image export, no named migration partner). Two lock-in mechanisms independently confirmed:
- **Image hosting:** the CSV export contains image *URLs* pointing at InkFrog's own CDN (`imgs.inkfrog.com`), not the image files themselves. Named eBay Community user **Mathias7** (primary, ~2026-05-07): "I can download an account csv with my listing data... but there's no image download/backup option. I hate how you get locked into tools like this."
- **Template self-containment:** per an independent trade-press retrospective, live eBay listing HTML built with InkFrog templates referenced InkFrog-hosted images/CSS/scripts — when InkFrog's servers went dark June 1, every listing using those templates broke simultaneously, not gradually (a vendor blog with a commercial conflict of interest also describes this mechanism, but the technical claim is independently plausible and consistent with community accounts).
No evidence was found describing eBay/Etsy marketplace API re-authorization itself as a friction point (an open gap, not confirmed either way).

### Data portability
InkFrog itself provided only the bare CSV (text fields), and even that was clumsy in practice — eBay Community user **moo_cow_corner** (primary, ~2026-06) describes exporting the "Library" (drafts) separately from the main CSV, 50 listings at a time, page by page. Because InkFrog provided no image export, third parties filled the gap unprompted before shutdown: SpareDollar/"Rescue" (built post-announcement by an InkFrog co-founder), Nembol, and a hobbyist tool pulled images via the CSV's URLs while InkFrog's CDN was still live — named user **saturdaystoys** (primary, ~2026-05) confirms this worked: "Over 10,000 inkFrog listings... and over 60,000 accompanying photos... DONE within 30 minutes." One user (**jim1024**, primary) asks, unanswered in-thread, whether sold/unsold library history was fully captured — genuinely unresolved.

**Confirmed for two of the three named destinations:** an eBay-API-direct import path exists that needs no InkFrog cooperation at all. FolderLister's own product page documents: "Open Manage Listings, let your active eBay listings load, and use Add selected" — pulling directly from eBay, not from InkFrog. LitCommerce's own product page describes CSV import plus a separate paste-based "Import from InkFrog" template re-import. This means *active* eBay listings can often be reclaimed without InkFrog's cooperation — a genuine reduction in switching cost versus a typical SaaS-to-SaaS migration. It does **not** rescue InkFrog-hosted template design/CSS or description images not already resolved on eBay's own CDN. No InkFrog-specific import feature was found for Sixbit (unconfirmed).

### Contract / procurement friction
No evidence of an annual contract or minimum-term clause blocking InkFrog cancellation was found; the shutdown email's promise of a per-day prorated refund is itself evidence InkFrog ran rolling/monthly billing. The forced shutdown makes this question largely moot for InkFrog specifically. A different, unexpected friction point surfaced on the **destination** side: **saturdaystoys** (primary, ~2026-05) reports a "meltdown" trying to cancel a 3Dsellers trial: "Customer service is managed only by a 'bot'... Tried to cancel my 7-day trial subscription... but failed." This is real onboarding/cancellation friction, but it belongs to one destination vendor (3Dsellers), not to leaving InkFrog, and was not found for LitCommerce, FolderLister, or Sixbit specifically.

### Integration / workflow rebuild
Evidence is mixed and splits by the path taken:
- **Template/design rebuild:** substantial, unless routed through LitCommerce's InkFrog-template importer (a vendor claim, not independently confirmed by a first-person account praising that specific feature) or a pre-shutdown rescue tool.
- **Item-specifics mapping:** one genuine first-person positive account — **lit1213** (primary, voluntary-switch thread): "Personally I use folderlister... Re-use profiles with pre set item specifics... works very well for my big Collection of postcards."
- **Image hosting:** recoverable only if a CSV+image rescue was done before May 31, 2026, or if photos already resolved on eBay's own CDN.
- **Cross-listing sync/automation rebuild:** no first-person account found either way (a gap).
- Outcomes range from easy (**myshoppingtree**, primary, 24-year seller, moved to 3Dsellers: "the migration has been a very positive experience... a fairly easy transition") to effectively abandoned rather than migrated (**funfactorychannel**, primary, 10-year InkFrog user: "I am giving up on the photo and data. I will just retake pictures and re-search as needed.").
**Rating: moderate for basic listing continuity** (via eBay-API re-import), **substantial/lossy for full-fidelity template+image migration** without proactive rescue action taken before the CDN went dark.

### Actual switching evidence
**Voluntary** (eBay Community thread "Inkfrog alternatives?", original post dated 2022-11-29, confirmed via page metadata — years before the shutdown): organic complaint "inkfrog has so many issues now I can't even list correctly." Destinations named by actual users, not just recommenders: **andy.johns_4** switched to LitCommerce ("found it on the Shopify app store... pretty smooth for syncing so far"); **lit1213** switched to FolderLister (quoted above). Caveat: the specific *replies* naming these destinations are dated ~May 2026 — after the shutdown announcement — so they cannot be cleanly certified as untainted by shutdown urgency, even though the original complaint clearly predates it.

**Forced** (thread "Inkfrog to shut down," started directly in response to the shutdown email): a wider destination set — SpareDollar/Rescue, 3Dsellers, Nembol, Sixbit, plus others — with LitCommerce and FolderLister notably **absent** from this thread. Forced migrators show more acute image/data-loss anxiety and more destination-onboarding friction (the 3Dsellers cancellation issue above) than the voluntary thread's brief "pretty smooth" account.

A second, independent forced-migration data point (different incumbent, same pattern): a named LitCommerce Trustpilot review (dated 2026-09-20, primary): "We were a long term user of Codisto Linq/Marketplace Connect, which suffered... a catastrophic failure on 6/8/26... within a week of pressing the big green 'GO' button, we are fully operational." Confirms a "catastrophic incumbent failure → forced migration → LitCommerce, about a week to operational" pattern outside InkFrog specifically — this reviewer is a Shopify/marketplace-apps seller, not a classic InkFrog template user, so it corroborates the general forced-migration pattern more than it measures InkFrog-specific rebuild cost.

None of the cited evidence is a mere "alternative to X" marketing page or an unfulfilled feature request — all are first-person accounts of a completed or actively-underway move.

### Switching destinations
LitCommerce, FolderLister, Sixbit, 3Dsellers, Nembol, and SpareDollar are all small/specialist vendors — none is an entrenched dominant incumbent, and none of the observed destinations is Wix's own tooling or eBay's/Etsy's own native listing tools. This is the pattern §8 treats as more favorable than incumbent-to-incumbent churn: switchers are moving away from a dominant (now-defunct) incumbent toward multiple small, competing specialist tools. Gap: no direct search was run for whether any meaningful fraction of InkFrog's base migrated to a major platform's built-in tools instead of any specialist vendor.

### Feasibility assessment
Lock-in and portability friction are real but bounded and partially mitigable: CSV export existed (if clumsy), eBay-API-direct re-import bypasses InkFrog's cooperation entirely for at least two of the three named destinations' live listings, and multiple named forced *and* voluntary migrators completed switches, several describing the process as easy. Procurement/contract friction is moot for InkFrog (forced shutdown, no restrictive terms found) though real for at least one destination (3Dsellers' cancellation issue) — a destination-specific risk, not a leaving-InkFrog risk. Realistic alternatives clearly exist and have named, paying/active users (LitCommerce's paid status independently confirmed in `PAYMENT_GATE.md`). Switching destinations are specialist vendors, not entrenched incumbents.

### Gate result
**PASS**

### Remaining unknowns
Whether eBay/Etsy API re-authorization itself is a friction point. Whether Sixbit has any InkFrog-specific import path. Whether LitCommerce's template-importer is as smooth in practice as the vendor claims (no first-person account found praising that specific feature). Whether any InkFrog users migrated to a major platform's native tools rather than a specialist vendor. Whether SpareDollar's "Rescue" data (sold/unsold history) was ever confirmed complete.

---

## Cross-Candidate Observations

*Methodological patterns only — no opportunity judgment, ranking, or score.*

- **Switching is genuinely common between accounting/reconciliation-style tools (Candidates 1 and 2), and comparatively harder in workflow/document-portal-style tools (Candidate 3).** In both Insurance Commission Reconciliation and Multichannel E-Commerce Accounting Reconciliation, the underlying task is data reconciliation against external, third-party-controlled sources (carrier statements; marketplace settlements) that live outside either the old or new tool — switching mainly means reconnecting to those external sources and rebuilding mapping rules, not migrating an internal system of record. In the Tax Practice Client Portal, the tool itself *is* the system of record for client relationships, documents, and workflow history, and that data is shown (via primary ToS/help-center sources) to be much less portable. This is a structural difference in what kind of tool is being switched, not a difference in vendor goodwill.
- **Forced migration (Candidate 4, InkFrog) behaves differently from dissatisfaction-driven voluntary switching, with different destination sets.** The same underlying candidate produced two visibly different migration patterns: a small, narrow voluntary-switch group before the shutdown (destinations: LitCommerce, FolderLister) and a larger, more anxious forced-migration group after it (destinations: SpareDollar/Rescue, 3Dsellers, Nembol, Sixbit — notably not overlapping with the voluntary group's top two choices). Treating "people switched" as one undifferentiated signal would have hidden this.
- **A destination vendor's own review page is not independent evidence of ease-of-leaving a different, named incumbent — this is a real and, in one candidate (Tax Practice Portal), category-wide limitation.** Multiple candidates relied on Capterra reviews hosted on the *destination* vendor's page describing a prior *source* product. This is legitimate first-person switching evidence (a real named person describing a real completed move), but it is not independent confirmation that leaving the source product specifically is easy — only that arriving at the destination succeeded. In Candidates 1, 2, and 4, at least some corroborating evidence existed off the destination vendor's own page (forum threads, independent trade press, Trustpilot). In Candidate 3, a dedicated search for such corroboration returned nothing at all — the entire evidence base for that candidate is destination-page-hosted, which is why that candidate did not clear this gate cleanly.
- **All observed switching destinations across all four candidates are small/specialist vendors, not entrenched dominant incumbents (with one partial exception).** Per §8's explicit rule, incumbent-to-incumbent churn would need to be flagged as a distribution/entry risk rather than an opportunity signal; that pattern was not found here. The one partial exception is Link My Books (Candidate 2's dominant destination), which — while still smaller than A2X — was acquired by Visma, a large accounting-software group, in January 2025, meaning the "specialist" destination is no longer fully independent. This is recorded as a destination-pattern fact for possible Distribution-stage relevance, not reinterpreted as a switching-feasibility problem here.

---

## Next Research

*Only the next gate to investigate is named below — it is not performed in this task.*

- **Insurance Commission Reconciliation (PASS):** eligible for Distribution Evidence (`BASELINE.md` §9).
- **Multichannel E-Commerce Accounting Reconciliation (PASS):** eligible for Distribution Evidence (`BASELINE.md` §9) — the Link My Books/Visma acquisition fact from this pass should inform how that candidate's distribution channels are read.
- **eBay/Etsy Cross-Listing & Listing-Template Management (PASS):** eligible for Distribution Evidence (`BASELINE.md` §9) — the forced-vs-voluntary destination split from this pass (LitCommerce/FolderLister vs. SpareDollar/3Dsellers/Nembol/Sixbit) should inform which specific channel is investigated.
- **Tax Practice Client Document/Engagement Workflow Portal (BLOCKED/INCONCLUSIVE):** does not advance to Distribution yet. The specific open question to resolve first is the one this pass could not close — independent (non-destination-vendor-hosted) confirmation that firms can and do leave Canopy, SmartVault, ShareFile, Karbon, SafeSend, GoFileRoom, PracticeSuite, Keap, or Onboardible. Until at least one such independent account is found, or the contractual-timing/rebuild-cost friction found here is otherwise resolved, this candidate should not be carried into Distribution research on the strength of its current switching evidence alone.
