# Discovery Pass

## Scope

- **Date:** 2026-09-22
- **Research objective:** Discover a small set of problem domains (not product ideas) with observable evidence of a specific buyer, existing spending/allocated labor, an existing paid solution, and recent dissatisfaction/switching signals — testing whether the patched methodology in `BASELINE.md` v2 can reliably surface such domains.
- **Method:** Four parallel, independently-run research passes, each assigned a different sector cluster to maximize source diversity and avoid overfitting to one "loud" industry: (1) regulated professional services (accounting/tax/law/insurance back-office), (2) local/trades and field operations (HVAC/plumbing/property management/construction/restaurants), (3) solo/small professional operators (recruiters, real-estate agents, insurance agents), (4) e-commerce and platform-ecosystem operations (Shopify/Amazon/eBay/Etsy sellers). Each pass used two parallel source classes (Class A and Class B, below), classified every signal per `BASELINE.md`'s taxonomy, and applied the Existing Spending tier hierarchy and the Free-Incumbent Trap. All evidence below was gathered via live WebSearch/WebFetch against real, dated sources — no candidate was invented or reverse-engineered from a product idea.
- **What was explicitly not researched:** the Payment Plausibility Gate, the Switching Feasibility Gate, and the Distribution Gate were **not** run to completion for any candidate — those are later-phase gates per the canonical chain in `BASELINE.md` §4. No niche, marketplace, platform, or product/wedge was selected. No scoring, weighting, or ranking was produced.

---

## Source Classes

### Class A — Dissatisfaction / Switching

Used across the four passes: Capterra/G2/TrustRadius/Trustpilot reviews (filtered for switching/migration language, not star ratings alone), named first-person migration accounts, vendor-neutral trade press (e.g. valueaddedresource.net, LawNext), platform-native community threads (eBay Community forum), and vendor customer-story press releases (used only where explicitly labeled non-independent). Every signal was classified as one of: complaint / recurring dissatisfaction / comparison / migration / replacement intent / actual switching. Feature requests and "alternative to X" pages were treated as, at most, lead sources — never as independent demand evidence — per `BASELINE.md` §11.

### Class B — Spending / Behavioral

Used across the four passes: vendor pricing pages (verified directly, not taken from secondary aggregators where avoidable), live job postings (Indeed/Upwork) for recurring roles tied to a specific workflow, dedicated staffing/gig marketplaces for a specific labor gap (e.g. VPM Solutions), and named contractor/service pricing (flat-fee transaction coordinators, contingency-fee auditors). Lost revenue, hypothetical opportunity cost, vague "takes a lot of time" claims, and market-size/search-volume figures were explicitly excluded as evidence throughout, per the Existing Spending hierarchy in `BASELINE.md` §5.

---

## Candidates

### Candidate 1 — Insurance Commission Reconciliation (Independent P&C/Multi-line Agencies)

*Surfaced independently by two separate research passes (regulated-services and solo-operator) without coordination; merged below.*

#### Problem domain
Independent insurance agencies must match commission payments received from carriers against what their book of business says they're owed ("commission reconciliation"), reconciling written/paid/earned amounts across dozens of inconsistent carrier statement formats (CSV, Excel, PDF) every month — typically run in Excel until transaction volume makes that unworkable.

#### Buyer
Independent US P&C/multi-line insurance agencies and individual agents — specifically finance/operations staff (bookkeepers, controllers, finance coordinators, agency principals/administrators) responsible for monthly carrier-statement reconciliation. Precise firm-size threshold: UNKNOWN, though the leading paid tool explicitly prices separate tiers for "independent agents," "small agencies," and "medium agencies."

