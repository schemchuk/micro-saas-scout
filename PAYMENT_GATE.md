# Payment Plausibility Gate

## Scope

- **Date:** 2026-09-22
- **Method:** `BASELINE.md` §6 (Payment Plausibility Gate), operationalized per the three-check structure defined in this task (Task 05). Desk research only — official vendor pricing/signup/terms pages as primary sources for Checks 1–2; independent named-customer reviews (Capterra, G2, Shopify App Store, Trustpilot, eBay Community) traced to primary reviewer text for Check 3. No users contacted, no product built, no preorder requested, no landing page created.
- **Candidates tested:** Insurance Commission Reconciliation; Tax Practice Client Document/Engagement Workflow Portal; Multichannel E-Commerce Accounting Reconciliation; Construction Subcontractor Pay-Application & Lien-Waiver Compliance; eBay/Etsy Cross-Listing & Listing-Template Management. (The 5 candidates specified in this task's scope, out of the 12 in `DISCOVERY.md`.)
- **Gates tested:** Payment Plausibility Gate only (`BASELINE.md` §6), all three sub-checks, for all five candidates.
- **Gates explicitly NOT tested:** Free-Incumbent Trap (§7) — not re-tested here since all five candidates already show a paid, non-free incumbent in `DISCOVERY.md`; Switching Feasibility & Switching Destination (§8); Distribution Evidence (§9); any TAM/SAM/SOM, competitor-count, or keyword-volume analysis; ranking or scoring of any kind.

---

## Candidate 1 — Insurance Commission Reconciliation

### Buyer
Independent US P&C/multi-line insurance agencies and individual agents — finance/operations staff (bookkeepers, controllers, agency principals/administrators) responsible for monthly carrier-statement reconciliation.

### Existing paid solution
Commission Tracker (commission-tracker.com), Commission Wizard (commissionswizard.com), AgencyBloc AMS+ (agencybloc.com), Applied Recon (add-on inside Applied Epic/Applied Systems, not independently re-checked this pass).

### Check 1 — Visible self-serve pricing
- **Evidence:** Commission Tracker's own pricing page (accessed 2026-09-22) publishes flat monthly tiers — Independent Agent $67/mo + $120 signup fee, Small Agency $72+/mo, Medium $119+/mo, Large $166+/mo — each with a working "Add to cart" self-serve checkout button; URL slug itself reads "month-to-month-no-contract." Capterra's independently reported price ($67/mo flat, secondary) matches. Commission Wizard's own pricing page publishes Starter $23/mo, Professional $39/mo (both "Start Free Trial," no card required), Enterprise $79/mo (contact-sales only); explicit text: "No setup fees, implementation fees, or long-term contracts." By contrast, AgencyBloc AMS+ publishes zero dollar figures anywhere — only "Request Customized Pricing Info" / "Schedule a 1:1 Demo," a pure contact-sales pattern.
- **Sources:** commission-tracker.com/pricing/ (primary, 2026-09-22); capterra.com/p/88991/Commission-Tracker-for-Insurance/pricing/ (secondary, 2026-09-22); commissionswizard.com/pricing (primary, 2026-09-22); agencybloc.com/pricing/ (primary, 2026-09-22).
- **Decision: PASS** — two named, relevant paid solutions (Commission Tracker, Commission Wizard) show real self-serve checkout/trial-signup mechanisms, distinct from the contact-sales-only pattern seen at AgencyBloc.

### Check 2 — Independent purchase
- **Evidence:** Commission Tracker's Independent Agent tier is explicitly sized for a single agent, checks out via "Add to cart" with no visible approval gate (a flat $120 signup fee applies to all software tiers). Commission Wizard's Starter tier (3 users) starts via a 14-day trial requiring only an email address, "No credit card required," and the vendor states directly on its pricing page: "No setup fees, implementation fees, or long-term contracts." Neither product's pricing page shows a minimum agency size or mandatory sales approval step. AgencyBloc requires a demo/sales conversation to purchase at all.
- **Sources:** commission-tracker.com/pricing/ (primary); commissionswizard.com/pricing and /register (primary). Terms-of-service fine print was not independently fetched for either product — flagged as a remaining unknown, not treated as a failure since the vendors' own pricing-page claims are unambiguous and uncontradicted.
- **Decision: PASS**

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Commission Tracker (a small specialist vendor, not a dominant/enterprise player) has 17+ named, dated Capterra reviewers self-identifying with real agency job titles, several describing multi-year continuous use — e.g., Gayle G., Agency Owner: "We have been using Commission Tracker for years" (5.0★, Sept 8 2026); Michael C., VP/Insurance Agency: "used the program over 15 years" (5.0★, Sept 10 2026); Jennifer K., Commissions Specialist (4.0★, Sept 17 2026). Reviews span 2018–Sept 2026 with several from the current month, confirming currently active paying users. Commission Wizard, by contrast, has no discoverable review-site profile on Capterra or G2 and no named customer testimonials on its own site — its purchase precedent is genuinely unconfirmed, not disproven.
- **Sources:** capterra.com/p/88991/Commission-Tracker-for-Insurance/reviews/ (primary named reviews, 2026-09-22); g2.com/products/commission-tracker/reviews (secondary corroboration, 2026-09-22).
- **Decision: PASS** — Commission Tracker alone provides sufficient, current, named-customer precedent that this buyer type purchases from a small/specialist vendor.

### Gate result
**PASS** (all three checks pass) — candidate may proceed to the next gate.

### Reason
A relevant paid solution (Commission Tracker) shows genuine self-serve pricing and checkout, no structural purchasing barrier for an independent agent, and current, named, multi-year customer precedent confirming this buyer type actually pays a small specialist vendor.

### Remaining unknowns
Commission Tracker's and Commission Wizard's full Terms of Service (cancellation terms, fine print beyond the pricing page) were not independently fetched. Commission Wizard's actual customer base remains unconfirmed either way (no review-site trail found — could mean it's too new/small to have left one, not that it lacks customers).

