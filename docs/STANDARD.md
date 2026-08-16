# Brand adoption standard

## Objects

| Object | Role | Owner |
| --- | --- | --- |
| Brand profile | Tokens, logo rules, voice | Product pack (`subactor/brand`) |
| Vocabulary | Preferred / forbidden / aliases | Product pack |
| Site facade | CSS tokens, UI copy, marketing projection | Runtime / channel (ADOPT) |

## Invariants

1. One product brand profile is authoritative for a given product HOME.
2. Offer catalogs reuse vocabulary for public naming; they do not fork prefer/forbid lists.
3. Portal and social facades MUST NOT introduce competing brand tokens or forbidden terms without a brand profile bump.
4. Drift gates fail closed before merge when facade tokens or public names diverge from the adopted profile.

## Adopting on a new site

1. ADOPT the product brand pack and pin the profile version used by the site.
2. Map CSS / i18n / marketing copy to the profile; keep local files as facades.
3. Validate offer display names against brand vocabulary when publishing commercial sheets.
4. Gate CI / review on vocabulary and token drift before merge.
