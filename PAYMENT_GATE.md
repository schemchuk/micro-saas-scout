# Payment Plausibility Gate

## Scope

- **Date:** 2026-09-22 (initial pass); corrected 2026-09-22 (Task 05A)
- **Method:** `BASELINE.md` §6 (Payment Plausibility Gate), operationalized per the three-check structure defined in Task 05. Desk research only — official vendor pricing/signup/terms pages as primary sources for Checks 1–2; independent named-customer reviews (Capterra, G2, Shopify App Store, Trustpilot, eBay Community) traced to primary reviewer text for Check 3. No users contacted, no product built, no preorder requested, no landing page created.
- **Correction pass (Task 05A):** the initial pass over-read Check 1 as "the dominant incumbents must be self-serve" rather than "does a relevant paid solution exist with a self-serve path," and blended two structurally different buyers (GC / subcontractor) into one verdict for Candidate 4. Tax Practice Client Portal and eBay/Etsy Cross-Listing were re-examined with targeted, bounded follow-up research and their results changed; Construction Subcontractor Pay-App was split into two buyer-side evaluations. Insurance Commission Reconciliation and Multichannel E-Commerce Accounting Reconciliation (both already PASS) were not re-opened. See each candidate's "What changed" note below.
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

### What changed from the previous pass
The previous pass marked this candidate `KILL` based on Check 1, reasoning from the three dominant incumbents (TaxDome, Canopy, SmartVault) alone — all three require a sales-booked demo before purchase. Task 05A's correction makes explicit that Check 1 asks whether the *category* contains at least one relevant self-serve paid path, not whether the dominant incumbents specifically have one. Financial Cents — already identified in the original pass as a smaller specialist vendor with real named customers, but whose own payment mechanism had never been checked — was verified directly this pass and found to have a genuine, vendor-documented self-serve trial-to-paid checkout. This reverses Check 1, and with it the candidate-level result, from `KILL` to `PASS`.

### Buyer
(unchanged) Small US tax preparation/accounting firms (solo practitioners up to small teams) — owners, partners, bookkeepers, staff accountants selecting practice-management/client-portal software.

### Existing paid solution
TaxDome (taxdome.com), Canopy (getcanopy.com), SmartVault (smartvault.com) — all confirmed demo-gated in the original pass, not re-researched here. **Financial Cents** (financial-cents.com — note: the live domain is hyphenated; `financialcents.com` redirects to it) — verified this pass as a genuine self-serve alternative.

### Check 1 — Visible self-serve pricing
- **Evidence:** Financial Cents' own pricing page (financial-cents.com/pricing, accessed 2026-09-22, page shows "Last Modified: September 10, 2026") publishes exact tiers: Solo $19/mo (1 user, "Cannot add additional users"), Team $49/user/mo annual ($69 monthly), Scale $69/user/mo annual ($89 monthly, "Most Popular"), Enterprise custom/"Contact sales." The homepage CTA "Start your 14-day free trial" links directly to a registration form (app.financial-cents.com/register/), with copy stating: "start a 14-day free trial with just your details and company info. No credit card required, no demo required, no sales call required." Financial Cents' own Help Center article ("How do I Subscribe to a monthly or Annual Plan?") documents the exact in-app self-serve checkout: "You can subscribe by going to Settings > Billing > Subscribe... you will need to input your card... You do not have to reach out to the support team to buy more users." A separate "Book a demo" CTA also exists on the site but coexists with, rather than replaces, the self-serve trial path.
- **Sources:** financial-cents.com/pricing (primary, 2026-09-22, "Last Modified: September 10, 2026"); financial-cents.com/ (primary, 2026-09-22); help.financial-cents.com/en/articles/6295938-how-do-i-subscribe-to-a-monthly-or-annual-plan (primary, vendor help center, 2026-09-22); help.financial-cents.com/en/articles/6079564-pricing-faq-s (primary, 2026-09-22).
- **Decision: PASS** — a relevant, named specialist vendor in this category has a genuine, vendor-documented self-serve trial-to-paid path (registration with no card required, then in-app card entry with no sales conversation required), distinct from the "contact sales" pattern found at TaxDome/Canopy/SmartVault.