---

## Candidate 2 — Tax Practice Client Document/Engagement Workflow Portal

### Buyer
Small US tax preparation/accounting firms (solo practitioners up to small teams) — owners, partners, bookkeepers, staff accountants selecting practice-management/client-portal software.

### Existing paid solution
TaxDome (taxdome.com), Canopy (getcanopy.com), SmartVault (smartvault.com); Financial Cents (financialcents.com) as a smaller specialist alternative.

### Check 1 — Visible self-serve pricing
- **Evidence:** All three major incumbents publish exact, non-negotiated prices — TaxDome: Essentials $800/yr, Pro $1,000/yr, Business $1,200/yr (1-yr commitment; page confirms "we do not negotiate on pricing"); Canopy: $74–149/user/mo; SmartVault: $55–85/user/mo (2–3 user minimums). But **every plan-selection CTA on all three pricing pages is a demo/sales-contact button**, not a buy button: TaxDome's own Help Center documents the actual process verbatim — "Click Contact sales. Complete the form to book a one-on-one demo with our team... When you're ready to move forward, you can configure the platform yourself." Canopy's CTA is "GET A DEMO" with FAQ text "Schedule a demo and talk with a sales representative to set up a trial." SmartVault's CTAs are "Book A Demo" / "Request A Trial." None of the three shows a working self-serve checkout button on the pricing page itself. A third-party mention of an instant-signup flow at app.taxdome.com/signup was found but not independently verified and conflicts with TaxDome's own documented process — treated as unconfirmed, not used as positive evidence.
- **Sources:** taxdome.com/pricing (primary, page `modified_time` 2026-08-14); help.taxdome.com/article/187-taxdome-pricing-faq and /article/72-firm-registration (primary, vendor help center); getcanopy.com/pricing (primary); smartvault.com/pricing (primary) — all accessed 2026-09-22.
- **Decision: FAIL** — this is the exact "contact sales despite a published, non-negotiable price" pattern the task instructs not to treat as self-serve. All three primary incumbents checked require a vendor-initiated demo/sales conversation before a purchase can occur, even for a single-seat solo buyer.

