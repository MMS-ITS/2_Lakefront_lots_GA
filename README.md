# Comprehensive Lot Due-Diligence — Two Georgia Lakefront Lots

| | Property A | Property B |
|---|---|---|
| **Address** | 12396 Edgewater Dr #23, Hampton, GA 30228 | 1147 & 1153 Watersedge Cove, Lots 130 & 131, Tignall, GA 30668 |
| **Subdivision** | Waterpointe, Unit 3 Lot 23 | Stillwater Coves |
| **County** (verified) | **Clayton County**, unincorporated — *not Henry* | **Lincoln County** — *not Wilkes* |
| **Size** | 1.3304 ac (57,954 sq ft, measured) | 2.14 ac (two 1.07-ac lots) |
| **Water body** | J.W. Smith Reservoir — CCWA drinking-water supply | Clarks Hill / J. Strom Thurmond Lake — USACE |
| **Parcel / APN** | `05050A A003` | `10A 130` |
| **Asking** | $125,000 / $98,000 (sources conflict) | $55,000 both lots |

## The deliverable

**[`Lot-Due-Diligence-Report.html`](Lot-Due-Diligence-Report.html)** — a single self-contained
interactive HTML report covering all 61 checklist items for both properties side by side.
No external dependencies: open it in any browser.

**[`Lot-Due-Diligence-Report.pdf`](Lot-Due-Diligence-Report.pdf)** — the same report exported to
**A4 portrait, 83 pages, with "Page N of 83" on every page**.

To regenerate the PDF yourself: open the HTML and use **Print → Save as PDF**. The stylesheet sets
A4 portrait and the page numbering is produced by native CSS page margin boxes (Chrome/Edge).

### Interactive controls in the HTML version

| Figure | Controls |
|---|---|
| Plat-equivalent boundary map | 7 layer toggles (lot, adjacent parcels, roads, buildings, reservoir, 150-ft buffer, dimensions) |
| Aerial overlays | Boundary / buffer / section-line toggles, overlay opacity, 330-ft and 346-ft contour lines |
| Topographic maps | Contour interval (5/10/20 ft), labels, hypsometric tint, high-low points, drainage arrow |
| Cross-sections | **Vertical-exaggeration slider (1×–10×) with a true 1:1 panel always shown beside it** |
| Slope diagram | True 1:1 panels, angle annotations |
| 3-D terrain | Rotate, tilt, vertical exaggeration, water surface, lot outline |
| Building envelope | Setbacks, buffer, envelope, house footprint, septic area, contours |

## What was measured rather than assumed

- **Terrain** — USGS 3DEP **1-metre lidar** DEMs (`GA_Central_2019_B19` and the Georgia 3DEP
  coverage), resampled over an 840 × 840 m window at each lot. Contours, true-scale sections,
  3-D surfaces, slope over **every** 50-ft run, drainage aspect.
- **Property A boundary** — the Clayton County Tax Assessor's live parcel service; 5 corners,
  perimeter cross-checked against the county's own figure to **0.1 ft**.
- **Flood zone** — FEMA National Flood Hazard Layer queried at the exact coordinates.
  Both lots: **Zone X, minimal hazard, no BFE**.
- **Soils** — USDA NRCS SSURGO: full horizon profiles plus engineering interpretations.
- **Aerial imagery** — USGS NAIP orthoimagery (public domain).

## Headline findings

1. **Both counties in the brief were wrong**, and the corrections change the zoning, septic,
   permitting, tax and short-term-rental rules that apply. Verified against the US Census Bureau
   geocoder and each county's own GIS.
2. **Property A is not a recreational lake lot.** J.W. Smith Reservoir is a closed drinking-water
   supply: no gas motors, boats ≤20 ft, **no swimming**, access only at the entrance gate,
   Sat–Wed for eight months a year, and **no private dock programme**. The lot does not touch the
   water — CCWA owns a measured **≈33-ft strip** in front of it.
3. **Property B's "DOCKABLE" claim is unsubstantiated.** The structured MLS field says
   "Lake Privileges"; sibling listings name the dockable lots and 130/131 are not among them;
   dockable lots on the same street ask **$136k–$143k each** against $55,000 for this pair.
   61–62% of Thurmond shoreline is Protected Shoreline where no new private structures are
   authorised. **Only USACE can resolve it: 1-800-533-3478.**
4. **Property A's slope is materially steeper than advertised.** Against a listing describing a
   "perfect gentle rolling lot": **81.7 ft of relief**, in-lot average **18.4% (10.4°)**, maximum
   **25.6% (14.3°) over a 50-ft run** — and the steepest ground is inside the building area.
   Property B is genuinely gentle (3.7% in-lot) with its steep reach on federal land.
5. **Both soils are rated "Very limited" for septic.** Property B's Zion silt loam has
   **indurated bedrock at 30 inches** against a mandatory 24-inch separation, plus **7.5% linear
   extensibility** (high shrink–swell). A conventional 5-bedroom drainfield may not be permittable.
6. **Building a 5-bedroom home is value-destructive on both** — likely **$833,600** (A) and
   **$940,600** (B) against best comparables of $565,000 and $422,000.

## Supporting research

The `research/` directory holds the long-form source research behind the report, with every claim
labelled `[OFFICIAL]` / `[LISTING]` / `[ESTIMATE]` / `[UNVERIFIED]` and inline source URLs:

- [`research/property-A-waterpointe-clayton-county.md`](research/property-A-waterpointe-clayton-county.md)
  — zoning, reservoir rules, HOA, utilities, STR, hazards for Property A
- [`research/property-B-stillwater-coves-lincoln-county.md`](research/property-B-stillwater-coves-lincoln-county.md)
  — USACE shoreline management, covenants, utilities, lake facts for Property B
- [`research/two-property-comparison.md`](research/two-property-comparison.md)
  — climate, hazards, demographics, schools, healthcare, services, airports, construction cost

## Limitations

This is a **screening and decision-support document**: not a survey, appraisal, legal opinion,
engineering certification, floodplain determination or soil evaluation. Values marked
*GIS-derived* are model-based. **Property B's boundary is a reconstruction** — no plat or parcel
polygon is publicly obtainable for Lots 130/131.

**§58 of the report lists 27 documents and determinations that could not be obtained.** Four are
flagged as conditions of an offer rather than post-closing tasks; they are the real next steps.
