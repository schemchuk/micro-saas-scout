# Micro-SaaS Scout — Agent Rules

These rules apply to Claude Code, Kimi, and any other research agent working in this repository.

## 0. Language & Git workflow

- Always communicate with the user in Ukrainian.
- At the end of every logical block of work, the agent that performed the task must commit and push the changes to the main branch.

## 1. Optimize for decisions, not document volume

Every research task must produce one of:

- KEEP
- TEST
- KILL
- BLOCKED
- INCONCLUSIVE

Do not create phases merely because more research is possible.

A longer report is not evidence of a better opportunity.

## 2. Do not repeat the old methodology

Do not default to:

`marketplace → keyword sweep → competitor count → scoring → another keyword sweep`

Marketplace research is allowed only when the marketplace itself is the proposed acquisition/discovery channel.

Do not treat "low competition" as proof of demand.

Do not treat a small review count, small install count, or young competitor as proof that a new entrant can acquire customers.

## 3. Distribution must be part of the hypothesis

For every serious candidate, identify:

`Problem → Buyer → Existing spending/effort → Existing solution → Observable dissatisfaction → Product wedge → Discovery channel → First payment`

A candidate without a credible discovery mechanism does not advance merely because the problem sounds painful.

## 4. Prefer evidence of behavior

Strong evidence includes:

- people already paying;
- repeated complaints about an existing paid solution;
- customers actively comparing alternatives;
- migration/switching discussions;
- recurring operational workarounds;
- clear requests for a missing capability;
- active search/discovery behavior;
- evidence that a small product can be adopted without long procurement.

Weak evidence includes:

- "there must be demand";
- social-media likes alone;
- a large theoretical market;
- a problem that only sounds annoying;
- a competitor with few reviews;
- a founder's personal intuition.

## 5. Timebox research

No candidate may consume an open-ended research cycle.

For each serious hypothesis, quickly determine:

1. Is the pain real?
2. Is someone willing to pay or already paying?
3. Can a solo developer build a narrow solution?
4. Can customers discover it without cold outreach?
5. Can the first payment be tested cheaply?

If a candidate fails a critical question, stop researching it.

## 6. No premature building

Do not write production code, design a full architecture, or build a polished MVP before the hypothesis survives validation.

A lightweight landing page, clickable mockup, waitlist, manual concierge test, or other cheap experiment may be appropriate.

## 7. No scoring theater

Do not use arbitrary weighted scores to manufacture precision.

Use explicit evidence and hard gates.

When evidence is mixed, say so.

## 8. Separate facts from interpretation

For each important claim:

- state the observed fact;
- identify the source;
- distinguish inference from the source's own statement;
- record uncertainty where relevant.

Never turn a source's opinion into an established fact.

## 9. Record dead ends

A killed hypothesis should be documented briefly with:

- hypothesis;
- decisive evidence;
- reason for kill;
- what lesson it provides.

Do not keep reopening a killed hypothesis unless new evidence materially changes the situation.

## 10. Avoid support-heavy products

Flag products that would create:

- 24/7 operational expectations;
- complex integrations;
- security/compliance obligations disproportionate to revenue;
- frequent customer-specific configuration;
- high-touch onboarding;
- difficult migration work.

This is not an automatic rejection, but it is a major risk for a solo developer.

## 11. Stop conditions

Research must stop and move to validation when:

- one candidate has a specific buyer;
- the pain is evidenced by real behavior;
- existing spending or a credible willingness-to-pay signal exists;
- a narrow wedge is identifiable;
- a discovery channel is plausible;
- the validation experiment can be run cheaply.

Research must also stop when the available evidence repeatedly fails these gates.

The objective is to learn whether a business can work, not to produce an exhaustive market map.