### Check 2 — Independent purchase
- **Evidence:** The Solo plan is capped at, and explicitly designed for, 1 user — no minimum-seat barrier for a solo buyer. No mandatory onboarding call or setup fee was found for the standard (Solo/Team/Scale) plans; only Enterprise requires "Contact sales." One real friction point was found: "All plans are a 12-month agreement," and monthly billing is gated to firms with 5+ users — a 1–4-user firm (i.e., most solo/small buyers) must prepay annually to get the advertised rate. This is a contract-term/prepayment constraint, not a procurement, certification, or third-party-approval barrier — the buyer still decides and completes the purchase alone, via self-serve checkout.
- **Sources:** help.financial-cents.com/en/articles/6079564-pricing-faq-s (primary, 2026-09-22).
- **Decision: PASS**, with the 12-month-agreement / 5-seat-monthly-minimum terms recorded as friction, not a structural purchasing barrier of the kind this check targets.

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Unchanged from the original pass — Financial Cents has multiple named, dated 2025 Capterra reviews confirming real paid use, including Megan C. (Principal Owner, Oct 31 2025, 5.0★): "Have used tax dome in the past but felt Financial Cents better fit our needs and was more flexible with better features and price" — an explicit, named switch away from the category's dominant incumbent. No contradicting evidence found this pass.
- **Sources:** capterra.com/p/186837/Financial-Cents/reviews/ (primary named reviewer testimony, previously verified 2026-09-22).
- **Decision: PASS** (unchanged)

### Gate result
**PASS** (corrected from `KILL`)

### Reason
The prior `KILL` conflated "the dominant incumbents are sales-gated" with "no relevant self-serve path exists in the category." Financial Cents — already established under Check 3 as having real named paying customers — was directly verified this pass to have a genuine, vendor-documented self-serve trial-to-paid checkout requiring no sales conversation, which reverses Check 1 and, with it, the candidate-level result.

### Remaining unknowns
The exact registration-form fields at app.financial-cents.com/register/ were not directly observed (the fetch tool was blocked, HTTP 403) — the self-serve claim rests on the vendor's own marketing copy plus its documented in-app billing flow, not a directly observed live signup. Whether the 12-month-agreement / 5-seat-monthly-minimum terms meaningfully deter real solo buyers in practice (versus a true no-commitment monthly product) was not tested.

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