### Check 2 — Independent purchase
- **Evidence:** TaxDome's Essentials tier is explicitly capped at 1 seat ("solo users only"), with no stated minimum beyond that, and no mandatory paid onboarding fee (onboarding described as free). A solo owner has full authority to decide and pay for TaxDome without needing organizational approval, a procurement committee, or a security certification — the only friction is the demo-booking step already captured under Check 1. SmartVault requires a 2–3 user minimum on some tiers, a mild structural constraint for a true solo practitioner but not a procurement barrier per se.
- **Sources:** help.taxdome.com/article/187-taxdome-pricing-faq (primary); smartvault.com/pricing (primary) — accessed 2026-09-22.
- **Decision: PASS** — no minimum firm size, committee approval, or certification requirement was found; the purchase decision itself rests with the individual buyer, distinct from the self-serve-mechanism question already resolved as FAIL under Check 1.

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Financial Cents (a smaller, specialist vendor relative to TaxDome/Canopy) has multiple named, dated 2025 Capterra reviews describing genuine hands-on paid use: Megan C., Principal Owner, Oct 31 2025, 5.0★: "Have used tax dome in the past but felt Financial Cents better fit our needs and was more flexible with better features and price" — an explicit, named switch away from the category's dominant incumbent; Angeliese W., Owner/Founder, Sept 19 2025, describing specific operational usage (document management, client communication, recurring templates); David B., Partner, Sept 19 2025, "Used the software for: 1-2 years," describing specific product friction consistent with real multi-year paid use.
- **Sources:** capterra.com/p/186837/Financial-Cents/reviews/ (primary named reviewer testimony hosted on secondary platform, page footer "Last updated August 26th, 2026") — accessed 2026-09-22.
- **Decision: PASS**

### Gate result
**KILL**

### Reason
Check 1 fails: the category's dominant, named incumbents (TaxDome, Canopy, SmartVault) all publish transparent, fixed pricing but gate the actual purchase behind a mandatory vendor-initiated sales/demo conversation, confirmed directly from TaxDome's own help documentation. Per gate logic, a Check 1 failure is a KILL regardless of the other checks' results — this is a textbook instance of the "real existing spending, but no credible self-serve payment mechanism" pattern the gate exists to catch.

### Remaining unknowns
Financial Cents' own pricing/signup mechanism was not independently checked this pass — it is possible a genuinely self-serve paid option exists in this category via Financial Cents or another smaller player, which would need direct verification (its own pricing page and signup flow) before this KILL could be revisited with materially new evidence, per `DECISION.md`'s reopening rule.

---

## Candidate 3 — Multichannel E-Commerce Accounting Reconciliation

### Buyer
Small-to-mid multichannel e-commerce sellers (roughly 100–20,000+ orders/month, selling across 2+ of Amazon/Shopify/eBay/Etsy/Walmart) and the bookkeepers/accountants who manage their books on Xero/QuickBooks Online.

### Existing paid solution
A2X (a2xaccounting.com), Link My Books (linkmybooks.com), Taxomate (taxomate.com), Dext Commerce.

### Check 1 — Visible self-serve pricing
- **Evidence:** A2X's own pricing pages publish exact tiers from $29/mo (single-channel) through named multi-channel tiers up to $1,869/mo (250,000 orders), with "Try A2X for Free" / "Get started" buttons on every tier up to 50,000 orders; "Talk to sales" appears only above that, for custom/enterprise volume. Link My Books' own pricing page publishes a usage-based calculator ($21–$176+/mo per independent secondary corroboration, eightx.co, June 2026) with a "Start a 14-Day Free Trial" button and explicit "No card required" — corroborated by a help-center article (help.linkmybooks.com, dated April 27 2026) documenting a live mid-2026 price change applied automatically to existing subscribers, confirming an active self-serve billing system.
- **Sources:** a2xaccounting.com/pricing, /multi-channel/pricing, /shopify/pricing (primary, 2026-09-22); linkmybooks.com/pricing (primary, 2026-09-22); help.linkmybooks.com/en/articles/11093698-2026-price-changes (primary, dated 2026-04-27); eightx.co/blog (secondary, dated 2026-06-18).
- **Decision: PASS**

