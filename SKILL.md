---
name: affiliate-content-sync
description: "Audit affiliate or partner-facing promotional content against the current website source of truth, then draft update guidance and outreach messages. Use when the user provides affiliate article links, partner roundup URLs, current product prices, bundle definitions, promotion updates, renamed products, partner-specific offer overrides, gift-policy changes, or offer changes and wants: (1) a content-diff audit, (2) instructions for affiliates who already published to update outdated copy, prices, bundles, gifts, or CTAs, (3) a current promotion brief for affiliates who have not published yet, or (4) softer relationship-preserving outreach that keeps an active partner offer while correcting supporting details or introducing a missing product. Trigger on requests about affiliate updates, partner notifications, outdated recommendation pages, promo sync, pricing or bundle changes, gift policy changes, co-branded offer status, or Chinese-language requests about notifying affiliate partners about website changes."
---

# Affiliate Content Sync

## Goal

- Keep affiliate-facing content aligned with the current website truth.
- Separate two jobs clearly:
  1. fix already-published affiliate content
  2. send current promotion guidance to affiliates who have not published yet
- Turn raw links and offer changes into partner-ready instructions, not just analysis.

## Priority Rules

1. Treat the user's latest website pricing, bundle, and promotion details as the primary source of truth.
2. Treat explicit user overrides as higher priority than scraped site content when the user is clarifying the live approved offer.
3. If the user provides a product table or bundle sheet, preserve its naming and numbers exactly.
4. Separate confirmed facts from suggested rewrites. Never blur the two.
5. Distinguish public promotions from partner-specific or co-branded offers. Do not tell a partner to remove an offer that the user says is still active unless the user explicitly asks for that.
6. When prices changed and the approved current numbers are known, list the exact changed products and current prices instead of telling the partner to broadly recheck pricing.
7. If a product has multiple options, variants, or configurations with distinct current prices, list each approved option and its price separately. Do not skip the product just because there is more than one valid price.
8. Do not invent discounts, bundle items, free gifts, coupon codes, end dates, regional availability, or seeding promises.
9. Preserve partner-specific context such as language, market, relationship tone, and page format when drafting updates.
10. If the user gives a required output format, use it exactly.

## Gather Inputs

Collect or confirm these inputs before drafting:

- Current site truth:
  - product names
  - product URLs
  - current prices
  - compare-at prices if relevant
  - bundle names
  - bundle contents
  - promo mechanics such as coupon, free gift, or limited-time note
  - effective dates if explicitly known
  - user-provided overrides that supersede the scraped site
  - partner-specific or co-branded offers that may still be active even when a public promo has changed
  - gift policy type: purchase-based, subscription-based, manual add-on, or no gift
- Affiliate partner context:
  - partner name
  - affiliate page URL
  - page status: published, not published, or unknown
  - target language
  - target market or region
  - any existing relationship notes from the user
  - preferred message style: direct correction, soft update, or expansion opportunity
  - missing products the user wants added to the article
  - seeding or review-unit status if the user wants to mention shipping a product
- Delivery requirements:
  - internal analysis language
  - partner-facing message language
  - email, DM, sheet row, or comment format
  - whether to include subject lines or follow-up reminders

If a required fact is missing and the gap would change the recommendation materially, state the gap explicitly instead of guessing.

## Workflow

1. Build the source-of-truth snapshot from the user's latest data.
2. Create an override ledger before comparing pages:
   - user-confirmed prices
   - user-confirmed gift policy
   - partner-specific active offers
   - approved talking points for missing products
3. Open each affiliate URL and extract only the claims that matter for synchronization:
   - product names
   - prices
   - bundle descriptions
   - promo language
   - CTA wording
   - landing links if visible
4. Classify each affiliate URL into one of these states:
   - current
   - outdated
   - partially outdated
   - no publish yet
   - cannot verify
5. Compare the affiliate page against the current site truth field by field, using the override ledger first whenever the user has clarified a fact.
6. Convert every mismatch into an action item with explicit before/after guidance.
7. If exact current prices are confirmed, replace generic advice with a concrete changed-price list.
   - if multiple approved options exist, include each option explicitly