### What changed from the previous pass
The previous pass evaluated this candidate as one buyer and reached a single `KILL` (Check 1 and Check 2 both failed, using GC-side evidence — GCPay, Siteline's quote-only pricing, and the GC-mandate structure — as if it applied to the whole candidate). Task 05A's correction requires GC-side and subcontractor-side purchasing to be evaluated as two separate buyer-side payment structures, since they are economically distinct. This pass re-verifies the GC-side evidence directly (confirming the prior `KILL` for that side) and separately investigates whether a subcontractor can independently buy a *relevant* self-serve tool — finding a more mixed, still-open picture for that side, not a clean `KILL`.

### Buyer
Split explicitly below into GC-side and subcontractor-side, per the correction.

### Existing paid solution
GC-side: GCPay (Autodesk-owned), Built Technologies (getbuilt.com). Subcontractor-side: Siteline (siteline.com, quote-only, confirmed unchanged); Payapps (payapps.com — newly identified, genuine self-serve list pricing, checkout mechanism unconfirmed); Levelset (levelset.com — self-serve pricing exists but for an adjacent problem, sales-gated for the core lien-waiver/pay-app scope).

---

### A. GC-side buyer

#### Check 1 — Visible self-serve pricing
- **Evidence:** GCPay's own current pricing page (ww3.gcpay.com/pricing-for-general-contractors/, re-fetched 2026-09-22) confirms, unchanged: "Custom pricing tailored to your business needs," no published price, CTAs are "Book Demo"/"Get Started" only. Built Technologies publishes one figure ("Lien Waiver Management $1,000/month"), but its actual signup path (getbuilt.com/lien-waiver-management-create-account/) reads "Get started – it's free. No credit card needed" — the live self-serve signup onboards into the **free** product, not a $1,000/mo checkout; the $1,000/mo tier's purchase mechanism remains unconfirmed as self-serve.
- **Sources:** ww3.gcpay.com/pricing-for-general-contractors/ (primary, 2026-09-22); getbuilt.com/products/lien-waiver-management-payments/ and /lien-waiver-management-create-account/ (primary, 2026-09-22).
- **Decision: FAIL** (confirmed, unchanged) — no GC-side vendor checked has a confirmed self-serve paid checkout.

#### Check 2 — Independent purchase
- **Evidence:** GCPay's pricing model requires a "custom pricing" negotiation keyed to "annual subcontracted construction volume" and "number of projects & subcontractors" — a real negotiated-contract process, not self-checkout. Page tone reads as SMB-style lead generation rather than formal RFP/procurement, and GCPay's own case studies (vendor-published, not independent — noted as context only) name moderate-size GCs (e.g., a 75-employee firm), suggesting the negotiation isn't limited to enterprise-scale buyers. But a negotiated custom contract is still required before any GC, large or small, can pay anything — matching this check's own listed barrier category, "complex contracting."
- **Sources:** ww3.gcpay.com/pricing-for-general-contractors/ and /demo/ (primary, 2026-09-22).
- **Decision: FAIL** — even a moderate-size GC must complete a negotiated custom-pricing process before purchasing; this is a structural contracting barrier, not a decision the buyer can complete alone.

#### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Unchanged from the original Discovery/Payment Gate pass — independent, named, dated Capterra reviews of GCPay from March 2026 (Carolinn T., Controller: "I resent being billed to collect our money," confirming real recurring billing; David C.; Mark J.; Staci B.), none vendor-published. (New GCPay case studies surfaced this pass are vendor-published and are noted only as supplementary, non-independent context, per the rule against treating vendor testimonials as independent evidence.)
- **Sources:** capterra.com (GCPay reviews, previously verified, primary named reviewers).
- **Decision: PASS**

#### GC-side result
**KILL** (Check 1 and Check 2 both FAIL)

---

### B. Subcontractor-side buyer

#### Check 1 — Visible self-serve pricing
- **Evidence:** Siteline's own pricing page (siteline.com/pricing, re-fetched 2026-09-22) confirmed unchanged: "We offer custom pricing based on the specific needs of our customers... answer these few quick questions" — no self-serve tier. A newly identified, directly relevant vendor, **Payapps** (payapps.com/uk/pricing-subcontractors/), publishes genuine tiered recurring self-serve prices explicitly for "applications for payment" — Basic £32/mo (1 contract), Standard £85/mo (5), Premium £140/mo (10), Unlimited £270/mo, plus £35/pay-app pay-per-use — directly matching the stated problem. However, whether its "Sign up now" flow (uk.payapps.com/signup) actually collects payment immediately, versus routing to sales-assisted onboarding, could not be confirmed from page content. Levelset's self-serve pricing ($59/recipient for demand/notice letters) addresses an adjacent problem (payment-rights enforcement), not the stated pay-app/change-order/lien-waiver/COI tracking workflow; the parts of Levelset matching the actual problem (fuller lien-waiver management) are sales-gated, not self-serve.
- **Sources:** siteline.com/pricing (primary, 2026-09-22); payapps.com/uk/pricing-subcontractors/ (primary, 2026-09-22); levelset.com/pricing/ and levelset.com/lien-notice/pricing/ (primary, 2026-09-22).
- **Decision: UNKNOWN** — a materially relevant vendor (Payapps) with genuine self-serve list pricing was identified, but its actual checkout mechanism was not confirmed to complete a purchase without a sales conversation. Per this task's correction rule, this is insufficient evidence to resolve either PASS or FAIL, not a basis for KILL.

#### Check 2 — Independent purchase
- **Evidence:** No evidence of a procurement, certification, or committee-approval requirement was found for Payapps — its pricing/signup framing is standard tiered SMB SaaS, unlike GCPay/Siteline's explicit "custom pricing"/negotiated-quote language. No minimum contract term or seat count was found on the Payapps pricing page.
- **Sources:** payapps.com/uk/pricing-subcontractors/ (primary, 2026-09-22).
- **Decision: PASS**, with the caveat that this is tied to the same unconfirmed checkout mechanism flagged in Check 1 — recorded as a lean, not a fully independent confirmation.

#### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** Unchanged from the original pass — independent, named, dated Capterra reviews of Siteline from May 2025 (Jordan C., Owner/President: "transformed the way my company processed billings"; Veronica C.; Holly S.; McKenzie P., switched from Sage 100) confirm subcontractors do pay for sub-side specialist tools. This evidence is for **Siteline** specifically (the quote-only vendor) — no customer reviews were found for **Payapps** (the self-serve-priced vendor) this pass. The vendor with confirmed paid precedent and the vendor with confirmed self-serve pricing are, currently, not the same product.
- **Sources:** capterra.com/p/252004/Siteline/ (primary, previously verified 2026-09-22).
- **Decision: PASS** — for the general claim that subcontractors independently purchase specialist sub-side tools; this does not by itself confirm Payapps has any customers.

#### Subcontractor-side result
**BLOCKED / INCONCLUSIVE** — Check 1 is UNKNOWN (no check FAILs, so this is not a KILL, but Check 1 is not confirmed PASS either).

---

### Buyer-side summary

| Buyer side    | Check 1 | Check 2 | Check 3 | Result |
| ------------- | ------- | ------- | ------- | ------ |
| GC            | FAIL    | FAIL    | PASS    | **KILL** |
| Subcontractor | UNKNOWN | PASS (leaning, tied to Check 1 gap) | PASS | **BLOCKED / INCONCLUSIVE** |

### Is the candidate too broad?
**Yes.** The evidence shows GC-side and subcontractor-side are two structurally distinct payment mechanics, not one problem domain with one verdict. GC-side purchasing is confirmed negotiated-custom-contract, clearly gated (`KILL`). Subcontractor-side purchasing has at least one vendor (Siteline) with confirmed paying customers but no self-serve pricing, and at least one vendor (Payapps) with confirmed self-serve pricing but no confirmed customers or checkout mechanism — a genuinely open question, not a clean pass or fail. If this candidate is investigated further, GC-side and subcontractor-side should be tracked as separate lines of evidence rather than re-merged into one problem domain. This is a factual observation about the evidence gathered, not a proposal to create two new candidates — none are introduced by this task.

### Gate result
**Split — GC-side: KILL. Subcontractor-side: BLOCKED/INCONCLUSIVE.** No single candidate-level verdict is recorded, per the finding above that these are not one payment-plausibility profile.

### Remaining unknowns
Whether Payapps' "Sign up now" flow actually completes a self-serve purchase (vs. routing to a sales-assisted process) — this is the single fact that would resolve the subcontractor-side Check 1 from UNKNOWN to PASS or FAIL. Whether Payapps has any named, current paying customers. Whether GCPay's quote-request process is functionally heavier than it reads (form fields could not be directly observed — JS-rendered). No first-person subcontractor complaint specifically describing being charged a GC-passed fee was found (the fee-passthrough mechanism is vendor-documented, but a named sub's own account of experiencing it was not located).

---

## Candidate 5 — eBay/Etsy Cross-Listing & Listing-Template Management

### What changed from the previous pass
Check 3 was previously `UNKNOWN` because the only named-user evidence found (an eBay Community forum thread) confirmed active use but not paid status, since LitCommerce and FolderLister both offer a trial/free tier. This pass searched specifically for explicit, named, dated paid-status confirmation and found it for LitCommerce: two independent, named/identifiable Trustpilot reviewers, dated within the 2025–2026 window, explicitly describe paying for or being charged by LitCommerce. This resolves Check 3 to `PASS` and reverses the candidate-level result from `BLOCKED/INCONCLUSIVE` to `PASS`.

### Buyer
(unchanged) Long-tenured eBay/Etsy power sellers and small multichannel resellers who pay monthly for a listing-management/template subscription, displaced by InkFrog's April–June 2026 shutdown.

### Existing paid solution
(unchanged) LitCommerce (litcommerce.com), Sixbit (sixbitsoftware.com), FolderLister (folderlister.com).

### Check 1 — Visible self-serve pricing
(Unchanged from the previous pass — not re-researched this pass, no contradicting evidence encountered.) **PASS** — all three named alternatives have genuine, working self-serve checkout with no sales-call gate at any tier (LitCommerce: "START FREE TRIAL" → real registration, 7-day trial; Sixbit: "TRY FREE" → direct checkout cart, 30-day trial; FolderLister: "Subscribe" → Stripe checkout, plus a genuine $0 tier).

### Check 2 — Independent purchase
(Unchanged from the previous pass — not re-researched this pass, no contradicting evidence encountered.) **PASS** — no procurement, minimum-term (beyond an avoidable optional annual discount at LitCommerce), or certification barrier found for any of the three.

### Check 3 — Small/specialist vendor purchase precedent
- **Evidence:** **LitCommerce** — two named, identifiable Trustpilot reviewers explicitly confirm paid status, both dated within the 2025–2026 window: **Lingo Lohr** (★3, Feb 17 2026): "I paid for their annual plan based on the reviews but requested refund within 30 days... because they want you to stick to them to continue to pay annual fee!" — explicit first-person paid statement. **Shizonic** (★1, Nov 17 2025): "A payment was charged from my bank for LitCommerce, and I provided full evidence: screenshots from Shopify, my bank statement, transaction details..." — explicit charge confirmation. Both are negative/complaint reviews, which if anything increases credibility (no incentive to fabricate paid status), and both are primary Trustpilot reviews from named/identifiable accounts, re-confirmed against LitCommerce's still-active 7-day trial (meaning sustained, charged use past that window is not explainable by a free tier).
  **FolderLister** — remains unconfirmed: its free tier was directly verified as permanent/non-expiring ("The free tier is permanent, not a trial... no expiry date and no card required," per FolderLister's own pricing FAQ), which undercuts any tenure-based inference. Only one review was found (an anonymous G2 "Verified User in Retail," 4/18/2026, no plan tier or volume stated), and FolderLister has no Trustpilot or Capterra review presence at all (both directly checked, neither exists).
  **Sixbit** — unambiguous paid confirmation exists but outside the preferred freshness window: Laura S. (★5, June 26 2024): "The monthly price is extremely reasonable"; Trish R. (★5, Aug 8 2024): "Prices are going up a bit in Sept. 2024." Capterra's full Sixbit review set is confirmed exhaustive (16 of 16 shown) with nothing newer than Dec 2024 — no 2025–2026 named Sixbit customer evidence exists to find.
- **Sources:** trustpilot.com/reviews/6993eb9273a6149a58d43524 (Lingo Lohr, primary, named, 2026-02-17); trustpilot.com/reviews/691bb435f5d6fe6d1fd05130 (Shizonic, primary, named, 2025-11-17); folderlister.com/ pricing FAQ (primary, 2026-09-22); g2.com/products/folderlister/reviews (primary, 2026-09-22); capterra.com/p/178178/SixBit-Software/reviews/ (primary, named, 2024 dates, confirmed exhaustive).
- **Decision: PASS** — LitCommerce alone provides sufficient, current (2025–2026), named, primary-source, explicitly-paid customer precedent for this buyer type purchasing from a small/specialist vendor. This does not extend to FolderLister (still genuinely unconfirmed) or close Sixbit's recency gap, but the check only requires evidence that this buyer type purchases from *a* relevant small/specialist vendor, which LitCommerce now satisfies unambiguously.

### Gate result
**PASS** (corrected from `BLOCKED/INCONCLUSIVE`)

### Reason
The previous `BLOCKED/INCONCLUSIVE` result was the correct call given the evidence available at the time (confirmed activity, unconfirmed payment). This pass found explicit, named, dated, primary-source confirmation of paid status for LitCommerce specifically — two independent complaint reviews that incidentally document real charges — which is sufficient to resolve Check 3 without inventing evidence.

### Remaining unknowns
FolderLister's and Sixbit's current (2025–2026) paid-customer status remain unconfirmed — FolderLister: genuinely open, its permanent free tier makes tenure a weak signal on its own; Sixbit: paid status is well-confirmed historically but not within the preferred freshness window. Neither affects this candidate's `PASS` result, since Check 3 only requires one relevant vendor's precedent, but both remain open questions if this candidate is investigated further at the next gate.

---

## Cross-Candidate Observations

*Methodological observations only — no ranking of candidates.*

- **"Contact sales despite a published, non-negotiable price" is a distinct failure mode from pure quote-only pricing**, and both were encountered in this pass (Candidate 2's dominant incumbents TaxDome/Canopy/SmartVault = published-but-demo-gated; Candidate 4's GCPay/Siteline = no price published at all). Both correctly fail Check 1 *for those specific vendors* under the task's own instruction not to treat "contact us" as self-serve, but future gate applications should keep recording which sub-pattern applies, since the two failure modes carry different implications (a published price at least signals the vendor doesn't negotiate case-by-case, even if the checkout mechanism itself isn't self-serve).
- **Review-tenure claims ("used it for 3 years," "using the app for over 1 year") on Capterra/Shopify App Store are a useful but imperfect proxy for confirmed paid status.** They strongly suggest sustained real usage but do not, on their own, rule out an extended free/trial tier, especially for products that offer a permanent free tier or an unusually long trial (as encountered with FolderLister in Candidate 5). Explicit first-person statements of payment or being charged (as eventually found for LitCommerce) are categorically stronger than tenure inference and should be actively searched for before defaulting to UNKNOWN.
- **A dual-sided buyer definition (Candidate 4's "GCs and subcontractors") can contain two structurally different Payment Plausibility profiles at once** — one side (GC) that purchases via custom quote, one side (subcontractor) that is often mandated onto the GC's chosen platform but can independently buy a *different*, complementary tool to cope with that mandate. Blending the two into one verdict (as the initial pass did) produces a misleading result; recording both sides explicitly, as a corrected pass, was necessary to reach a defensible verdict at all.
- **(Task 05A correction) Check 1 must be evaluated at the category/relevant-vendor level, not at the level of whichever vendor happens to be the largest or most frequently cited incumbent.** The initial pass's Candidate 2 `KILL` was driven entirely by checking the three most prominent incumbents and stopping there; a smaller, already-identified specialist vendor (Financial Cents) turned out to have a genuine self-serve path the first pass never checked. This is a general methodological risk — discovery evidence naturally surfaces the loudest/largest incumbents first, and Check 1 must not be resolved on their evidence alone before at least one smaller, already-named alternative has been directly checked.

---

## Methodological Issues

None found. The three-check structure specified in this task is consistent with, and a direct operationalization of, `BASELINE.md` §6's three questions and decision rule; no contradiction between this task's instructions and `BASELINE.md`/`BASELINE_PATCH.md`/`DECISION.md` was encountered while applying the gate.

---

## Corrected Gate Summary

| Candidate | Check 1 | Check 2 | Check 3 | Final |
| --- | --- | --- | --- | --- |
| Insurance Commission Reconciliation *(not re-opened, unchanged)* | PASS | PASS | PASS | PASS |
| Multichannel E-Commerce Accounting Reconciliation *(not re-opened, unchanged)* | PASS | PASS | PASS | PASS |
| Tax Practice Client Portal | PASS *(corrected)* | PASS | PASS | **PASS** *(corrected from KILL)* |
| Construction Pay-App / Lien Waiver — GC side | FAIL | FAIL | PASS | **KILL** |
| Construction Pay-App / Lien Waiver — Subcontractor side | UNKNOWN | PASS | PASS | **BLOCKED/INCONCLUSIVE** |
| eBay/Etsy Cross-Listing | PASS | PASS | PASS *(corrected)* | **PASS** *(corrected from BLOCKED/INCONCLUSIVE)* |

No ranking is implied by table order. Construction Pay-App / Lien Waiver has no single Final value because the evidence shows it is not one payment-plausibility profile — see "Is the candidate too broad?" above.

---

## Next Research

*Only the next gate to investigate is named below — it is not performed in this task.*

- **Insurance Commission Reconciliation (PASS, unchanged):** next gate per `BASELINE.md` ordering is Switching Feasibility & Switching Destination (§8).
- **Multichannel E-Commerce Accounting Reconciliation (PASS, unchanged):** same next step — Switching Feasibility & Switching Destination (§8).
- **Tax Practice Client Portal (PASS, corrected):** now eligible for Switching Feasibility & Switching Destination (§8) — `DISCOVERY.md` already recorded ≥7 named, dated switching accounts between TaxDome and competing products that now need to be checked against lock-in, contractual constraints, and realistic-alternative-availability per §8, specifically re-examined in light of Financial Cents as a documented, genuinely self-serve destination.
- **eBay/Etsy Cross-Listing (PASS, corrected):** now eligible for Switching Feasibility & Switching Destination (§8) — the InkFrog-shutdown switching evidence already on record in `DISCOVERY.md` needs the same §8 treatment.
- **Construction Pay-App / Lien Waiver — GC side (KILL):** no further research proposed. Per `DECISION.md`'s global rule, not reopened without materially new evidence — specifically, evidence that a GC-side vendor offers a genuinely self-serve, non-custom-quoted purchase path.
- **Construction Pay-App / Lien Waiver — Subcontractor side (BLOCKED/INCONCLUSIVE):** does not advance to the next gate yet. The specific open question to resolve first is Check 1 — whether Payapps' (or another relevant sub-side vendor's) signup flow completes a genuine self-serve purchase, and whether Payapps has any named, current paying customers.