### Check 2 — Independent purchase
- **Evidence:** Neither vendor's pricing page shows a mandatory setup call, minimum contract term, or minimum order-volume commitment for standard (small-to-mid) tiers. Link My Books' trial requires no card and its help center documents a simple self-cancel policy. Sales contact is offered as an option, not required, for either vendor below very high volume. (The exact checkout/payment page for both is behind the trial signup and was not directly observed — flagged as a minor unknown, not treated as a failure given the unambiguous "no card required" / direct trial-start language on both pricing pages.)
- **Sources:** a2xaccounting.com/pricing (primary); linkmybooks.com/pricing (primary) — accessed 2026-09-22.
- **Decision: PASS**

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Link My Books (smaller/specialist relative to dominant incumbent A2X) has strong, current, named-customer evidence: Capterra reviewers Aaron J. (Director, Aug 21 2026, switched from A2X), Erin S. (Apr 10 2026), Victoria K. (May 12 2026); and, independently, Shopify App Store verified-install reviews showing multi-year paid tenure — Eventcarpetsonline Ltd, "about 3 years using the app," explicitly noting recurring price increases (implying ongoing paid renewal), Newhill Deals ("over 1 year"), Minati ("about 1 year"). Taxomate has one solid named 2025 switcher (Mo K., May 16 2025, switched from Link My Books). Dext Commerce shows no reviews dated 2025–2026 in this search pass (most recent found: Aug 2023) — flagged as a genuine gap for that specific vendor, not evidence against the category.
- **Sources:** capterra.com/p/184768/Link-My-Books/reviews/ (primary, 2026-09-22); apps.shopify.com/linkmybooks/reviews (primary, verified installs, 2026-09-22); capterra.com/p/187763/taxomate/reviews/ (primary, 2026-09-22).
- **Decision: PASS**

### Gate result
**PASS** (all three checks pass) — candidate may proceed to the next gate.

### Reason
Multiple relevant paid solutions show genuine self-serve trial-to-payment mechanisms with no procurement barrier for the identified small-to-mid seller buyer, and a smaller specialist vendor (Link My Books) has strong, current, multi-source named-customer evidence of real recurring paid use, including explicit switches away from the dominant incumbent.

### Remaining unknowns
The literal checkout/payment-collection page for both A2X and Link My Books was not directly observed (paywalled behind trial signup). Dext Commerce specifically has no confirmed 2025–2026 customer evidence, though this doesn't affect the category-level Check 3 result since Link My Books alone provides sufficient precedent.

---

## Candidate 4 — Construction Subcontractor Pay-Application & Lien-Waiver Compliance

### Buyer
General contractors (GCs) and subcontractors on commercial construction projects, per `DISCOVERY.md`'s dual-sided buyer definition.

### Existing paid solution
GCPay (Autodesk-owned, GC-side), Siteline (subcontractor-side billing), Built Technologies (getbuilt.com — construction finance/lien waivers).

### Check 1 — Visible self-serve pricing
- **Evidence:** GCPay's own pricing page shows no price at all — exact text: "Custom pricing tailored to your business needs," "Only pay for the volume of projects that you're managing with subcontractors," CTA "Book Demo"/"Get Started." Capterra corroborates: "Contact vendor for pricing," no free trial. Siteline's own pricing page likewise shows no price — "We work with our customers to offer pricing that best suits their product usage, billing volume, and integration needs," gated behind a multi-step "Get a custom quote" form. Built Technologies is a partial exception: it publishes one concrete figure ("Lien Waiver Management $1,000/month" for a standalone tier, discounts "when processing payments"), but no self-serve checkout/buy button was found for this tier — the mechanism to actually purchase it was not confirmed as self-serve.
- **Sources:** ww3.gcpay.com/pricing-for-general-contractors/ (primary, 2026-09-22); capterra.com/p/182990/GCPAY/pricing/ (secondary, "last updated August 26, 2026"); siteline.com/pricing (primary, 2026-09-22); getbuilt.com/products/lien-waiver-management-payments/ (primary, 2026-09-22).
- **Decision: FAIL** — the two most central, named incumbents for this candidate (GCPay, Siteline) are both pure quote-only/custom-pricing, with zero published price and a mandatory custom-quote request process; the one vendor with a published number (Built) has no confirmed self-serve purchase path for it.

