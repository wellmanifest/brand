# wellmanifest/brand (standard pointer)

**Standards pack only.** Product brand kits do **not** HOME here.

| Concern | HOME | Role of this pack |
| --- | --- | --- |
| Colors, logos, voice, closed vocabulary | [`subactor/brand`](https://github.com/subactor/brand) | Normative ADOPT rules below |
| Public plan names used on commercial sheets | `subactor/brand` vocabulary + `subactor/offer` amounts | Sites ADOPT both; no parallel brand SSOT |

Do not place Subactor (or other product) brand assets, `dsl-manifest` profiles, or vocabulary under `wellmanifest/brand`. An earlier empty mistaken HOME is abandoned; this repository only states the standard.

## Normative rules (ADOPT)

When a runtime, portal, offer sheet, or social channel publishes brand copy or tokens:

1. **HOME** brand tokens and closed vocabulary in a product pack under `subactor` (canonical: `subactor/brand`).
2. Sites and marketing channels **ADOPT** the product brand profile; they must not invent a second token or prefer/forbid list in portal tickets.
3. `subactor/offer` (and other commercial packs) MUST reuse brand vocabulary for public plan names and metering language; amounts stay in the offer pack.
4. Classify portal CSS tokens / copy facades as `facade` or `locale_catalog` over the product brand pack (`wellmanifest/ssot`); gate drift before merge when tokens or forbidden terms diverge.
5. Feature tickets MUST NOT rewrite brand facades as a parallel SSOT. Integration workstreams bump the brand profile first, then re-pin consumers.

## Placement

| Field | Value |
| --- | --- |
| home | wellmanifest |
| shape | domain_pack |
| product content | HOME `subactor/brand` (ADOPT this standard) |

See also: `wellmanifest/offer` (commercial sheets), `wellmanifest/new-project` commercial + brand SSOT rules, `wellmanifest/modularity` single-exporter contracts.
