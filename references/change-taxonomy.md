# Change Taxonomy

Use this file when classifying affiliate-page mismatches against the current website truth.

## Core Mismatch Types

- `price-change`
  - The listed price no longer matches the website.
  - Usually a mandatory fix.
- `bundle-change`
  - Bundle name, included products, or savings framing changed.
  - Usually a mandatory fix.
- `promo-expired`
  - The affiliate page still mentions an expired or unverified offer.
  - Mandatory fix.
- `product-rename`
  - Product name, model label, or version naming changed.
  - Mandatory if it affects user understanding or search intent.
- `cta-stale`
  - CTA angle or landing page no longer reflects the current offer.
  - Recommended or mandatory depending on severity.
- `claim-unverified`
  - The affiliate page states a gift, deadline, percentage-off, or availability claim that the current website truth does not confirm.
  - Mandatory fix.
- `region-mismatch`
  - The page uses pricing, shipping, or availability language that does not match the target market.
  - Mandatory when the partner serves a specific region.
- `content-gap`
  - The partner has no live content yet.
  - Use unpublished-partner outreach flow.
- `cannot-verify`
  - The page cannot be accessed or the relevant section cannot be found.
  - Escalate as an open question instead of guessing.

## Severity Guide

- `mandatory`
  - Wrong price
  - Wrong bundle contents
  - Expired promo
  - Unverified gift or coupon
  - Wrong product naming
- `recommended`
  - Better CTA alignment
  - Better angle based on the new bundle
  - Refreshing screenshots or headings
- `optional`
  - Tone polish
  - Reordering content blocks

## Minimal Audit Fields

For each partner URL, capture:

- partner name
- page URL
- page status
- mismatch type
- current page wording or fact
- approved replacement fact
- severity
- note to partner

## Escalation Rules

- If the user-provided website truth conflicts with the live site, prioritize the user's explicit latest instruction and mention the discrepancy.
- If dates are missing for a time-sensitive offer, avoid deadline language in partner-facing copy.
- If the bundle is known but the bundle savings math is not explicitly confirmed, describe the bundle contents and current price without inventing savings percentages.