### Check 2 — Independent purchase
- **Evidence:** This candidate carries a specific, confirmed structural risk. GCPay's own help-center documentation describes a per-transaction "$15 fee" on its ePayments & Lien Waiver Exchange, with a GC-side setting to "take on the $15 fee instead of passing it on to the subcontractor" — confirming the **GC is the account-holder/decision-maker**, who can unilaterally choose to pass a fee to subs who did not choose the platform. An independent industry blog (LienDone, May 10 2026) states directly: "Subs have to create an account in your pay-app system before they can sign. That's fine for the 10 subs who do every job with you. It's friction for the 50 specialty subs who you use once" — describing subs as compelled into whatever system the GC selects, not making an independent purchase decision of their own. Built Technologies shows the identical pattern ("General Contractors/project owners pay for the software subscription... Subcontractors... get free vendor accounts with no login required"). Siteline is the documented counter-case: its own FAQ contains the entry "Our GC requires us to use Textura, why would I add Siteline?" — Siteline's own site confirming the GC-mandate pattern is common enough to build a product around, positioning itself as a tool the **subcontractor independently chooses and pays for** specifically to cope with being mandated onto GC-chosen portals.
- **Sources:** help.gcpay.com (primary, vendor support doc, 2026-09-22); liendone.com/blog/what-is-gc-pay (secondary, named industry blog, dated 2026-05-10); getbuilt.com (primary, 2026-09-22); siteline.com/faq (primary, 2026-09-22).
- **Decision: FAIL** — for the GC-side pattern that dominates this candidate's named incumbents (GCPay, Built), the subcontractor half of the identified buyer cannot independently choose or purchase; participation is mandated by the GC, and the GC itself purchases only through the custom-quote sales process already found under Check 1. Siteline's sub-independent pattern is real but is a workaround to the structural barrier, not evidence the barrier doesn't exist for the core GC-mandated workflow this candidate's problem domain describes.

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Both Siteline and Built Technologies have real, named, dated 2025–2026 Capterra reviews from individuals in construction roles, confirming actual paying/using customers exist independent of vendor marketing — Siteline: Jordan C., Owner/President, May 12 2025, 5.0★, "transformed the way my company processed billings"; Veronica C., Accounting Manager, May 6 2025; McKenzie P., Administrative Director, May 6 2025, switched from Sage 100. Built: Ben S., CEO, July 3 2026 (negative); Sarah M., Office Assistant, July 10 2025 (negative but confirms active real use).
- **Sources:** capterra.com/p/252004/Siteline/ (primary, 2026-09-22); capterra.com/p/159434/Built/reviews/ (primary, 2026-09-22).
- **Decision: PASS**

### Gate result
**KILL**

