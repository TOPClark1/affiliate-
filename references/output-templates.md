# Output Templates

Use these templates unless the user provides a stricter format.

## 1. Compact Audit Table

Use this when many affiliate URLs need review.

| Partner | URL | Status | Change Type | Required Update | Severity |
| --- | --- | --- | --- | --- | --- |
| Partner A | https://... | outdated | price-change | Update Product X from $99 to $89 | mandatory |

## 2. Published Partner Internal Summary

```md
### {Partner Name}

- URL: {url}
- Status: {current / outdated / partially outdated / cannot verify}
- Key mismatches:
  - {mismatch 1}
  - {mismatch 2}
- Mandatory fixes:
  - {approved replacement fact 1}
  - {approved replacement fact 2}
- Optional improvements:
  - {suggested refinement 1}
```

## 3. Published Partner Message

```md
Subject: Quick update needed for your {brand/product} content

Hi {Partner Name},

We noticed a few details on your published page that no longer match our current website offer. Could you please update the page when convenient?

Please update:
- {old fact} -> {approved new fact}
- {old fact} -> {approved new fact}

Current approved details:
- {product or bundle name}
- {current price}
- {bundle contents or promo mechanic}

If helpful, we can also send replacement wording for the relevant section.
```

## 4. Unpublished Partner Brief

```md
### {Partner Name}

- Status: no publish yet
- Current angle to share:
  - {new offer or bundle hook}
- Approved facts:
  - {product / bundle / price}
  - {promo mechanic if verified}
- Suggested audience fit:
  - {traveler / creator / desk setup / gifting / etc.}
```

## 5. Unpublished Partner Outreach

```md
Subject: Current {brand} offer you can feature

Hi {Partner Name},

We wanted to share our current website offer in case you would like to publish or refresh coverage.

Current approved details:
- {product or bundle name}
- {current price}
- {bundle contents}
- {verified promo notes only}

Possible angles:
- {angle 1}
- {angle 2}

If you want, we can also send a short product summary or recommended copy points for your audience.
```

## 6. Open Questions Block

```md
## Open Questions

- {missing price / missing bundle detail / unclear language / inaccessible page}
- {why it matters}
```

## Usage Notes

- Keep partner-facing copy short enough to forward without editing.
- Replace placeholders with confirmed facts only.
- If the user requests sheet-ready output, flatten the same information into columns instead of prose.