8. Draft partner-facing communication in the appropriate lane:
   - published partner: correction and replacement guidance
   - unpublished partner: current promo brief and publishing suggestions
   - relationship-preserving published update: keep active partner offers intact while correcting supporting details
   - article expansion: ask the partner to add a missing product and mention seeding only if the user approved that message
9. End with open questions only if they block accurate messaging.

## What To Compare

Always compare these items when available:

- product naming and model/version naming
- standalone prices
- variant or option prices when a product has multiple valid configurations
- bundle names
- bundle contents
- savings framing
- public coupon or code mentions
- partner-specific or co-branded offer mentions
- gift-with-purchase claims
- gift policy type: purchase-based vs subscription-based vs manual add-on
- promo timing or urgency language
- CTA angle
- landing-page destination
- region-specific claims
- stock or availability statements
- products missing from the article that the user now wants included

Read [references/change-taxonomy.md](references/change-taxonomy.md) when you need a compact checklist for mismatch types, severity, and recommended actions.

## Published Partner Output

For partners who already published, produce:

1. A short diagnosis:
   - what is on the page now
   - what is outdated or risky
2. A fix list:
   - exact field to change
   - current approved replacement
   - whether the issue is mandatory or recommended
   - explicit changed prices when confirmed
   - each variant price when more than one approved option exists
3. A partner-facing message:
   - concise
   - easy to forward
   - specific enough that the partner can update quickly
   - matched to the requested relationship style

Default structure:

### Internal Audit

- Partner:
- URL:
- Status:
- Key mismatches:
- Mandatory fixes:
- Optional improvements:

### Partner Message

- Subject or opener
- Short explanation of what changed
- Bullet list of required updates
- Approved replacement facts
- CTA asking them to refresh the page

When helpful, include replacement copy for the exact outdated sentence or bullet.

## Relationship Style Modes

Choose the message style based on the user's instruction and partner context:

- `direct correction`
  - Use when accuracy matters more than diplomacy.
  - State the outdated facts and required replacements plainly.
- `soft update`
  - Use when the partner relationship should be preserved and the main co-branded offer is still active.
  - Lead with what remains valid, then mention only the supporting details that need to be refreshed.
  - Avoid calling out an expired public code if the user says the partner's active offer is still approved.
- `expansion opportunity`
  - Use when the article is missing a product the user wants featured.
  - Pair the correction note with an invitation to add the product.
  - Mention shipment, seeding, or a review unit only if the user explicitly says it has been or will be sent.

## Unpublished Partner Output

For partners who have not published yet, produce:

1. A current promotion brief
2. The approved product and bundle facts
3. Suggested angles for the partner's audience
4. A ready-to-send outreach message

Keep unpublished-partner outreach focused on what is new and worth publishing now. Do not overload it with audit detail that only matters for already-live pages.

## Language Rules

- Match the user's requested language first.
- If the user does not specify:
  - keep internal analysis in Chinese
  - keep partner-facing copy in the affiliate page language when obvious
  - otherwise default partner-facing copy to English
- If the partner page is in a different language from the website data, preserve the facts exactly and localize only the surrounding wording.

## Guardrails

- Do not fabricate facts that are not present in the user's source-of-truth data or the verified website.
- Do not let scraped site details override a newer explicit user correction.
- Do not carry over expired promo language just because it appears on an affiliate page.
- Do not confuse a public expired code with an active partner-specific offer.
- Do not describe a subscription-only gift as a purchase-based free gift.
- Do not skip a product price update only because the product has two options or two valid current prices.
- Mark uncertain items as unverified instead of treating them as true.
- Do not recommend misleading urgency, stock, or discount claims.
- Distinguish clearly between:
  - approved fact
  - suggested positioning
  - inferred opportunity

## Default Deliverables

Unless the user specifies another format, deliver these sections in order:

1. `Current Website Change Summary`
2. `Published Partners Requiring Updates`
3. `Unpublished Partners To Notify`
4. `Open Questions`

If there are many URLs, use a compact table first and then provide partner-ready messages below it.

Read [references/output-templates.md](references/output-templates.md) when you need reusable table layouts or message templates for published and unpublished partners.