### Reason
Check 1 fails (the category's central incumbents, GCPay and Siteline, are quote-only with no published price) and Check 2 independently fails (confirmed structural GC-mandate barrier: subcontractors — half of the identified buyer — do not independently choose or purchase the compliance platform; the GC does, and only through a sales-gated custom quote). Either failure alone triggers KILL per gate logic; both are independently confirmed here with primary vendor documentation. This is precisely the pattern described in this task's "Important distinction" section: real existing spending and a real paid incumbent, but a payment mechanism that requires procurement/custom contracting before any purchase occurs.

### Remaining unknowns
No first-person subcontractor complaint specifically describing being charged a GC-passed fee was found (the structural mechanism is vendor-documented, but a named sub's own account of experiencing it was not located this pass). Built Technologies' actual self-serve purchase mechanism for its one published price point ($1,000/mo) was not fully traced to a checkout flow.

---

## Candidate 5 — eBay/Etsy Cross-Listing & Listing-Template Management

### Buyer
Long-tenured eBay/Etsy power sellers and small multichannel resellers who pay monthly for a listing-management/template subscription, displaced by InkFrog's April–June 2026 shutdown.

### Existing paid solution
LitCommerce (litcommerce.com), Sixbit (sixbitsoftware.com), FolderLister (folderlister.com) — the three named InkFrog-alternative destinations from `DISCOVERY.md`'s eBay Community forum evidence.

### Check 1 — Visible self-serve pricing
- **Evidence:** LitCommerce's own pricing page publishes an interactive slider ("From $29/mo" for 3 channels/1,000 listings), with a direct "START FREE TRIAL" button linking to a real registration flow, 7-day trial, accepting card/PayPal/Shopify/Wix Payment, no setup costs. Sixbit's own pricing page publishes five exact named tiers ($29.99–$184.99/mo), each with a "TRY FREE" button linking directly to a checkout cart (`clients/cart.php?a=add&bid=...`), 30-day free trial, explicit "no contractual obligations." FolderLister's homepage publishes three tiers including a genuine $0 free tier ("No payment details required") plus Pro $25/mo and Extreme $45/mo, each with a "Subscribe" button linking straight to Stripe checkout, license key delivered by email after payment.
- **Sources:** litcommerce.com/pricing/ (primary, page `og:updated_time` 2026-09-09, accessed 2026-09-22); sixbitsoftware.com/pricing/ (primary, page `modifiedTime` 2024-08-06, accessed 2026-09-22); folderlister.com/ (primary, accessed 2026-09-22).
- **Decision: PASS** — all three named alternatives have genuine, working self-serve checkout with no sales-call gate at any tier.

### Check 2 — Independent purchase
- **Evidence:** All three allow an individual seller to sign up and pay online today with no procurement step. LitCommerce's monthly plan cancels "at any time"; its only contract wrinkle is an optional discounted annual plan that "commit[s] you to a full year of service" — avoidable by staying on monthly billing. Sixbit explicitly states "no contractual obligations," no setup fee. FolderLister's free tier requires no payment info at all, and its paid tiers go straight through Stripe with no stated minimum term or onboarding call.
- **Sources:** litcommerce.com/pricing/ FAQ (primary); sixbitsoftware.com/pricing/ FAQ (primary); folderlister.com/ (primary) — all accessed 2026-09-22.
- **Decision: PASS**

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** The eBay Community forum thread (community.ebay.com, replies dated ~May 2026, during the InkFrog shutdown window) shows named posters describing active use — andy.johns_4: "Try LitCommerce, i found it on the Shopify app store... been pretty smooth for syncing so far"; lit1213: "Personally I use folderlister... Re-use profiles with pre set item specifics." Critically, **neither post confirms paid status**: LitCommerce offers a 7-day trial and FolderLister has a permanent free tier, so both named users could plausibly be on a free/trial tier rather than paying. A FolderLister vendor-published testimonial names a real, checkable eBay storefront (Sven Masch / ebay.com/usr/fotohistorie) but is vendor marketing content, not independent evidence. An independent Trustpilot review (litcommerce.com, dated Sept 20 2026) describes a detailed, dated migration from Codisto Linq/Marketplace Connect and being "fully operational" within a week, but the reviewer is anonymous and the tier (free/paid) is not stated. Sixbit's most recent named Capterra review is from Sept 16 2024 (Rob N.) — no current (2025–2026) named customer evidence was found for Sixbit specifically.
- **Sources:** community.ebay.com/t5/Seller-Tools/Inkfrog-alternatives/td-p/33386424 (secondary forum, named posters, replies ~2026-05); trustpilot.com/review/litcommerce.com (independent, 2026-09-20); capterra.com/p/178178/SixBit-Software/reviews/ (primary, 2026-09-22); g2.com/sellers/folderlister (independent, "Verified Current User," date/tier not stated).
- **Decision: UNKNOWN** — real, dated, named activity around these tools exists, but no evidence gathered this pass unambiguously confirms *paid* (as opposed to free-tier or trial) usage by an identified individual, and Sixbit's own customer trail is stale (>12 months).

### Gate result
**BLOCKED / INCONCLUSIVE**

### Reason
Checks 1 and 2 both pass cleanly — self-serve pricing and independent purchase are well-confirmed for all three named alternatives. Check 3's evidence is real but does not clear the bar for confirmed *paid* precedent (the two most relevant named forum users could plausibly be on free/trial tiers). Per gate logic, "Check 3 = UNKNOWN → BLOCKED/INCONCLUSIVE. Do not manufacture a PASS."

### Remaining unknowns
Whether andy.johns_4 (LitCommerce), lit1213 (FolderLister), or the G2/Trustpilot reviewers are actually on a paid tier, versus free/trial. Whether any current (2025–2026) named Sixbit customer exists at all — the only trail found is from 2024.

---

## Cross-Candidate Observations

*Methodological observations only — no ranking of candidates.*

- **"Contact sales despite a published, non-negotiable price" is a distinct failure mode from pure quote-only pricing**, and both were encountered in this pass (Candidate 2 = published-but-demo-gated; Candidate 4's GCPay/Siteline = no price published at all). Both correctly fail Check 1 under the task's own instruction not to treat "contact us" as self-serve, but future gate applications should keep recording which sub-pattern applies, since the two failure modes carry different implications (a published price at least signals the vendor doesn't negotiate case-by-case, even if the checkout mechanism itself isn't self-serve).
- **Review-tenure claims ("used it for 3 years," "using the app for over 1 year") on Capterra/Shopify App Store are a useful but imperfect proxy for confirmed paid status.** They strongly suggest sustained real usage but do not, on their own, rule out an extended free/trial tier, especially for products (like two of the three checked in Candidate 5) that offer a permanent free tier or an unusually long trial. This gap directly produced the Candidate 5 UNKNOWN result and should be treated as a recurring limitation of Capterra/App-Store review evidence generally, not specific to that candidate.
- **A dual-sided buyer definition (Candidate 4's "GCs and subcontractors") can contain two structurally different Payment Plausibility profiles at once** — one side (GC) that purchases via custom quote, one side (subcontractor) that is often mandated onto the GC's chosen platform but can independently buy a *different*, complementary tool (Siteline) to cope with that mandate. Averaging or picking one side without stating which was evaluated would have obscured this finding; recording both explicitly was necessary to reach a defensible Check 2 verdict.

---

## Methodological Issues

None found. The three-check structure specified in this task is consistent with, and a direct operationalization of, `BASELINE.md` §6's three questions and decision rule; no contradiction between this task's instructions and `BASELINE.md`/`BASELINE_PATCH.md`/`DECISION.md` was encountered while applying the gate.

---

## Next Research

- **Insurance Commission Reconciliation (PASS):** next gate per `BASELINE.md` ordering is Switching Feasibility & Switching Destination (§8) — `DISCOVERY.md` already recorded actual-switching signal (Excel → Commission Tracker; AgencyBloc AMS+ → Commission Tracker) that now needs to be checked against lock-in, procurement/contractual constraints, and realistic-alternative-availability per §8, not simply carried forward as-is.
- **Multichannel E-Commerce Accounting Reconciliation (PASS):** same next step — Switching Feasibility & Switching Destination (§8), using the A2X → Link My Books / Dext Commerce → Link My Books switching evidence already on record in `DISCOVERY.md`.
- **eBay/Etsy Cross-Listing & Listing-Template Management (BLOCKED/INCONCLUSIVE):** per §6's own rule, this does not advance to the next gate yet. The specific open question to resolve first is Check 3 itself — Source Class B evidence (§10) that directly confirms *paid* (not free/trial) status for named current users of LitCommerce, FolderLister, or Sixbit, and any current (2025–2026) named Sixbit customer at all.
- **Tax Practice Client Portal and Construction Subcontractor Pay-Application (KILL):** no further research proposed under this task's scope. Per `DECISION.md`'s global rule, a KILL is not reopened without materially new evidence — for Candidate 2, that would mean direct confirmation of a genuinely self-serve (non-demo-gated) purchase path at a relevant vendor (e.g., Financial Cents, unverified this pass); for Candidate 4, it would mean evidence that the GC-mandate structural pattern found here is not, in fact, dominant for this problem domain.