#### Existing paid solution
Multiple paid, purpose-built incumbents: Commission Tracker ([commission-tracker.com/pricing](https://commission-tracker.com/pricing/) — $67/mo independent agents, $72–187/mo agency tiers, confirmed on its own pricing page and via Capterra); Commission Wizard ($23–79/mo, own pricing page); AgencyBloc AMS+; Insurstein/CommissionSight (named as competitors in reviews, pricing not independently verified); and, for larger agencies already on an AMS, Applied Recon, a paid add-on inside Applied Epic (Applied Systems).

#### Existing spending
**Strong.** Commission Tracker and Commission Wizard both have publicly visible, tiered, recurring monthly pricing explicitly segmented down to the solo/independent-agent level, and named, dated reviewers confirm real ongoing paid usage. Applied Recon is a paid add-on to an AMS agencies already license, with named customer case studies of adoption.

#### Class A evidence
- Capterra, Commission Tracker for Insurance reviews ([capterra.com/p/88991/Commission-Tracker-for-Insurance/reviews/](https://www.capterra.com/p/88991/Commission-Tracker-for-Insurance/reviews/)), sampled independently in both passes:
  - Five named reviewers dated Sept 8–17, 2026 (Commissions Specialist, Executive VP, VP, Managing Partner, Agency Owner): one reviewer's paraphrased history — "prior to CT, an excel spreadsheet was my recording method" — another describing a prior "commission process was a mess" with "leaks throughout" before adopting the tool. Signal: **migration** (manual process → paid tool).
  - "Ben T." (President, Financial Services, independent agency; date on record Aug 2024 — flagged by the researcher as not independently re-verified character-by-character): "After 1,000 sales in Excel, the matrix slowed down to a crawl" — switched from Excel. Signal: **actual switching**.
  - "Kathy B." (agency administrator; date on record Sept 2026, same date-reliability caveat): switched from **AgencyBloc AMS+**, citing cost and ease of use. Signal: **actual switching between two paid products**.
- Applied Systems / Manger Insurance press release, GlobeNewswire, July 29, 2026: direct quote from Kalyn Murphy, Finance and Operations Coordinator: "It used to take me at least two to three days every month digging through commission statements." Signal: migration/replacement intent, but vendor-published, not independent.

#### Class B evidence
Commission Tracker and Commission Wizard pricing pages (Strong — visible recurring pricing, corroborated by independent named reviewers actually using the tools). Kalyn Murphy's self-reported "2–3 days/month" labor estimate, tied to a documented switch to a paid tool (Medium — self-estimated by the affected person, but sourced from a vendor press release, so independence is limited). Vendor-claimed "40–80 hours/month" industry-wide figures (repeated across multiple vendor blogs) are explicitly **not used as evidence** — marketing copy, not self-reported by an affected buyer.

#### Freshness
Mixed: several Commission Tracker reviews dated Sept 2026 (fresh); one ("Ben T.") dated Aug 2024 (older than 12 months, flagged); Applied Systems case study dated July 2026 (fresh but vendor-published).

#### Source independence
Two distinct chains: (1) Commission Tracker Capterra reviews — genuinely independent named reviewers, though all drawn from one platform, and the two research passes happened to sample different individual reviews from the same product page without coordinating — treated as a mild corroborating signal, not double-counted as more sources than it is. (2) Applied Systems press releases/blog — a single vendor's PR content, one evidence chain, not multiple independent confirmations.

#### Switching signal
**Actual switching** — both manual-process-to-paid-tool and paid-tool-to-paid-tool movement independently observed.

#### Switching destination
Manual/Excel process → standalone SaaS (Commission Tracker, Commission Wizard); AgencyBloc AMS+ → Commission Tracker; or AMS-embedded add-on (Applied Recon) for larger agencies already on Applied Epic.

#### Buyer publicness
Partially public — Capterra reviews exist and are informative, but no active independent Reddit/forum discussion of this specific pain point was found in either research pass.

#### Distribution hypothesis — UNVERIFIED
Independent Insurance Agents & Brokers of America (Big "I") state/national association channels, AMS-specific user communities (e.g. Applied Systems user groups), and insurance FMO/IMO marketing hubs that reportedly publish "best commission tracking software" buyer's guides.

#### Unknowns
Whether pain concentrates below a size threshold that can't justify an AMS-embedded solution; whether standalone tools win primarily on price or on carrier-format coverage; a genuinely independent (non-vendor, non-Capterra) account of switching friction.

#### Why investigate further?
Two independently-run research passes, using different search strategies, converged on this domain without coordination, and both found multiple paid competitors with real, dated, named-reviewer evidence of the exact manual-to-paid and paid-to-paid migration pattern.

---

### Candidate 2 — Tax Practice Client Document/Engagement Workflow Portal

#### Problem domain
Small tax and accounting firms need a system to collect client documents, manage engagement workflow (organizers, e-signatures, intake), and communicate with clients — replacing scattered email/file-sharing with a structured client portal.

#### Buyer
Small US tax preparation/accounting firms (solo practitioners up to small teams; exact size threshold UNKNOWN), specifically owners, partners, bookkeepers, and staff accountants selecting practice-management/client-portal software.

#### Existing paid solution
TaxDome ([taxdome.com/pricing](https://taxdome.com/pricing) — Essentials $800/yr solo, Pro $1,000/yr, Business $1,200/yr, per seat, 1-yr commitment), Canopy ($74–149/user/mo plus consumption add-ons), SmartVault (~$480/user/yr). All confirmed via pricing pages/aggregator summaries.

#### Existing spending
**Strong.** All three products have publicly visible, identifiable per-seat recurring pricing, and dozens of dated, named Capterra reviews confirm actual paid usage and active switching between them.

#### Class A evidence
Capterra, TaxDome reviews ([capterra.com/p/186749/TaxDome/reviews](https://www.capterra.com/p/186749/TaxDome/reviews)), sampled across multiple pages, named reviewers with roles and dates, all within roughly the last 13 months:
- Jenifer V., Partner/Accounting, Aug 27, 2025: switched from Canopy — "User interface was the biggest reason for leaving. They were not user friendly." Also a pricing complaint about per-user cost.
- Joe K., Staff Accountant, Oct 23, 2025: switched from SmartVault and monday.com, consolidated both into TaxDome.
- Nancy A., CPA/Founder, Jul 4, 2025: switched from Progress ShareFile.
- Peggy B., Founder/CEO, Dec 29, 2025: switched from Karbon.
- Ivette C., Administrative Assistant, Dec 22, 2025: switched from SafeSend, GoFileRoom, and PracticeSuite simultaneously.
- Andrew S., Tax Associate, Oct 23, 2025: switched from Keap.
- Lakisha W., Enrolled Agent, Feb 1, 2026: switched from Onboardible; separately: "pricing is high to add additional users... fees are constantly increasing."
- Kyle A., Owner, Aug 5, 2026: "High pricing for a solo-practitioner firm."

Signal classification: **actual switching** (≥7 independently-reported, dated migrations from named competing paid products), plus separate **recurring dissatisfaction** (pricing complaints) among both switchers and non-switchers.

#### Class B evidence
TaxDome, Canopy, and SmartVault pricing pages (**Strong** — visible recurring per-seat pricing). Reviewer-confirmed real paid usage across ≥7 independent firms switching between named paid competitors within roughly the last 13 months. **Strong.**

#### Freshness
≤12 months for nearly all cited reviews (Jul 2025–Aug 2026); one (Jenifer V., Aug 27, 2025) is just over 12 months from today but close.

#### Source independence
Genuinely independent — each review is a distinct named reviewer/firm on Capterra's verified-review system, not syndicated from one story. Caveat: all reviews were pulled from TaxDome's own Capterra page, so the sample is biased toward people who chose TaxDome as their destination (survivorship bias toward one destination — see Methodological Limitations).

#### Switching signal
**Actual switching** — the strongest and most repeatedly observed signal in the entire discovery pass, with named source products and a named destination documented across at least 7 independent, dated reviews.

#### Switching destination
Predominantly TaxDome, per the reviews (caveat: this reflects TaxDome's own review page, so it is not necessarily the modal destination industry-wide).

#### Buyer publicness
Public — active, detailed, dated review activity on Capterra.

#### Distribution hypothesis — UNVERIFIED
Capterra/Software Advice/G2 category pages themselves (where buyers are already actively comparing), and CPA/EA professional communities (e.g. r/taxpros, NAEA, AICPA PCPS forums).

#### Unknowns
Whether dissatisfaction concentrates around a specific workflow step (organizer collection, e-signature, billing) versus general practice management; true churn rate; whether recent TaxDome price increases (multiple reviewers cite "constantly increasing" fees) are creating a fresh wave of switching-out not visible on TaxDome's own review page.

#### Why investigate further?
This candidate has the strongest, freshest, most numerous independent actual-switching evidence found in this pass — at least 7 named, dated migrations between competing paid products within roughly the last year.

---

### Candidate 3 — Law Firm Trust Accounting / IOLTA Three-Way Reconciliation

#### Problem domain
Small law firms handling client funds must perform monthly "three-way reconciliation" of their IOLTA/trust account — matching the bank balance, the firm's book balance, and the sum of individual client ledger balances — a state-bar-mandated compliance task.

#### Buyer
Small US law firms (solo to small firm; exact size threshold UNKNOWN) subject to state bar IOLTA/trust accounting rules — attorneys, office managers, or firm CFOs responsible for trust compliance.

#### Existing paid solution
CosmoLex ($109–129/user/mo, built-in trust accounting), Clio Manage ($49–89+/user/mo, requires separate QuickBooks Online for full accounting), TrustBooks ($59–249/mo tiered add-on specifically for trust reconciliation, [trustbooks.com/pricing](https://trustbooks.com/pricing/)).

#### Existing spending
**Strong.** All three products have visible, identifiable recurring pricing, and dated reviews confirm actual paid adoption. A specific Upwork job posting titled "U.S. based bookkeeper for law firm (trust accounting) — ongoing part-time" was found, indicating recurring contractor spend, but the posting body could not be fetched (HTTP 403), so only the title/existence is confirmed, not budget/rate details.

#### Class A evidence
- Capterra, TrustBooks reviews ([capterra.com/p/145679/TrustBooks/reviews/](https://www.capterra.com/p/145679/TrustBooks/reviews/)): Quintina H., Attorney, Dec 1, 2020: previously used QuickBooks Enterprise; "the reconciliation process is done in a matter of minutes" now. Robert W., Partner, Nov 17, 2020: "What used to take hours a month now takes minutes," implied prior QuickBooks Enterprise use. Signal: **actual switching**, but **older than 12 months** (2020).
- Capterra, CosmoLex reviews ([capterra.com/p/18931/CosmoLex/reviews/](https://www.capterra.com/p/18931/CosmoLex/reviews/)), last 12 months: George G., Lawyer, Sept 26, 2025, 3★: retention driven by "integration with accounting," despite other frustrations — a **comparison**-type retention signal, not switching. Kathleen K., CFO, Apr 30, 2026, 1★: general software-quality complaint, not trust-specific. Two further 1-star reviews (2024–2025): general pricing/billing complaints, not trust-specific.
- Industry news: Clio ending its LawPay integration Aug 31, 2026 ([LawNext, May 2026](https://www.lawnext.com/2026/05/practice-management-platform-clio-to-discontinue-its-longtime-integration-with-payments-processor-lawpay.html)) — firms must re-evaluate their trust-adjacent payment workflow. A structural/forced-change event, not a user complaint; classified as **replacement intent context only**, not switching evidence per se.

#### Class B evidence
CosmoLex, Clio, and TrustBooks pricing pages (Strong). Upwork job posting for a recurring part-time law-firm trust bookkeeper (Medium — title/existence confirmed, rate/budget unverified due to fetch failure).

#### Freshness
**Mixed.** The clearest actual-switching evidence is older than 12 months (2020). General CosmoLex dissatisfaction is fresh (Sept 2025–Apr 2026) but not trust-accounting-specific. The Clio/LawPay integration-sunset event is fresh (2026) but is industry news, not a user complaint.

#### Source independence
Three distinct chains: (1) TrustBooks reviews — independent but old/sparse. (2) CosmoLex reviews — independent, recent, but not trust-specific. (3) Clio/LawPay trade press — appears to derive from a single company announcement covered by multiple outlets; treated as one evidence chain, not several independent confirmations.

#### Switching signal
**Actual switching** is the strongest signal observed (QuickBooks Enterprise → TrustBooks) but is dated 2020; the freshest signal within the last 12 months is only **recurring dissatisfaction** (CosmoLex, not trust-specific).

#### Switching destination
QuickBooks Enterprise → TrustBooks (per 2020 reviews). Bidirectional movement also referenced between Clio and CosmoLex in third-party comparison content, but not confirmed at reviewer-level with dates.

#### Buyer publicness
Mostly private/partially public — Capterra reviews exist but are sparse for the most specialized tool; no active Reddit/forum thread on this specific pain point was found.

#### Distribution hypothesis — UNVERIFIED
State bar association CLE/practice-management resource pages (several state bars publish trust-accounting software guidance) as a first-pass channel hypothesis.

#### Unknowns
Whether the trust-accounting pain point itself is fresh or a largely-solved niche (TrustBooks has existed since ~2015); true current switching volume; whether Upwork trust-bookkeeper demand is recurring/growing or a handful of one-off postings.

#### Why investigate further?
A state-bar-mandated, error-prone monthly compliance task with multiple existing paid incumbents at different price points — but freshness of the actual-switching evidence is the weakest of the professional-services candidates and should be re-verified before further investment.

---

### Candidate 4 — Real-Estate Transaction Coordination (Contract-to-Close)

#### Problem domain
Managing a real-estate transaction from executed contract to closing — tracking deadlines, collecting signatures/disclosures, coordinating with title/lender, and preparing the commission disbursement authorization — a compliance- and deadline-heavy workflow independent agents either run themselves in transaction-management software or pay a contractor to handle.

#### Buyer
Independent US real-estate agents and small brokerages doing roughly 10–40 transactions/year (either buying transaction-management software themselves, hiring a freelance/contract transaction coordinator, or both).

#### Existing paid solution
Software: dotloop, SkySlope, Brokermint, Paperless Pipeline. Contractor: independent freelance Transaction Coordinators (TCs) — e.g. AgentUp ($299/file), Empower Transactions ($400–500/file, $500/mo minimum), Gold Key TC ($369/file flat fee), and individually-listed Upwork TCs.

#### Existing spending
**Strong**, on two independent legs: (1) recurring software subscriptions with visible pricing; (2) contractor expenditure — standardized flat per-file TC fees of $300–$750 across multiple named providers, corroborated by live Upwork postings for ongoing ("6+ months") transaction-coordinator roles.

#### Class A evidence
Capterra, dotloop reviews ([capterra.com/p/136372/dotloop/reviews/](https://www.capterra.com/p/136372/dotloop/reviews/)): reviewers "Dan P." and "Russ C." reported switching away from **SkySlope** ("a total mess" per Russ C.); "Suzanne F.," "Maria C.," "Ali H.," "mark P." reported switching from **DocuSign**; "Tricia J." previously used **Form Simplicity**; "Deborah C." tried alternatives and returned to dotloop. Signal: **actual switching** (multiple named paid-to-paid moves). Same fetch also surfaced dissatisfaction (CRM integration gaps, mobile usability, one dated 2024).

#### Class B evidence
TC flat-fee pricing across three independently-operated providers (AgentUp, Empower, Gold Key TC) — **Strong**. Live, ongoing Upwork job postings for transaction-coordinator roles — **Strong** corroboration of recurring (not one-off) contractor demand. dotloop/SkySlope/Brokermint subscription pricing — **Strong**.

#### Freshness
Mixed/uncertain: one dotloop complaint explicitly dated 2024 (borderline-stale); TC pricing pages and Upwork listings appear current but exact posting dates weren't captured.

#### Source independence
The switching accounts (SkySlope, DocuSign, Form Simplicity) all come from one aggregator page/fetch — not independent *sources* of each other, though each names a different prior product. The TC pricing data comes from three genuinely independently-operated businesses.

#### Switching signal
**Actual switching** — dotloop reviewers explicitly named the prior paid tool they left.

#### Switching destination
Overwhelmingly to another entrenched incumbent (dotloop, an established platform with a vendor-claimed 150M+ processed transactions). **Per `BASELINE.md`'s Switching Feasibility rule, this is recorded as a distribution/entry risk, not an opportunity** — the observed churn is incumbent-to-incumbent and says nothing about whether an unknown solo-built entrant could capture any of it.

#### Buyer publicness
Partially public — large review volume on Capterra/G2 for the software leg; the TC/contractor leg is mostly transacted on Upwork/agency websites rather than publicly discussed.

#### Distribution hypothesis — UNVERIFIED
TC-specific communities/directories (referenced by vendor content, not independently verified), real-estate agent communities like BiggerPockets forums, or Upwork/Fiverr itself as a discovery surface for the contractor side.

#### Unknowns
Whether agents who hire a TC also separately pay for dotloop/SkySlope, or whether the TC brings their own software; exact freshness of the Upwork listings.

#### Why investigate further?
The only candidate with two independent, corroborating Strong-tier spending legs (software subscription + standardized contractor day-rate market) — though the incumbent-to-incumbent switching-destination pattern is a real caution flag that should be resolved before going further.

---

### Candidate 5 — Independent/Small-Agency Recruiting ATS-CRM Switching

#### Problem domain
Independent recruiters and small staffing/search agencies (roughly 1–10 seats) manage candidate pipelines, client records, and placements in an ATS/CRM, and repeatedly hit friction with per-seat pricing that scales poorly with headcount, contract lock-in, and support/usability complaints on the dominant enterprise incumbent, prompting moves to smaller, cheaper, more flexible vendors.

#### Buyer
Independent (self-employed) recruiters and small staffing/search-agency owners/directors, typically 1–10 seats, who choose and pay for their own ATS/CRM.

#### Existing paid solution
Bullhorn (dominant incumbent, $99–165/user/month published tiers). Also Loxo, Crelate, Recruiterflow, Recruit CRM, Zoho Recruit, CATS — all paid competitors with visible pricing.

#### Existing spending
**Strong.** Visible, recurring per-seat SaaS pricing across the whole category.

#### Class A evidence
Capterra, Recruit CRM reviews ([capterra.com/p/174348/Recruit-CRM/reviews/](https://capterra.com/p/174348/Recruit-CRM/reviews/)): multiple reviewers reported switching from **Bullhorn**, described as "difficult and expensive and not customer friendly." "Jeff M." (Co-Founder, small agency): switched from Bullhorn citing "cost point vs long term growth vs ease of use." Other reviewers reported switching from Salesforce, Loxo, CATS ("product stagnation"), Voyager Infinity, Firefish, RESUMate. "Nicky C." (Director, self-employed/independent recruiter) valued Recruit CRM's "monthly rolling contract option," contrasted against "everyone else seems to want 12 months commitment." A separate Recruiterflow review noted a switch from Salesforce Sales Cloud ("too manual"), and a separate Bullhorn review noted a switch *to* Bullhorn from "Prospect CRM" — evidence flows in both directions and is reported honestly rather than cherry-picked.

#### Class B evidence
Bullhorn published per-seat pricing (**Strong**). Multi-seat annual contract minimums reported in a vendor-comparison article were **not independently verified** and are treated as lead/background only, not standalone Class B evidence. "Nicky C."'s explicit shopping on payment-term flexibility is a weak corroborating signal that solo buyers actively evaluate contract terms, not just price.

#### Freshness
UNKNOWN for the specific switching quotes — the Capterra fetch did not return clean per-review dates for Recruit CRM. Category-level pricing reflects current 2026 data.

#### Source independence
The Bullhorn-switching mentions all come from one aggregator page/fetch — one evidence chain from one page, not several independent sources, though each names a different reviewer.

#### Switching signal
**Actual switching** — multiple reviewers explicitly name Bullhorn (and other tools) as what they left, with stated reasons.

#### Switching destination
Mixed — some move to mid-market challengers (Recruit CRM, Recruiterflow) rather than another giant, and some move *to* Bullhorn from smaller tools. Healthier than the real-estate candidate, but still established SaaS vendors, not confirmed capture by a brand-new solo-built entrant.

#### Buyer publicness
Public — the most vocal segment among the solo-operator sector; switching reasons are stated explicitly and specifically.

#### Distribution hypothesis — UNVERIFIED
r/recruiting and other recruiter-specific communities, RecruitingDaily, Top Echelon network for split-fee independent recruiters.

#### Unknowns
Exact review dates; how much "switching from Bullhorn" volume comes from truly independent/solo recruiters vs. mid-size staffing firms (possible enterprise/SMB mismatch, since Bullhorn skews toward larger agencies); whether a narrower sub-problem inside this category (e.g. duplicate-candidate handling across job boards) would be a tighter domain than "ATS switching" broadly.

#### Why investigate further?
The most explicit, named, reason-stated switching quotes of any candidate in this pass, and uniquely shows switching flowing to non-giant vendors as well as away from them — but the domain as scoped is closer to a whole software category than one narrow problem.

---

### Candidate 6 — Multichannel E-Commerce Accounting Reconciliation

#### Problem domain
Reconciling marketplace/platform settlement data (Amazon, Shopify, eBay, Etsy, Walmart payouts — sales, fees, refunds, shipping, taxes) into accurate summarized journal entries that match actual bank deposits, for bookkeeping/COGS/tax purposes — the "settlement-to-ledger" matching workflow, not general bookkeeping.

#### Buyer
Small-to-mid multichannel e-commerce sellers (roughly 100–20,000+ orders/month per the tools' own pricing tiers, selling across 2+ of Amazon/Shopify/eBay/Etsy/Walmart) and the outsourced or in-house bookkeepers/accountants who manage their books on Xero/QuickBooks Online.

#### Existing paid solution
A2X ([a2xaccounting.com](https://a2xaccounting.com)) — dominant incumbent, paid plans from $29/month, no permanent free version. Named competitors sellers are actively paying for instead: Link My Books ($21–$176+/month, usage-based), Taxomate, Dext Commerce, Tradebox/"Blocks."

#### Existing spending
**Strong.** Visible recurring subscription pricing on both the incumbent and the tools people switch to, confirmed via named, dated customer reviews from paying users.

#### Class A evidence
Capterra, Link My Books reviews ([capterra.com/p/184768/Link-My-Books/reviews/](https://capterra.com/p/184768/Link-My-Books/reviews/)): Aaron J., Director/Retail (Aug 2026, 5★): switched from A2X — "Pricing was more competitive and to be honest the user interface is far superior." Erin S., Accounts Assistant (Apr 2026, 5★): "Cheaper and the user interface was a lot easier to understand" — left A2X. Victoria K., Director/Retail (May 2026, 5★): "I got more for my money, when functionality was pretty much the same" — vs. A2X. Jenny B., Owner/Consumer Goods (Jun 2025, 5★): switched from Dext Commerce, "it was more fiddly." Steven P., Director/Retail (Apr 2026, 5★): switched from Tradebox/Blocks, "more expensive and overly complicated in comparison." Older reviews (2021, 2023) show the same pattern going back years.

#### Class B evidence
A2X pricing (from $29/mo scaling to ~$899/mo by order volume) and Link My Books pricing ($21–176/mo, plus a July 2026 price increase) — both **Strong**, and both directly confirmed as actually paid by the named reviewers above.

#### Freshness
Mixed but recent-dominant: most switching reviews are Jun 2025–Aug 2026 (≤12 months), with a long tail back to 2021 showing the pattern is not new.

#### Source independence
All reviews pulled from Capterra, but each is an independent, named, dated submission from a different company/role — genuinely independent accounts, not cross-posts of one story.

#### Switching signal
**Actual switching** — multiple first-person, named, dated accounts of moving from A2X/Dext Commerce/Tradebox to a named competitor.

#### Switching destination
Link My Books (from A2X, Dext Commerce, and Tradebox/Blocks).

#### Buyer publicness
Public — reviews posted openly on Capterra/G2/GetApp, and comparison content widely written about by vendors and third parties.

#### Distribution hypothesis — UNVERIFIED
QuickBooks Online / Xero app marketplaces, Shopify App Store and Amazon Selling Partner Appstore listings, and ecommerce-bookkeeper communities (e.g. accountant/bookkeeper Facebook groups specializing in ecommerce).

#### Unknowns
How much switching is purely price-driven vs. a real accuracy/reliability problem with A2X; how sticky reconciliation tooling is once wired into a client's chart of accounts.

#### Why investigate further?
The one candidate with documented, dated, first-person actual switching between two named paid competitors, both with fully visible recurring pricing.

---

### Candidate 7 — Amazon FBA Reimbursement Auditing

#### Problem domain
Detecting and filing claims for Amazon-owed discrepancies (lost/damaged warehouse inventory, customer-return shortfalls, overcharged FBA fees) that require ongoing manual comparison of Amazon's inventory/fee reports against a seller's own records — a recurring reconciliation task most small sellers don't have time to do themselves.

#### Buyer
Small-to-mid Amazon FBA sellers who lack the time/expertise to audit Amazon's reports themselves and instead pay a third party on contingency. UNKNOWN exact seller-size threshold.

#### Existing paid solution
GETIDA ([getida.com](https://getida.com)) — contingency-fee reimbursement-auditing service, an approved Amazon Selling Partner Appstore partner. Named direct competitor: Refunds Manager.

#### Existing spending
**Strong.** Direct evidence of a 25% commission on recovered amounts, plus a reviewer describing an additional "service fee" charged on top — real money changing hands on a contingency basis.

#### Class A evidence
Trustpilot reviews of GETIDA (overall 2.3/5 across the sample): Adam P. (Apr 2026, 1★): unresolved billing-policy dispute. L Clarke (Sep 2025, 1★): a promised $400 credit "quietly removed... with no warning." CmH (Aug 2025, 1★): GETIDA "covertly added a 'service fee'... about 5 times what they managed to reclaim." Nicky Taylor-East (Dec 2025, 1★): 25% commission not reversed even if Amazon reverses the reimbursement. Eric Charpentier (Apr 2025, 1★): "Too expensive (25% fee) for a poor service." James (Dec 2024, 3★): slow, unresponsive support. Comparative note: Refunds Manager shows 4.9/5 across 389 reviews on the same aggregator vs. GETIDA's 2.3/5 — a **comparison** signal only; no first-person "I switched from GETIDA to Refunds Manager" quote was found.

#### Class B evidence
25% contingency commission on recovered funds, confirmed by multiple reviewers describing actual charges. **Strong.**

#### Freshness
≤12 months for most cited reviews (Sep 2025–Apr 2026); two slightly older (Apr 2025, Dec 2024) included for pattern context.

#### Source independence
All from Trustpilot, but each review is a distinct, named/initialed, dated individual account — genuinely independent, not a single syndicated story.

#### Switching signal
**Recurring dissatisfaction**, with a secondary **comparison** signal (star-rating gap vs. a named competitor). Not confirmed as actual switching.

#### Switching destination
UNKNOWN with confidence — Refunds Manager is the most plausible destination based on comparative ratings alone, but this is inferred, not observed.

#### Buyer publicness
Public — Trustpilot reviews exist; direct Reddit (r/FulfillmentByAmazon) text could not be retrieved this session, so broader community sentiment is UNKNOWN.

#### Distribution hypothesis — UNVERIFIED
Amazon Selling Partner Appstore listing (where GETIDA is already an approved partner), FBA seller Facebook groups, SellerCentral/Reddit FBA communities.

#### Unknowns
True churn rate from GETIDA to competitors; whether the underlying pain is the audit/detection problem itself or GETIDA's specific commission structure/customer service.

#### Why investigate further?
Recent, named, dated complaint evidence tied to a well-documented contingency-fee paid incumbent — but the switching-destination story needs direct confirmation before treating it as more than dissatisfaction.

---

### Candidate 8 — eBay/Etsy Cross-Listing & Listing-Template Management (post-InkFrog)

#### Problem domain
Managing product listing templates, HTML/design hosting, and cross-promotion/relisting across eBay and other marketplaces (Etsy, Amazon) from a single tool — the tooling multichannel resellers depend on to keep listings from expiring and to relist/archive efficiently.

#### Buyer
Long-tenured eBay/Etsy power sellers and small multichannel resellers (some described using the same tool for "nearly 20 years") who pay monthly for a listing-management/template subscription. UNKNOWN precise business size.

#### Existing paid solution
InkFrog (Wix-owned) — paid tiers historically $11–$79/month plus a free 10-listing tier. InkFrog announced shutdown April 29, 2026, effective June 1, 2026, forcing a hard migration deadline (per [valueaddedresource.net](https://valueaddedresource.net/inkfrog-shut-down)).

#### Existing spending
**Strong.** Visible recurring monthly pricing tiers actually paid by named users over an extended period (years).

#### Class A evidence
- valueaddedresource.net (independent eBay-seller trade press), Apr–May 2026: reports the shutdown announcement; seller reaction described as "a sucker punch," questioning "how a major platform like Wix could do this with so little notice" (close paraphrase, not a verbatim named quote).
- eBay Community forum thread "Inkfrog alternatives" ([community.ebay.com/t5/Seller-Tools/Inkfrog-alternatives/td-p/33386424](https://community.ebay.com/t5/Seller-Tools/Inkfrog-alternatives/td-p/33386424)): original poster funfactorychannel (thread ~3 years old): "inkfrog has so many issues now I can't even list correctly." Recent replies (~4 months old, i.e. ~May 2026): ethanwalker_9 recommends "sixbit or litcommerce"; andy.johns_4: found LitCommerce via the Shopify App Store, "been pretty smooth for syncing so far" (**actual switching**); lit1213 describes using FolderLister, working "very well" for a large postcard collection (**actual switching**).

Classification: mix of complaint (older post) and actual switching (recent replies), independent of and slightly predating the formal shutdown — dissatisfaction with InkFrog was already driving switching before the shutdown made it forced for everyone else.

#### Class B evidence
InkFrog's own historical pricing tiers ($11–$79/month), corroborated by the "nearly 20 years" of sustained paid use mentioned in shutdown coverage. **Strong.**

#### Freshness
Mixed: the forum thread originated ~3 years ago, but the most relevant switching replies are ~4–5 months old (≤12 months), and the shutdown itself is Apr–Jun 2026 (~3–5 months old).

#### Source independence
Genuinely independent: valueaddedresource.net (independent trade press, not vendor-owned) and the eBay Community forum (first-party user discussion) are two distinct, non-syndicated source types. Several "InkFrog alternatives" blog posts found incidentally are vendor/competitor-authored marketing content and were **not** counted as Class A evidence — treated as lead sources only.

#### Switching signal
**Actual switching** — both pre-shutdown organic dissatisfaction (named users moving to LitCommerce/FolderLister/Sixbit) and the post-announcement forced migration qualify.

#### Switching destination
LitCommerce, Sixbit, and FolderLister (named directly by users in the eBay Community thread).

#### Buyer publicness
Public — active eBay Community forums and independent eBay-seller trade press cover this openly.

#### Distribution hypothesis — UNVERIFIED
eBay's own certified-provider/partner app directory, eBay Community seller forums, and organic search traffic around "InkFrog alternative"/"InkFrog shutdown" queries capturing forced-migration intent.

#### Unknowns
How many affected sellers are small/individual vs. larger multi-store operations; whether this candidate's core need (listing templates/cross-promotion) is closer to merchandising tooling than to inventory/order reconciliation; durability of the panic-driven migration once the initial scramble settles.

#### Why investigate further?
A rare, real-time, independently-documented forced-migration event from an unambiguously paid incumbent (years of confirmed subscription revenue), with both pre-existing organic switching evidence and a hard, dated shutdown deadline.

---

### Candidate 9 — Field-Service Job-Costing & Payroll Reconciliation (HVAC/Plumbing/Electrical)

#### Problem domain
Reconciling technician hours, job costs, and commission data exported from field-service-management (FSM) software against QuickBooks/payroll runs — office staff manually re-verify these numbers to avoid commission disputes and misstated job profitability.

#### Buyer
Small-to-mid HVAC/plumbing/electrical contractors already running an FSM platform (ServiceTitan) who push data into QuickBooks/payroll. Exact size band UNKNOWN.

#### Existing paid solution
ServiceTitan. No public rate card; multiple 2026 pricing aggregators report $245–$500/technician/month plus $5K–$50K setup fees and a 12-month contract.

#### Existing spending
**Strong** — real recurring per-technician contract pricing, corroborated indirectly by a reviewer citing "$1500 a month" as an actual paid amount.

#### Class A evidence
Capterra, ServiceTitan reviews: John S., CFO, Construction (May 18, 2026, 5★): "don't understand how transactions were recorded...don't export properly" (QuickBooks integration) — complaint. Edward K., VP Operations, Construction (Mar 10, 2026, 2★): switched from Housecall Pro; "We traded some headaches for more complex issues"; on time-tracking, "4 months working with your team...proved impossible" — **migration** (into ServiceTitan) + recurring dissatisfaction with payroll/time-tracking specifically. Jacqueline P., Owner, Construction (Nov 23, 2024, 1★): "$1500 a month for a program that is lacking in every way," states she's "looking for a new CRM" — complaint + **replacement intent** (whole-platform, not reconciliation-specific).

#### Class B evidence
ServiceTitan per-tech pricing ($245–500/mo), consistent across several 2026 secondary sources (**Strong**, with the caveat that the exact figure is aggregator- rather than vendor-published).

#### Freshness
Mixed: two reviews ≤12 months (Mar/May 2026), one ~22 months old (Nov 2024, explicitly flagged).

#### Source independence
Genuinely independent — three separate named-role Capterra reviewers, different companies/dates.

#### Switching signal
**Recurring dissatisfaction** (accounting/payroll-integration specifically); one reviewer states explicit **replacement intent** at the whole-platform level, not proven for the reconciliation sub-problem alone.

#### Switching destination
Partially known only at whole-platform level (Housecall Pro ↔ ServiceTitan crossover observed); no destination evidence specific to the reconciliation pain. UNKNOWN.

#### Buyer publicness
Public (Capterra, named roles).

#### Distribution hypothesis — UNVERIFIED
r/HVAC, r/electricians, r/Plumbing, trade associations (e.g. ACCA), ServiceTitan's own app marketplace.

#### Unknowns
Whether the pain is separable from a whole-platform-switch decision; how much is ServiceTitan-specific vs. generic to any FSM+QuickBooks pairing; frequency/severity of actual commission disputes.

#### Why investigate further?
Multiple independent, mostly-recent, named-role reviews of the dominant paid FSM platform specifically flag accounting/payroll-integration breakdowns as a recurring failure mode.

---

### Candidate 10 — Construction Subcontractor Pay-Application & Lien-Waiver Compliance

#### Problem domain
Collecting, tracking, and reconciling monthly pay applications (AIA-style billing), change orders, and compliance documents (lien waivers, COIs) between general contractors and subcontractors before payment release.

#### Buyer
General contractors and subcontractors on commercial projects already using a paid GC-side or sub-side billing/compliance platform. Precise revenue band UNKNOWN.

#### Existing paid solution
GCPay (owned by Autodesk, GC-side; 4.7/5 across 484 Capterra reviews as of Aug 2026); Siteline (subcontractor-side billing); Built Technologies (construction finance/lien waivers).

#### Existing spending
**Strong** — a GCPay reviewer directly confirms being charged fees to collect payment ("I resent being billed to collect our money"), i.e. real money changes hands recurrently. Siteline and GCPay both use custom/quote-based pricing (verified directly on siteline.com/pricing; a secondary source's "$1,000/mo" claim was checked and not corroborated on the vendor's own page, so it is **not** used).

#### Class A evidence
Capterra, GCPay reviews, all dated March 2026: Carolinn T., Controller (3★): "I resent being billed to collect our money"; "Having to click repetitively in your check off list is excruciating" — recurring dissatisfaction with the paid incumbent itself. David C., Project Manager (4★): switched from Procore; payment turnaround concerns ("3 steps," funds held) — migration (toward GCPay) + complaint. Mark J., Project Development Manager (5★ overall): "Pausing workflow... to execute physical documents in 2026 is a little behind the times" (manual notary, no e-signature) — complaint. Staci B., Director of Finance (4★): must void invoices when change orders aren't approved; lien-waiver-upload timing creates extra work for subs — complaint.

#### Class B evidence
GCPay: real recurring billing confirmed via reviewer testimony (**Strong**, though rate card not publicly listed). Siteline: confirmed paid, quote-based, price point itself UNKNOWN after direct verification (corrected from an unverified secondary-source figure).

#### Freshness
**≤12 months** — all four GCPay reviews dated March 2026.

#### Source independence
Four distinct named-role Capterra reviewers, different companies/dates — independent, though all drawn from the same platform.

#### Switching signal
**Recurring dissatisfaction** is the strongest consistently-observed signal on the current paid incumbent. One migration data point exists (Procore → GCPay) but that is movement toward, not away from, this incumbent.

#### Switching destination
UNKNOWN — no evidence found of where dissatisfied GCPay/Siteline users go next.

#### Buyer publicness
Public (Capterra, named roles).

#### Distribution hypothesis — UNVERIFIED
Associated General Contractors (AGC) chapters, Procore App Marketplace, LinkedIn construction-finance communities.

#### Unknowns
Whether "fee resentment" reflects structural dislike of any GC-mandated portal model (not GCPay-specific); scale of the paper/notary-process friction across the buyer base.

#### Why investigate further?
Recent (March 2026), independently-authored, named-role reviews of a dominant paid incumbent show a consistent complaint pattern (fee resentment, manual/paper steps, change-order/lien-waiver timing friction) — the freshest evidence cluster found for any single incumbent in this pass.

---

### Candidate 11 — Restaurant Back-Office Vendor Invoice / AP Reconciliation

#### Problem domain
Capturing, coding, and reconciling food & beverage vendor invoices against orders/deliveries, tracking vendor credits, and getting accurate item-level costs into accounting — a recurring, error-prone AP workflow for independent/small multi-unit restaurants.

#### Buyer
Independent restaurants and small multi-unit groups with a bookkeeper/controller/GM handling AP. Unit-count threshold UNKNOWN.

#### Existing paid solution
MarginEdge — restaurant invoice-processing/AP and recipe-costing platform, $350/location/month (rising to $500 bundled with Freepour) plus a $250 one-time setup fee. xtraCHEF and Optimum Control are named paid competitors.

#### Existing spending
**Strong** — visible, specific recurring per-location subscription price.

#### Class A evidence
Capterra, MarginEdge reviews: Tyler S., Partner/Executive Chef (2+ yr tenure, exact date UNKNOWN, 5★): switched from xtraCHEF, "better functionality" — **actual switching**. Greg C., Owner (2+ yr tenure, 5★): switched from Optimum Control, needed better "record retention and Ownership reporting" — **actual switching**. Dana B., Finance/HR Manager (1–2 yr tenure, 2★): "trouble with the amount of time it takes for payments to reach Vendors... tracking credits is not easy... major problem with some electronic payments" — recurring dissatisfaction. Lupe H., Bookkeeper (1–2 yr tenure, 4★): "invoices are put in with a credit without actually receiving the vendor credit" — complaint. Dinh P., Business Analyst (Oct 22, 2020, 5★): evaluated xtraChef, Foodager, Marketman before choosing MarginEdge — comparison, but **older than 12 months**.

#### Class B evidence
MarginEdge published pricing (**Strong**). Aggregate Capterra rating 4.1/5 (71 reviews), customer-service sub-score 3.8 with "slow follow-up and unresolved tickets" cited — confirms an active paying base with support friction (contextual, not standalone spending evidence).

#### Freshness
Mixed/partially UNKNOWN — reviewer tenure bands ("1–2 years," "2+ years") were captured rather than exact publish dates for the switching/credit-tracking reviews; one comparison review is confirmed Oct 2020.

#### Source independence
Five distinct named/titled Capterra reviewers, different companies — genuinely independent.

#### Switching signal
**Actual switching** is directly observed, but toward this incumbent (from xtraCHEF/Optimum Control), not away from it. The signal most relevant to a new entrant is the **recurring dissatisfaction** (payment delays, credit-tracking errors) on the current incumbent.

#### Switching destination
For xtraCHEF/Optimum Control leavers: MarginEdge (confirmed). For MarginEdge-dissatisfied users: UNKNOWN.

#### Buyer publicness
Public (Capterra, named roles).

#### Distribution hypothesis — UNVERIFIED
Restaurant-industry Facebook groups, r/restaurantowners, National Restaurant Association / state associations, POS marketplaces (Toast, Square).

#### Unknowns
Exact publish dates of the key reviews (freshness not fully confirmed); how much of the "vendor credit tracking" pain is MarginEdge-specific vs. an industry-wide issue (vendors being slow to issue credits regardless of software).

#### Why investigate further?
A paid incumbent with clearly visible, meaningful pricing has multiple independent, named-role reviewers describing the same specific reconciliation failure mode rather than generic dissatisfaction.

---

### Candidate 12 — Property Management Maintenance-Coordination Labor Gap

#### Problem domain
Dispatching, tracking, and following up on maintenance work orders between tenants, property managers, and vendors/contractors — a high-touch coordination workflow that property-management software records but does not automate end-to-end.

#### Buyer
Small-to-mid residential property management companies (roughly 50–1,000+ units, since AppFolio itself enforces a 50-unit minimum) that already pay for PM software and separately staff or hire out maintenance coordination. UNKNOWN precise band.

#### Existing paid solution
AppFolio Property Manager (Core ≈$1.40–1.49/unit/month, ~$280–298/mo minimum; higher tiers to $5+/unit; 50-unit portfolio minimum, quote-based pricing per several 2026 secondary sources) or Buildium (4.5/5 across 2,200+ Capterra reviews) as the software layer; separately, paid VA/staffing labor sourced via VPM Solutions (a dedicated property-management VA marketplace) or Upwork.

#### Existing spending
**Strong** for the software layer (real recurring per-unit paid subscriptions). **Medium-to-Strong** for the labor layer: a live, functioning marketplace (VPM Solutions) exists specifically for hiring PM VAs including maintenance coordination, and Upwork/Indeed show real budgeted job postings ($17.79–$24.28/hr reported median). Not personally-observed invoice-level proof, so flagged as a caveat rather than upgraded to full Strong.

#### Class A evidence
- Vendoroo.ai (a vendor in this exact space), comparison article, Nov 2025: "Maintenance coordination is the highest-volume pain point in property management — and neither Buildium nor AppFolio fully automates it." **Vendor marketing claim, not independent evidence** — treated as a lead only, per the "alternative to X pages are lead sources only" rule.
- Capterra, AppFolio reviews: Doug H., Owner/Manager (Oct 10, 2019, 5★): move-in/out transition friction, manual date-manipulation workaround — complaint, but **stale** (~7 years old). Benjamin B., Executive Manager (Nov 5, 2020, 5★): slow inspection photo uploads — complaint, stale.
- No independent (non-vendor), recent Class A evidence tying "maintenance coordination" specifically to switching/replacement intent was found — a genuine gap, reported honestly rather than papered over.

#### Class B evidence
VPM Solutions — a live marketplace exclusively for PM virtual staff (**Medium-Strong** — real recurring paid engagements occur, but no individual transaction record was pulled). Upwork PM-VA postings with visible hourly budgets (**Medium**). Indeed postings for in-house "Maintenance Coordinator" roles (**Medium-Strong** — "hiring for the workflow" is explicitly named as acceptable Class B evidence in `BASELINE.md`).

#### Freshness
Mixed: VPM Solutions/Upwork/Indeed evidence is current (live 2026 listings); Capterra maintenance-specific review evidence is stale (2019–2020); the "highest-volume pain point" claim is dated Nov 2025 (≤12 months) but non-independent (vendor-sourced).

#### Source independence
Weak on Class A — the strongest-sounding claim comes from a single commercially-interested vendor, one non-independent data point, not corroborated.

#### Switching signal
**Complaint** (weak, stale) is the strongest thing independently supportable from Class A. Not upgraded despite the vendor's stronger-sounding claim.

#### Switching destination
UNKNOWN.

#### Buyer publicness
Partially public — PM software reviews are public, but how companies actually staff around the coordination gap is mostly visible only through job postings/staffing marketplaces rather than public complaint threads; direct Reddit access (r/PropertyManagement, r/Landlord) was blocked this session, likely underselling public discussion that exists there.

#### Distribution hypothesis — UNVERIFIED
NARPM (National Association of Residential Property Managers) chapters/forums, r/PropertyManagement, property-management staffing marketplaces (e.g. VPM Solutions itself as a channel).

#### Unknowns
Whether this is a solvable product problem or fundamentally a labor/communication problem software alone can't fix; true scale of VA/staff spend allocated specifically to maintenance coordination vs. bundled PM-VA duties (not separable from current evidence).

#### Why investigate further?
A dedicated, live paid staffing marketplace exists specifically for this exact labor gap — a real behavioral signal of recurring paid demand — even though independent Class A dissatisfaction evidence for this specific sub-problem was thin and partly stale. This is the clearest test case in the batch for `BASELINE.md` §12's rule that a quiet domain with real spending evidence remains eligible.

---

## Cross-Domain Observations

*Methodological observations only — no candidate is ranked or declared a winner.*

- **Reconciliation-type workflows dominate the surfaced set** (8 of 12 candidates center on matching one system's records against another: commission statements, marketplace settlements, IOLTA trust accounts, job costs, pay applications, vendor invoices, FBA reimbursements, client-document workflow). This may reflect a genuine cross-industry pattern in back-office pain, but it may equally be an artifact of what's easiest to find on review platforms — reconciliation problems have a clean before/after story ("I used to spend X hours, now I don't") that reviewers write up, while other problem types may not surface as readily through Class A sourcing. This should not be read as evidence that reconciliation problems are inherently more attractive; it may simply be more visible.
- **Switching-destination patterns vary in a way the Switching Feasibility rule anticipated.** Candidate 4 (real estate) shows switching almost entirely toward one entrenched incumbent (dotloop) — flagged explicitly as a distribution/entry risk, not an opportunity, per `BASELINE.md` §8. Candidate 5 (recruiting) shows healthier two-way flow between several mid-market vendors. Several others (Candidates 6, 9, 11) show switching mostly *toward* the incumbent used as the evidence source, meaning the most relevant signal for those candidates is the dissatisfaction *among current users*, not a confirmed exit path.
- **Two independent research passes converged on the same domain (Candidate 1) without coordination.** This is treated as a mild corroborating signal that the domain is genuinely discoverable through this method, not as proof of opportunity — both passes drew primarily from the same underlying platform (Capterra), so the convergence is partly a reflection of that platform's coverage, not fully independent triangulation.
- **Buyer publicness correlates with how the domain was found.** Candidates found primarily through Class B (Candidate 12, partially Candidate 4's contractor leg) have thinner Class A trails, exactly the pattern `BASELINE.md` §10 predicted the two-source-class approach would catch. Candidate 12 in particular would likely have been dropped entirely under a complaints-only methodology.

---

## Evidence Gaps

- Direct Reddit access was blocked for at least two of the four research passes (confirmed for the trades/local-operations pass: r/HVAC, r/PropertyManagement, r/Construction, r/restaurantowners; likely affected FBA/insurance searches in other passes as well). This probably underrepresents true Buyer Publicness for several candidates (9, 10, 11, 12, 7) where community discussion plausibly exists but could not be directly retrieved this session.
- Exact review publication dates could not be captured for several important data points (Candidate 5's Recruit CRM reviews, Candidate 11's MarginEdge switching reviews, Candidate 9's ServiceTitan pricing) — recorded as UNKNOWN rather than assumed fresh.
- G2 fetches returned HTTP 403 in at least one pass; Upwork job-posting bodies returned HTTP 403 in another (Candidate 3) — access limitations, not findings about the underlying market.
- Several plausible Class B data points (e.g. specific dollar-figure contract minimums for recruiting CRMs, an FBA-reimbursement industry-hours estimate) were deliberately excluded because they traced back to vendor/affiliate comparison content rather than a verifiable primary source — the gap is intentional, not an oversight.
- No candidate's Payment Plausibility, Switching Feasibility (beyond the incidental destination-tracking above), or Distribution was verified — by design, per the task scope.

---

## Methodological Limitations

- **Single-platform concentration.** The overwhelming majority of Class A evidence across all 12 candidates comes from one platform, Capterra (with Trustpilot for Candidate 7, and eBay Community/trade press for Candidate 8 as the main exceptions). Individual reviewers are independent people, but the source *type* diversity is low. `BASELINE.md` §14 items 17/24/25 (vocal-minority bias, platform effects on visibility, false independence from cross-posting) apply with extra force here: review-platform visibility is itself shaped by which buyers bother to leave reviews and by each platform's own moderation/ranking.
- **Survivorship bias toward the "winning" vendor.** For Candidates 2, 4, 6, 8, and 11, the primary evidence source is the *destination* vendor's own review page — meaning the sample is inherently people who completed a switch and (mostly) stayed satisfied enough to review, not a neutral cross-section of everyone who left the incumbent. Failed or abandoned switching attempts are systematically invisible in this evidence base, per `BASELINE.md` §14 item 21.
- **Reviewer-name/date reliability caveat.** Two of the four sub-agents explicitly flagged that some reviewer names/dates were extracted via automated page-fetch-and-summarize rather than manually verified character-by-character (Candidates 1 and 5 in particular). This is recorded per-candidate above rather than silently smoothed over.
- **Anti-bias compliance check:** none of the forbidden shortcuts (SaaS idea lists, "best micro-SaaS ideas" sites, competitor-count lists, "low competition" searches, market-size rankings, app-store star-rating rankings, marketplace app counts, feature-request counts as switching) were used as core evidence for any candidate. Each research pass's own "domains dropped" notes confirm several candidates were excluded specifically *because* the only available evidence was exactly one of these forbidden types (e.g. Candidate-adjacent healthcare-credentialing and bookkeeper-practice-management domains were dropped for lacking independent Class A beyond affiliate/comparison content).
- **Source diversity across sectors was achieved by design** (four parallel passes assigned to different sectors), not by discovering diversity organically — this is a deliberate methodological choice to counter `BASELINE.md` §14 item 27 (domain-selection bias toward loud domains), not a claim that these 12 domains are representative of all possible problem domains.

---

## Recommended Next Research

*No candidate is ranked, scored, or declared a winner. Grouped by recommended status; order within each group reflects discovery order only.*

**Note on "TEST" in this document:** per `BASELINE.md`'s canonical chain, none of these candidates has yet passed the Payment Plausibility Gate (§6), so "TEST" here means *"proceed next to the Payment Plausibility Gate"* — it is not an authorization to run a live paid-validation experiment. Actual Validation remains several gates away for every candidate.

### TEST — proceed to Payment Plausibility Gate next

1. **Candidate 2 — Tax practice client workflow portal.** ≥7 independent, named, dated actual-switching reviews within ~13 months — the freshest and most numerous evidence in the whole pass.
2. **Candidate 1 — Insurance commission reconciliation.** Corroborated independently by two separate research passes; multiple paid competitors; actual switching both from manual process and between paid tools.
3. **Candidate 6 — Multichannel e-commerce accounting reconciliation.** Named, dated, first-person actual-switching accounts between two fully-priced paid competitors.
4. **Candidate 10 — Construction subcontractor pay-application & lien-waiver compliance.** Four independent, named-role reviews, all within the last ~6 months, describing the same specific reconciliation/compliance friction on a confirmed-paid incumbent.
5. **Candidate 8 — eBay/Etsy listing-template management.** A rare, independently-documented, real-time forced-migration event with pre-existing organic switching evidence layered on top.

### INCONCLUSIVE — real evidence exists, but a specific gap must close before further investment

6. **Candidate 4 — Real-estate transaction coordination.** Dual strong Class B evidence, but the observed switching destination is incumbent-to-incumbent, which `BASELINE.md`'s Switching Feasibility rule requires recording as a distribution/entry risk rather than an opportunity.
7. **Candidate 5 — Recruiting ATS-CRM switching.** The most explicit, reason-stated switching quotes found, but the domain as scoped is closer to a whole software category than one narrow problem, and some complaint volume may reflect an enterprise/SMB mismatch.
8. **Candidate 7 — Amazon FBA reimbursement auditing.** Strong, recent, named complaint evidence on a confirmed-paid incumbent, but no first-person "I switched to X" quote was found, only a comparative rating gap.
9. **Candidate 9 — Field-service job-costing & payroll reconciliation.** Independent, mostly-recent reviews flag the exact reconciliation failure mode, but switching-destination evidence is specific to a whole-platform decision, not the reconciliation sub-problem, and one key data point is stale.
10. **Candidate 11 — Restaurant back-office vendor invoice/AP reconciliation.** Independent, named-role reviews describe the same specific failure modes, but exact review dates could not be fully confirmed and the clearest switching evidence flows toward, not away from, the incumbent used as the evidence source.

### BLOCKED — a specific missing input, not a killed hypothesis

11. **Candidate 3 — Law firm trust accounting / IOLTA reconciliation.** The clearest actual-switching evidence found is dated 2020; the only evidence within the last 12 months is general (non-trust-specific) dissatisfaction — fresh, sub-problem-specific Class A evidence is needed before this can be treated as current.
12. **Candidate 12 — Property management maintenance-coordination labor gap.** A live, dedicated paid staffing marketplace confirms real recurring spend on this exact labor gap, but independent (non-vendor) Class A evidence is thin and stale; direct access to property-management communities (blocked this pass) is needed next — precisely the case `BASELINE.md` §10/§12 warns against dropping for lack of complaint volume alone.

No candidate is marked `KILL`: the Discovery Pass deliberately did not run the Payment Plausibility, Switching Feasibility, or Distribution gates to completion for any candidate, so no candidate has yet been tested against a condition capable of producing a `KILL` verdict under `BASELINE.md`'s own rules. No candidate is marked `KEEP`, per the task's explicit instruction not to award `KEEP` on discovery-stage promise alone.
