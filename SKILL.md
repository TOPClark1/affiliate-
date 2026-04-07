---
name: affiliate-content-sync
description: "Audit affiliate or partner-facing promotional content against the current website source of truth, then draft update guidance and outreach messages. Use when the user provides affiliate article links, partner roundup URLs, current product prices, bundle definitions, promotion updates, renamed products, or offer changes and wants: (1) a content-diff audit, (2) instructions for affiliates who already published to update outdated copy, prices, bundles, or CTAs, or (3) a current promotion brief for affiliates who have not published yet. Trigger on requests about affiliate updates, partner notifications, outdated recommendation pages, promo sync, pricing or bundle changes, or Chinese-language requests about notifying affiliate partners about website changes."
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
2. If the user provides a product table or bundle sheet, preserve its naming and numbers exactly.
3. Separate confirmed facts from suggested rewrites. Never blur the two.
4. Do not invent discounts, bundle items, free gifts, coupon codes, end dates, or regional availability.
5. Preserve partner-specific context such as language, market, and page format when drafting updates.
6. If the user gives a required output format, use it exactly.

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
- Affiliate partner context:
  - partner name
  - affiliate page URL
  - page status: published, not published, or unknown
  - target language
  - target market or region
  - any existing relationship notes from the user
- Delivery requirements:
  - internal analysis language
  - partner-facing message language
  - email, DM, sheet row, or comment format
  - whether to include subject lines or follow-up reminders

If a required fact is missing and the gap would change the recommendation materially, state the gap explicitly instead of guessing.

## Workflow

1. Build the source-of-truth snapshot from the user's latest data.
2. Open each affiliate URL and extract only the claims that matter for synchronization:
   - product names
   - prices
   - bundle descriptions
   - promo language
   - CTA wording
   - landing links if visible
3. Classify each affiliate URL into one of these states:
   - current
   - outdated
   - partially outdated
   - no publish yet
   - cannot verify
4. Compare the affiliate page against the current site truth field by field.
5. Convert every mismatch into an action item with explicit before/after guidance.
6. Draft partner-facing communication in the appropriate lane:
   - published partner: correction and replacement guidance
   - unpublished partner: current promo brief and publishing suggestions
7. End with open questions only if they block accurate messaging.

## What To Compare

Always compare these items when available:

- product naming and model/version naming
- standalone prices
- bundle names
- bundle contents
- savings framing
- coupon or code mentions
- gift-with-purchase claims
- promo timing or urgency language
- CTA angle
- landing-page destination
- region-specific claims
- stock or availability statements

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
3. A partner-facing message:
   - concise
   - easy to forward
   - specific enough that the partner can update quickly

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
- Do not carry over expired promo language just because it appears on an affiliate page.
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
