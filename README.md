# Land Due-Diligence Report — 12396 Edgewater Dr #23, Hampton, GA 30228

**Subject:** Vacant lakefront lot, Waterpointe subdivision, ±1.33 acres
**Prepared:** October 2026 · All research conducted against live primary sources
**Source labels:** `[OFFICIAL]` government/HOA/utility primary · `[LISTING]` MLS-derived · `[ESTIMATE]` model/derived · `[UNVERIFIED]` could not confirm

> 📊 **Companion report:** [`TWO-PROPERTY-COMPARISON.md`](TWO-PROPERTY-COMPARISON.md) — side-by-side
> due diligence of this lot against the **Stillwater Coves lots (1147 & 1153 Watersedge Cove, Lincoln
> County, GA)** on Clarks Hill Lake, covering climate, natural hazards, demographics, schools,
> healthcare, shopping, South Asian community access, recreation, walkability, airports, and a
> line-item **construction cost estimate for a 5-bedroom home on each lot**.

---

## 0. Executive summary — three premises in the request are wrong

Before anything else: **three of the assumptions in the research brief are factually incorrect**, and each one changes the answer to multiple downstream questions. All three are confirmed by multiple independent official sources.

| Brief assumed | Reality | Confidence |
|---|---|---|
| Henry County, Georgia | **Clayton County, Georgia** (FIPS 13063) | Confirmed ×4 |
| Henry County Water Authority (HCWA) reservoir | **Clayton County Water Authority (CCWA)** reservoir | Confirmed ×3 |
| Possibly inside City of Hampton limits | **Unincorporated** — no city jurisdiction at all | Confirmed ×3 |

**Why the confusion is understandable:** the mailing address is genuinely "Hampton, GA 30228," and Hampton is a Henry County city. But the lot sits in the **Clayton County "panhandle"** — a southern salient of Clayton County that reaches down toward Hampton. The USPS address and the governing jurisdiction do not match. This is also why the subdivision is accessed from **Panhandle Road**.

**The single most important discovery:** Clayton County's zoning ordinance contains a provision written **specifically and by name** for lots abutting this exact reservoir — **Sec. 4.5(D), "J.W. Smith Reservoir"** — imposing a 50,000 SF minimum lot area, a 400-foot minimum lot depth, a **permanent 150-foot protection buffer**, and an expectation that **sanitary sewer be installed**. Any analysis of this lot that misses Sec. 4.5(D) is unusable. Full text in §2.

**Net read on the lot:** it is a legitimately buildable, legally-created 1.33-acre lot that comfortably clears the two hardest numeric tests (≥50,000 SF area, ≥400 ft depth). The real constraints are (a) the 150-ft reservoir buffer consuming roughly a third of the lot depth, (b) a minimum heated-area requirement of 1,800–2,000 SF that rules out a small cabin, (c) genuine ambiguity about whether sewer or septic governs, and (d) the fact that **the lot does not touch the water** and the lake is a closed drinking-water reservoir with no private docks, no swimming, and no gas motors.

---

## 1. Parcel identification — the factual base

All values below are from the Clayton County Tax Assessor's live GIS parcel service unless noted.

| Field | Value |
|---|---|
| Parcel ID | **05050A A003** |
| Situs | 12396 Edgewater Dr, Hampton, GA 30228 |
| Legal | **Unit 3, Lot 23**, Waterpointe |
| Plat reference | **Plat Book 27, Page 24** |
| Current deed | **Deed Book 12617, Page 0653** (2021) |
| Last sale | **2021-08-31 — $85,000** |
| Owner of record | MCKNIGHT DESMOND (mailing: 3136 Elmwood Ct, Atlanta, GA 30349) |
| Zoning | **RS-180** (Single-Family Residential) |
| Taxing jurisdiction | `CVTTXDSCRP = COUNTY` — **unincorporated** |
| Area | **57,943 SF = 1.3302 acres** (GIS); 57,720 SF independently recomputed from polygon |
| Land use | Residential vacant |
| Appraised / assessed | $60,000 / $24,000 |
| FEMA floodplain flag | **NO** |
| Commission district | 3 |
| Assessor neighborhood | WATERPOINTE |

`[OFFICIAL]` Parcel query: [Clayton County TaxAssessor/Parcels MapServer](https://gis.claytoncountyga.gov/server/rest/services/TaxAssessor/Parcels/MapServer/0/query) · Property card: [publicaccess.claytoncountyga.gov — PIN 05050A A003](https://publicaccess.claytoncountyga.gov/Datalets/Datalet.aspx?mode=&UseSearch=no&pin=05050A%20A003)

### 1.1 Measured geometry (computed from the official parcel polygon)

I pulled the parcel polygon in WGS84 and measured it directly:

| Dimension | Measured |
|---|---|
| Street frontage (Edgewater Dr) | **≈ 147.5 ft** |
| East side line | ≈ 418.3 ft |
| West side line | ≈ 415.4 ft |
| Rear line (toward reservoir) | ≈ 129.8 ft (116.3 + 13.5 ft segments) |
| Perimeter (computed / GIS-reported) | 1,111.0 ft / 1,112.1 ft — agree to 0.1% |
| Effective lot depth | **≈ 415–418 ft** |
| Average width | ≈ 133 ft |

`[ESTIMATE]` — derived from `[OFFICIAL]` geometry. Local equirectangular projection; perimeter cross-check against the county's own reported value agrees within 1.1 ft, so these figures are reliable to roughly ±1%. **A boundary survey is still required for permitting** — parcel lines in GIS are explicitly disclaimed by the county as not a true representation of boundaries.

### 1.2 Jurisdiction — how it was confirmed four ways

1. `[OFFICIAL]` **US Census Bureau geocoder**, coordinate query at 33.416191, -84.369848 → `Counties: Clayton County`; **no "Incorporated Places" result returned at all** (= unincorporated). [Census Geocoder](https://geocoding.geo.census.gov/geocoder/geographies/coordinates?x=-84.369848&y=33.416191&benchmark=Public_AR_Current&vintage=Current_Current&format=json&layers=all)
2. `[OFFICIAL]` **Census geocoder, address query** for "12396 Edgewater Dr, Hampton, GA 30228" → matched, `Counties: Clayton County`, `STATE 13 / COUNTY 063`, Census Tract 406.36, Block 1000 (GEOID 130630406361000), **Clayton County School District**.
3. `[OFFICIAL]` **Clayton County's own tax parcel layer** contains this address with `ZONE = RS180` and `CVTTXDSCRP = COUNTY`. A Henry County parcel would not appear in Clayton's assessor database.
4. `[OFFICIAL]` **The HOA's own bylaws** place the subdivision "on Panhandle Road at Northbridge Road in the area of Land Lots 50, 51, 78 & 79 of the 5th District of **Clayton County, Georgia**," and state that in 1992 "the jurisdictional authority was transferred to Clayton County."

**City limits — definitively not in any city.** I queried Clayton County's municipal boundary layer for every incorporated place in the county. The complete list is **Lake City, Morrow, Riverdale, Lovejoy, College Park, Forest Park, and Jonesboro**. Hampton is not among them (Hampton is a Henry County city and cannot annex across the county line). The parcel intersects **none** of these boundaries. `[OFFICIAL]` [Reference/MunicipalAreas MapServer](https://gis.claytoncountyga.gov/server/rest/services/Reference/MunicipalAreas/MapServer/0/query)

> **Zoning authority = Clayton County Department of Community & Economic Development, Planning & Zoning.** Zoning Administrator: Tyler L. McSwain, 121 South McDonough St., Jonesboro, GA 30236, (770) 477-3569. `[OFFICIAL]` [Planning & Zoning](https://www.claytoncountyga.gov/government/community-economic-development/planning-zoning/)

The City of Hampton, Henry County government, and Henry County Water Authority have **no regulatory authority over this parcel**. Every Henry County/HCWA rule in the original brief is inapplicable — see §2.6 for what HCWA's analogous rules say, included only for contrast.

---

## 2. The reservoir: J.W. Smith Reservoir (CCWA)

### 2.1 Ownership, identity, and physical facts

`[OFFICIAL]` **J.W. Smith Reservoir is owned and operated by the Clayton County Water Authority.** CCWA's fishing page states plainly: "J.W. Smith Reservoir is a 250 acre CCWA-owned lake." [CCWA Fishing Information](https://www.ccwa.us/1285/Fishing-Information)

**It is not an HCWA reservoir.** HCWA's own reservoir page lists its complete five-reservoir network — Tussahaw (1,466 ac), Upper Towaliga (1,100 ac), Lower Towaliga (121 ac), Long Branch (277 ac), Indian Creek/Gardner (209 ac). **J.W. Smith is absent from that list.** `[OFFICIAL]` [HCWA Reservoirs](https://hcwa.com/resources_facilities/reservoirs.php)

| Attribute | Value | Source |
|---|---|---|
| Owner | Clayton County Water Authority | `[OFFICIAL]` CCWA |
| Surface area | **250 acres** | `[OFFICIAL]` CCWA; corroborated by NID at 250.0 ac |
| Impounded stream | **Shoal Creek** | `[OFFICIAL]` National Inventory of Dams, GA03893 |
| Year built | **1984** | `[OFFICIAL]` NID GA03893 |
| Dam type / height / length | Earth / 42.5 ft / 1,400 ft | `[OFFICIAL]` NID GA03893 |
| Normal storage / max storage | 2,650 AF / 4,090 AF | `[OFFICIAL]` NID GA03893 |
| Hazard class / condition | **High hazard** / Satisfactory (insp. Jan 2016) | `[OFFICIAL]` NID GA03893 |
| Designer | Robert & Company | `[OFFICIAL]` NID GA03893 |
| Primary purpose | Water supply | `[OFFICIAL]` NID GA03893 |
| Regulator | Georgia Safe Dams Program | `[OFFICIAL]` NID GA03893 |
| Normal pool elevation | ≈ 247 ft (northern lobe) / ≈ 241 ft (southern lobe) | `[OFFICIAL]` Clayton County hydrography layer |

NID data via [Snoflo mirror of USACE National Inventory of Dams, GA03893](https://snoflo.org/reservoir/georgia/ga03893-j-w-smith-reservoir-dam) — note this page's prose erroneously says "Fayetteville" in one sentence and "Clayton County" in another; the **tabular NID fields** are the reliable part and are what I have used.

**Depth:** no surveyed bathymetry exists. `[ESTIMATE]` Derived maximum depth is bounded by the dam height of 42.5 ft; realistic maximum pool depth near the dam is on the order of 30–40 ft, shallowing substantially in the arms. No national bathymetric survey exists for US reservoirs, so **treat any specific depth figure as unverified**.

**A naming quirk worth knowing.** In the National Hydrography Dataset and in Clayton County's basemap, the lake is mapped as **two polygons** split by the North Bridge Road crossing:

- Northern lobe — GNIS name **"Club Lake"** (GNIS ID 00312768), 134.5 acres, elev. 247 ft — *this is the lobe the subject lot fronts*
- Southern lobe — unnamed, 114.4 acres, elev. 241 ft

134.5 + 114.4 = **248.9 acres ≈ CCWA's stated 250 acres.** I confirmed both polygons fall inside the single CCWA ownership parcel, so they are two mapped lobes of one reservoir. If a title search or survey refers to "Club Lake," that is the same water body as J.W. Smith Reservoir. `[OFFICIAL]` [Clayton Basemap Waterbodies layer](https://gis.claytoncountyga.gov/server/rest/services/Basemap/Clayton_Basemap_WebmapBuilder/MapServer/11/query)

### 2.2 Who owns the bed, the shoreline, and the strip in front of the lot

`[OFFICIAL]` **CCWA owns the reservoir bed, the shoreline, and a strip of upland between the lot and the water.**

The adjoining tract is **Parcel 05045 051001**:

| Field | Value |
|---|---|
| Owner | **CLAYTON COUNTY WATER AUTHORITY** |
| Situs | 275 Hampton Rd, Hampton, GA 30228 |
| Mailing | 1600 Battlecreek Rd, Morrow, GA 30260 (CCWA HQ) |
| Area | **336.09 acres** |
| Zoning | **AG** (Agricultural) |
| Acquired | **1974** — Deed Book 0748, Page 115 |
| Land use | Improved Government Owned Exempt |
| Appraised | $5,480,100 |

I verified by spatial query that the **centroids of both reservoir lobes fall inside this CCWA parcel** — so the water itself is CCWA-owned land, acquired a decade before the dam was completed.

**Measured gap between the lot and the water.** Using the official parcel polygon and the official waterbody polygon, the minimum distance from the subject lot's boundary to the water's edge is **≈ 33 feet**. `[ESTIMATE]` (derived from `[OFFICIAL]` geometry)

Adjacency testing confirms the relationship: a spatial query at 0 ft returns no CCWA parcel, while 10 ft and beyond returns parcel 05045 051001. That sub-10-ft discrepancy is ordinary GIS digitizing slop between two separately-mapped boundaries — in practice **the lot's rear line abuts CCWA land**, and CCWA land then continues roughly 33 more feet to the waterline.

> **Practical consequence:** this lot is "lakefront" in the sense of *abutting the reservoir property and having water views*, **not** in the sense of owning frontage on the water. There is CCWA fee-owned land between the rear lot line and the lake. You cannot walk from your deeded land into the water without crossing CCWA property. This is the single most commonly misunderstood fact about these lots.

### 2.3 Is there an HCWA-style buffer strip? Yes — a CCWA one, and it is bigger than the land strip

The ±33 ft of CCWA upland is **not** the regulatory buffer. The regulatory buffer is **150 feet and it extends onto the private lot.** See §2.4 — this is the central finding of the report.

### 2.4 ⭐ Clayton County Zoning Sec. 4.5(D) — written specifically for this reservoir

This is the controlling local provision and it names the reservoir explicitly.

`[OFFICIAL]` **Clayton County Code, Appendix A — Zoning, Article 4 (Special Districts), Sec. 4.5(D):**

> **"D. J.W. Smith Reservoir:** In addition to the above, all lots abutting the J.W. Smith Reservoir property must also comply with the following restrictions:
> 1. All such lots are to be at least **50,000 square feet** in area.
> 2. Such lots are generally to have a **minimum depth of at least 400 feet**. However, up to ten percent of such lots may vary from this standard; provided that compliance with the standard would pose a unique hardship due to the configuration of the reservoir property; and the average depth of nearly all such lots is 400 feet or greater.
> 3. All such lots shall have a **permanent 150-feet protection buffer adjoining the reservoir property**. **No septic tanks, septic tank absorption field, related structure or feature, substantial structure, or other feature which may adversely impact the reservoir may occupy any portion of this 150 feet buffer.** Additionally, it is preferable that this area be a natural vegetated buffer.
> 4. **Access to the J.W. Smith Reservoir to conform to the Clayton County Water Authority policies.**
> 5. **Sanitary sewer to be installed unless EPD indicates such sewer should not be installed.**"

Source: [Municode — Clayton County Code, Appendix A, Art. 4, Sec. 4.5](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART4SPDI_S4.5SURE) (code current through Sep 10, 2026)

**How the subject lot measures against Sec. 4.5(D):**

| Requirement | Required | Subject lot | Result |
|---|---|---|---|
| Minimum lot area | ≥ 50,000 SF | **57,943 SF** | ✅ Passes, with ~7,900 SF margin |
| Minimum lot depth | ≥ 400 ft | **≈ 415–418 ft** | ✅ Passes |
| 150-ft protection buffer | Permanent, no septic/substantial structure | ≈ 36% of lot depth | ⚠️ Material constraint — quantified below |
| Reservoir access | Per CCWA policy | See §2.5 | ⚠️ CCWA policy is restrictive |
| Sanitary sewer | To be installed unless EPD says otherwise | Availability unconfirmed | ⚠️ **Must verify with CCWA** |

**Quantifying the 150-ft buffer.** The ordinance text is internally inconsistent about the measurement datum (see §11, Contradiction C1):

- Sec. 4.5(D)(3) says *"adjoining the reservoir property"* → measured from the CCWA property line = the rear lot line
- Sec. 4.6(E) says *"adjoining the reservoir property **from the normal full-pool elevation**"* → measured from the waterline, ~33 ft further back

`[ESTIMATE]` Using the lot's measured ~130 ft rear width and ~417 ft depth:

| Datum | Buffer depth onto lot | Approx. lot area in buffer | Approx. remaining |
|---|---|---|---|
| From rear lot line (conservative) | 150 ft | ≈ 20,000 SF | ≈ 37,900 SF |
| From normal full pool (~33 ft out) | ≈ 117 ft | ≈ 15,600 SF | ≈ 42,300 SF |

**Resulting building envelope (conservative reading):**
417 ft depth − 150 ft rear buffer − 30 ft front setback = **≈ 237 ft of usable depth**, by roughly 128–148 ft of width net of the 10-ft side setbacks. That is a generous envelope for a large house. **The buffer is a real but manageable constraint** — it does not render the lot unbuildable, and the lot retains well above the 25,000 SF of usable area that septic would require (see §5.3).

Note Sec. 4.6(E)'s conflict rule: *"In cases when the requirements of this section conflict with the requirements within itself or any other lawfully adopted rules, regulations, resolutions, deed restrictions or covenants, **the more restrictive or that imposing higher standards shall govern**."* So assume the 150 ft is measured from the rear lot line until the county says otherwise in writing.

### 2.5 Recreation: boating, fishing, docks, swimming — what CCWA actually allows

`[OFFICIAL]` CCWA publishes a two-page **"Recreation Areas — Schedule and Fees / Rules & Regulations"** document. I extracted the full rule set. [CCWA Recreation Area Regulations (PDF)](https://www.ccwa.us/DocumentCenter/View/506)

**Is J.W. Smith open to the public? Yes — this one actually is.** CCWA operates five raw-water reservoirs, **three of which are open for public recreation**: Shamrock, Blalock, and J.W. Smith (plus limited Shoal Creek access). This is a meaningful difference from the HCWA assumption in the brief — the lake *is* open, on a published schedule.

**Season and hours** `[OFFICIAL]`
- Season: **March 1 – October 31**
- J.W. Smith is **open Saturday through Wednesday; closed Thursdays and Fridays**
- March: 7 am–7 pm · April–September: 7 am–8 pm · October: 7 am–7 pm
- Permitted activities: **fishing, picnicking, and canoeing**
- Off-season (Nov–Feb): the J.W. Smith Park Area may be reserved for group use — $50 for ≤25 people, or $2/person above 25

**Fees** `[OFFICIAL]` Season pass $30 (Clayton residents) / $40 (non-residents); daily $5 per vehicle (residents) / $10 (non-residents). Cash and checks only, sold at the reservoir entrance office. Buses/vans over 10 passengers cost extra.

**Key rules bearing directly on a lakefront owner:**

| # | Rule (CCWA Rules & Regulations) | Impact on this lot |
|---|---|---|
| 2 | **Max boat length 20 feet. Electric motors or paddles only. "Gas motor usage is prohibited under any circumstances."** | No powerboat, no ski boat, no pontoon with an outboard |
| 5 | **"Access to the reservoir shall be made only at the entrance gate."** | ⭐ **You may not launch or enter the water from your own back yard** |
| 6 | Bank fishing only within "marked" boundaries | No fishing from your own shoreline frontage |
| 7 | Limit of two poles per person | — |
| 8 | **"Wading, swimming, or bathing is prohibited."** | ⭐ **No swimming — body contact banned** |
| 16 | Once boaters cast off, they must stay in boats except emergencies | No beaching/landing along the shore |
| 1 | No alcoholic beverages of any kind | — |
| 13 | No firearms, bows, projectile devices, fireworks, explosives | — |
| 17 | Pets welcome but must be restrained (leash law enforced) | — |
| 19 | Open fires prohibited | No lakeside fire pit on CCWA land |
| 3 | Must comply with GA DNR fishing regulations; fishing license required age 16+ | State license needed *in addition* to CCWA pass |

Enforcement: first offense = 7 days expulsion; second = expulsion for the entire season. Max group size 100.

**Private docks: NOT PERMITTED.** This is a firm conclusion drawn from three converging facts:
1. CCWA owns the bed, the shoreline, and the upland strip (§2.2) — a private owner has no riparian interest to build from.
2. Clayton County Zoning Sec. 4.5(D)(3) bars any "**substantial structure, or other feature which may adversely impact the reservoir**" within the 150-ft buffer — which encompasses the entire shoreline area.
3. CCWA Rule 5 confines all reservoir access to the entrance gate, and Sec. 4.5(D)(4) subordinates all access to CCWA policy.

Nothing in any CCWA published document authorizes private docks, and **no dock permit program appears to exist**. `[OFFICIAL]` for the three underlying rules; the synthesis is my conclusion — **get it in writing from CCWA before paying any premium for "dock potential."**

**Body contact / swimming: prohibited** (CCWA Rule 8), consistent with standard practice on raw drinking-water reservoirs. `[OFFICIAL]`

**Note on listing language.** At least one MLS listing for a neighboring Waterpointe lot advertises *"private access to lake."* `[LISTING]` [Redfin — 12122 Edgewater Dr #15](https://www.redfin.com/GA/Hampton/12122-Edgewater-Dr-30228/unit-15/home/92213906) **This is contradicted by CCWA's published Rule 5.** See §11, Contradiction C2.

### 2.6 For contrast only — the HCWA rules from the brief

The brief asked specifically about the HCWA buffer guidance document. I retrieved it. **It does not govern this parcel**, but it is a useful analogue because HCWA and CCWA face the same state rule, and it shows what a formal adjoining-owner buffer program looks like.

`[OFFICIAL]` [HCWA Buffer Area Access Permit Rules and Regulations, eff. April 11, 2019 (PDF)](https://cms3.revize.com/revize/henrycountywaterauthority/Documents/Development/WaterShed%20Protection/Buffer_Permit_Guidance_Doc_050820%20(002)(1).pdf)

- HCWA Ordinance 2019-02 (orig. 1998, modified 2019); Henry County Watershed Protection Ordinance **2004-64**
- Buffer Area = HCWA-owned property adjacent to full pool, **"typically one hundred fifty (150) feet from the normal pool level"** — the same 150-ft figure
- Adjoining owners may obtain a **Buffer Area (Work) Permit or (Access) Permit** to clear underbrush, trim trees, and access the reservoir — explicitly **"by privilege, not right"**; renewed annually; $45, or $25 for seniors 62+/disabled/military
- Prohibited in the buffer: **bodily contact including wading, swimming, bathing**; construction of structures not on the permit; storing watercraft in the buffer; alcohol/drugs; burning; motorized vehicles; fish baskets, seines, set hooks, trotlines
- Violations: fines up to **$1,000 per violation per day** plus restoration costs; non-permitted users are trespassers
- **Docks: the HCWA document never mentions docks at all** — and HCWA's own FAQ states: *"can I launch a watercraft from my property? **No**, for safety and security reasons, all watercraft must be launched at a designated public boat ramp"*

So both authorities converge on: 150-ft buffer, no body contact, no launching from private property, no private docks. **The regime is materially the same even though the brief named the wrong authority.**

---

## 3. Watershed protection and buffer rules

### 3.1 Georgia EPD / DNR Rule 391-3-16-.01 — the state floor

`[OFFICIAL]` Full rule text: [Ga. Comp. R. & Regs. 391-3-16-.01, Criteria for Water Supply Watersheds](https://rules.sos.ga.gov/gac/391-3-16-.01) · readable mirror: [Cornell LII](https://www.law.cornell.edu/regulations/georgia/Ga-Comp-R-Regs-R-391-3-16-.01)

**Definitions that matter** (Rule 391-3-16-.01(2)):
- *"Reservoir Boundary"* = **"the edge of a water supply reservoir defined by its normal pool level."**
- *"Water Supply Reservoir"* = a **governmentally owned** impoundment whose primary purpose is supplying government-owned public drinking water systems (excludes USACE multipurpose reservoirs). J.W. Smith qualifies.
- *"Small water supply watershed"* = **less than 100 square miles** of land upstream of the intake. Clayton County has **three small and two large** drinking water supply watersheds (per county ordinance Sec. 4.1); J.W. Smith is treated as a **small** watershed in the county's ordinance structure.

**§(7) — Minimum criteria for SMALL water supply watersheds** (this is what the brief asked for):

*Perennial stream corridors **within** a 7-mile radius upstream of a government-owned intake or water supply reservoir:*
| Control | Requirement |
|---|---|
| Buffer | **100 ft** on both sides, measured from stream banks |
| Impervious setback | **No impervious surface within 150 ft** on both sides from stream banks |
| Septic | **Septic tanks and drainfields prohibited** in that 150-ft setback |

*Perennial stream corridors **outside** the 7-mile radius:*
| Control | Requirement |
|---|---|
| Buffer | **50 ft** both sides from stream banks |
| Impervious setback | **No impervious surface within 75 ft** |
| Septic | **Prohibited** in that 75-ft setback |

*Applying at **all** locations in a small water supply watershed:*
- New sanitary landfills only with synthetic liners + leachate collection
- New hazardous waste treatment/disposal facilities **prohibited**
- **Impervious surface of the entire watershed limited to 25%**, or existing use, whichever is greater — ⚠️ **this is a watershed-wide cap, NOT a per-lot cap.** It does not limit an individual homeowner. The per-lot limit comes from zoning (35%, see §4.2). This distinction is frequently misreported.
- New facilities handling DNR-specified hazardous materials must operate on impermeable surfaces with spill/leak collection

**§(8) — Water Supply Reservoir Management Plans — the source of the 150 ft:**

> "(a) The owner of a water supply reservoir shall develop a reservoir management plan for approval of the Department of Natural Resources…
> (b)(1) Any recreational uses shall take into consideration the protection of the water quality of the reservoir for drinking water purposes. The following recreational uses **are permissible in the reservoir management plan if the water quality of the reservoir is adequately protected**: (i) Swimming; (ii) Fishing; (iii) Boating; (iv) **Docks**; (v) Public Access; and (vi) **Adjacent Property Owner Access**.
> (b)(2) The reservoir management plan shall include a **buffer that shall be maintained for a distance of 150 feet from the reservoir boundary**. The allowable buffer vegetation and disturbance shall be specified in the reservoir management plan. Allowable disturbances may include public and/or private access to the reservoir and/or the buffer via **docks, trails, and similar amenities** provided that such disturbances are addressed in the reservoir management plan.
> (b)(3) Reservoir owners may adopt buffers of differing sizes than in 2. above upon approval of the Department of Natural Resources."

> **Read this carefully, because it is the crux of the dock question.** The state rule makes swimming, boating, docks, and adjacent-property-owner access *permissible* — but **only if CCWA's DNR-approved reservoir management plan provides for them.** CCWA's published recreation rules do the opposite: they ban swimming and wading, ban gas motors, cap boats at 20 ft, and confine access to the entrance gate. So the state rule permits docks *in principle*, and **CCWA has elected not to allow them.** The operative document is CCWA's reservoir management plan, which is **not published online** — request it directly (see §12).

**§(10)** permits a certified local government to adopt alternate stream-buffer criteria, but expressly notes: **"These options do not affect the buffer around the water supply reservoir."** The 150-ft reservoir buffer is therefore not something Clayton County could have reduced through the alternate-criteria route.

### 3.2 Clayton County Watershed Protection District (WSP) — Zoning Article 4

`[OFFICIAL]` **Sec. 4.1 — Purpose:** "Clayton County has three small drinking water supply watersheds and two large drinking water supply watersheds. Uses permitted in this district are closely regulated to protect surface and underground water resources… Provisions of this district shall apply to all land lying within the boundary of the applicable watershed." [Municode Sec. 4.1](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART4SPDI_S4.1WAPRDIWSUR)

**Sec. 4.5(A) — Supplemental requirements, all locations in a small watershed:**
1. New sanitary landfills only with synthetic liners and leachate collection
2. New hazardous waste treatment/disposal facilities prohibited
3. Hazardous-materials facilities on impermeable surfaces with spill/leak collection
4. ⭐ **"All developments within the small drinking water supply watershed must comply with the Clayton County Water Authority Guidelines."**

**Sec. 4.5(B) — Perennial stream corridors within 7 miles of the intake:** 100-ft buffer each side; **impervious prohibited within 150 ft**; **septic prohibited within 150 ft**. (Mirrors state Rule 391-3-16-.01(7)(b)(1).)

**Sec. 4.5(C) — Perennial stream corridors beyond 7 miles:** 50-ft buffer; impervious prohibited within 75 ft; septic prohibited within 75 ft.

**Sec. 4.5(D) — J.W. Smith Reservoir:** quoted in full in §2.4 above.

**Sec. 4.6 — Buffer Requirements** [Municode Sec. 4.6](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART4SPDI_S4.6BURE)

- **(A) Buffer composition:** buffers "are to provide protection to the County's drinking water source and therefore, **are intended to be left in their natural undisturbed state.**"
- **(B) County variance** — requires the Zoning Administrator or Director of Transportation & Development to find **all six** of: (1) extraordinary/exceptional conditions of size, shape or topography; (2) unnecessary hardship from literal application; (3) the circumstances are **not the result of the applicant's own acts**; (4) not a request for an otherwise impermissible use; (5) **no increase in impervious surface beyond what the ordinance prescribes** (water supply watersheds specifically); and (6) no substantial detriment to water quality or the ordinance's intent.
- **(C) State variance:** "Any encroachment into the twenty-five (25) feet undisturbed State Water Buffer will require a buffer variance from the Georgia Environmental Protection Department."
- **(D) Conditions:** alternative mitigation measures may be imposed as a variance condition.
- **(E) Miscellaneous:** the 150-ft buffer language (quoted §2.4), plus the conflict rule — **the more restrictive standard governs.**

### 3.3 Clayton County Stream Buffer Protection Ordinance — Chapter 38, Article VIII

`[OFFICIAL]` Ord. No. 2005-34 § 2 (3-15-05); amended by Ord. 2005-87 and Ord. 2015-86. Sec. 38-140 et seq. [Municode Ch. 38 Art. VIII](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_CH38EN_ARTVIIICLCOSTBUPROR)

**Sec. 38-144.1 — Buffer and setback requirements:**
> "(a) An undisturbed natural vegetative buffer shall be maintained for **50 feet**, measured horizontally, on both banks (as applicable) of the stream as measured from the top of the stream bank.
> (b) An additional setback shall be maintained for **25 feet** … beyond the undisturbed natural vegetative buffer, **in which all impervious cover shall be prohibited.** Grading, filling and earthmoving shall be minimized within the setback.
> (c) **No septic tanks or septic tank drain fields shall be permitted within the buffer or setback.**"

→ **50 ft undisturbed + 25 ft no-impervious = 75 ft total from any stream bank.**

**Important scope limit.** "Stream" is defined (Sec. 38-142) as a stream beginning at a spring/seep/groundwater outflow sustaining streamflow, or at a point with a **drainage area of 25 acres or more**, or where field studies verify a stream. **The definition does not include lakes, reservoirs, or impoundments** — "impoundment" appears only in the definition of *"riparian."* So this ordinance governs any stream on or adjacent to the lot, **not the reservoir shoreline**; the reservoir is governed by Sec. 4.5(D)/4.6(E).

**Sec. 38-143 — Applicability** adds the important savings clause: these requirements "are in addition to, and do not replace or supercede, any other applicable buffer requirements established under state law."

**Sec. 38-144.2 — Variance procedures:** for a parcel **platted before the ordinance's effective date** whose shape/topography/physical condition prevents compliant development, and where the county finds the ordinance prohibits otherwise lawful use, the **Board of Commissioners may grant a variance, conditioned on mitigation**. Requires a public hearing, newspaper notice, and a posted sign visible from the adjacent road. ⭐ **The subject lot was platted in 1988 (Plat Bk 27 Pg 24) — it would qualify for consideration under this provision** if a stream buffer proves to be an obstacle.

### 3.4 Is a buffer work permit needed?

`[UNVERIFIED]` **Clayton County / CCWA do not publish an adjoining-property-owner "buffer work permit" program** equivalent to HCWA's. I searched CCWA's full sitemap (294 URLs) and the county code; no such permit form or program appears. Given that Sec. 4.6(A) requires the buffer be "left in their natural undisturbed state" and Sec. 4.5(D)(4) subordinates reservoir access to CCWA policy, the working assumption must be that **vegetation removal in the 150-ft buffer requires county and/or CCWA authorization, and a county buffer variance under Sec. 4.6(B) for anything more than trivial.** Confirm with both agencies — this is on the call list in §12.

### 3.5 Summary of every buffer that could touch this lot

| Buffer / setback | Width | Measured from | Authority | Applies here? |
|---|---|---|---|---|
| **Reservoir protection buffer** | **150 ft** | CCWA property line *or* normal full pool (ambiguous) | Clayton Zoning Sec. 4.5(D)(3), 4.6(E); state Rule 391-3-16-.01(8)(b)(2) | ✅ **Yes — the governing constraint** |
| State waters buffer | 25 ft | Point of wrested vegetation | O.C.G.A. 12-7-6(b); EPD variance required to encroach | ✅ Yes, nested inside the 150 ft |
| Stream buffer (undisturbed) | 50 ft | Top of stream bank | Clayton Sec. 38-144.1(a) | Only if a qualifying stream is on/near the lot |
| Stream impervious setback | +25 ft (75 ft total) | Top of stream bank | Clayton Sec. 38-144.1(b) | Same |
| Perennial stream, ≤7 mi of intake | 100 ft buffer / 150 ft impervious + septic | Stream bank | Clayton Sec. 4.5(B); state 391-3-16-.01(7) | Same |
| Septic: lot-size exclusion zone | 50 ft | Lake/river/stream/wetland | Clayton Zoning Sec. 6.6(B) | ✅ Yes — see §5.3 |
| Septic drainfield separation | 50 ft | Normal water level of impoundment | GA Rule 511-3-1 | ✅ Yes |
| Septic tank separation | 25 ft | Lakes/ponds/impoundments | GA Rule 511-3-1 | ✅ Yes |
| Rear yard setback | 25 ft | Rear property line | Clayton Zoning Sec. 3.6 | ✅ Yes (subsumed by the 150 ft) |

**Governing constraint: the 150-ft reservoir buffer.** Everything else is either nested inside it or stream-specific.

---

## 4. Zoning — RS-180 Single-Family Residential (Clayton County)

Authority: **Code of Clayton County, Georgia, Appendix A — Zoning** (code current through **Sep 10, 2026**). Note the brief's guess of "R-2 / RS" was close in spirit — the district is **RS-180**.

### 4.1 Confirmation of district

`[OFFICIAL]` Clayton County's zoning GIS returns `ZONE = RS180` for parcel 05050A A003, and every one of the 72 Edgewater Drive parcels queried is RS-180. [PlanningZoning/PEZ_CurrentZoning MapServer](https://gis.claytoncountyga.gov/server/rest/services/PlanningZoning/PEZ_CurrentZoning/MapServer/0/query) · Interactive: [Find My Zoning](https://cccd-gis.maps.arcgis.com/apps/webappviewer/index.html?id=20bb677504f64402b7fe67c67eb15986) · [Zoning Map](https://experience.arcgis.com/experience/c76a914336c94479b6135810eaa37259)

> The county's own disclaimer: *"Contact 770-288-7526 to verify zoning"* — and a **Zoning Verification Letter** costs **$100 per parcel**. For a purchase decision, buy the letter.

### 4.2 Sec. 3.6 — RS-180 District Standards (verbatim from the ordinance)

`[OFFICIAL]` [Municode Sec. 3.6](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART3ZODIINUSST_S3.6RSREDIST) — the standards are published as a graphic table; I retrieved and read the official image asset.

| Standard | RS-180 requirement | Subject lot | Status |
|---|---|---|---|
| **Minimum lot area** | **18,000 SF** | 57,943 SF | ✅ 3.2× the minimum |
| **Minimum lot width** | **120 ft** | ≈147.5 ft frontage | ✅ Passes |
| **Maximum lot depth** | **2.5 × lot width** | ≈417 ft vs. 369 ft max | ❌ **Exceeds** — see §11 C3 |
| **Minimum lot frontage** | 100% of lot width on a public street, with access from that street | Edgewater Dr | ✅ Presumed — verify Edgewater is public |
| **Sewer and water** | "Connection to public water and sewer is **preferred**" | TBD | ⚠️ See §5 |
| **Min. front yard setback** | 50 ft (Arterial) / 35 ft (Collector) / **30 ft (Local Road)** | Edgewater = local | 30 ft applies |
| **Min. side yard setback** | **10 ft each side, 20 ft total** | — | — |
| **Min. rear yard setback** | **25 ft** | — | Subsumed by 150-ft buffer |
| **Maximum lot coverage** | **35% of lot area** — "square footage of all primary and accessory structures, **and impervious surface**" | 35% × 57,943 = **20,280 SF** | ✅ Generous |
| **Minimum living area** | **2,000 SF heated for 2-story** (primary dwelling)<br>**1,800 SF heated for 1-story** (primary dwelling)<br>**800 SF** (accessory use dwelling) | — | ⚠️ **Rules out a small cabin** |
| **Maximum structure height** | **35 ft primary / 25 ft accessory**; all agriculture-related structures exempt; telecom per Article 6 | — | — |

**Two things to flag on this table:**

1. **Max lot coverage of 35% counts impervious surface, not just buildings.** House footprint + driveway + patio + pool decking + walkways all count against 20,280 SF. On a 1.33-acre lot that is still roomy, but a long driveway to a deep building pad consumes more of it than people expect.

2. **The minimum living area is a genuine constraint.** You must build at least **1,800 SF heated (single-story)** or **2,000 SF heated (two-story)**. A modest lake cottage is not permitted in RS-180.

**Additional development standards cross-referenced by Sec. 3.6:** Lot/Yard (LY), Height (HT), **Septic Tank (ST)**, Accessory Use/Structure (AS), Architectural (AA), Home Occupations (HO), Day Care, Personal Care Home, Places of Worship, Public/Private School, Performance, Sight Visibility, Public Improvement, Fence and Wall, Parking, Loading, Landscaping, Buffer Yard, Outdoor Lighting, Telecommunication, Sign. All in Article 6.

### 4.3 Permitted and conditional uses in RS-180

`[OFFICIAL]` From the Article 3 use matrices (P = Permitted, C = Conditional, N = Not permitted):

| Use | RS-180 | Standards ref |
|---|---|---|
| Dwelling, single-family | **P** | — |
| **Dwelling, single-family (accessory as an additional dwelling)** | **C** | Sec. 6.9 AS-05 |
| Home occupation Type I | **P** | Sec. 6.10 |
| Home occupation Type II | **P** | Sec. 6.10 |
| **Keeping of chickens** | **P** | **Sec. 6.42** |
| Keeping of livestock | **N** | — |
| Family day care home | **P** | — |
| Boarding/group/personal care home, ≤3 persons | P | Sec. 6.12 |
| Boarding/group/personal care home, ≥4 persons | C | Sec. 6.12 |
| Swimming pools and pool enclosures | P (accessory) | Sec. 6.9 AS-07 |
| Nature preserve and recreation trails | P | — |
| **Bed and breakfast facility** | **N** | — |
| Assisted living / nursing home | C | — |
| Wireless telecom facility/tower | C | Sec. 6.37 |
| Agricultural crop production | N | — |
| Kennels | N | Sec. 6.20 |

### 4.4 ⭐ Accessory dwelling units, second kitchens, in-law suites

**Yes — ADUs are allowed in RS-180, as a conditional use.** This is one of the more favorable findings in the report.

`[OFFICIAL]` **Sec. 6.9, AS-05 — Accessory Dwellings (Garage Quarters / Guest Houses / Caretaker Houses / Mother-In-Law Suites):**

> "Accessory dwellings are permitted as **conditional use** within the principle dwelling or as a free standing dwelling in the following zoning districts: **AG, ER, and RS-180.**
> **A.** Accessory dwellings shall include basement quarters, garage quarters, caretaker or other employee quarters, guest houses, mother-in-law suites, and other accessory dwellings as determined by the Zoning Administrator.
> **B. Accessory dwellings contained within a principle dwelling** shall comply with the following standards:
>  1. There shall be **no more than 1 accessory dwelling** in a principle dwelling unit.
>  2. The accessory dwelling **shall not have the only single access point being from a separate exterior entrance.**
>  3. **One additional parking space** shall be provided to serve the accessory dwelling.
>  4. The accessory dwelling shall comply with all building and health code standards.
> **C. Freestanding accessory dwellings** shall comply with the following standards:
>  1. There shall be **no more than 1 accessory dwelling per residential lot.**
>  2. The accessory dwelling **may be located in a second floor over a detached garage or may be a separate structure.**
>  3. The accessory dwelling **shall be located only within the rear yard.**
>  4. The accessory structures shall comply with the **minimum setbacks set forth within Article 3.**
>  5. The residential lot shall comply with the minimum lot area standards set forth within Article 3, **except that in no case shall an accessory dwelling be located on a lot having less than 12,000 square feet of lot area.**
>  6. **One additional parking space** shall be provided."

Source: [Municode Sec. 6.9](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART6DEST_S6.9ACUSSTST)

**What this means in practice for this lot:**
- An ADU is **permitted but requires a Conditional Use Permit** — public hearing before the Board of Commissioners, **$500 application fee**.
- **Minimum 800 SF** of living area for an accessory use dwelling (Sec. 3.6).
- Maximum **25 ft height** for accessory structures.
- Only **one** ADU per lot, either internal or freestanding — not both.
- A freestanding ADU must be in the **rear yard** — which collides directly with the **150-ft reservoir buffer** (Sec. 4.5(D)(3) bars "substantial structure" there). ⚠️ **The rear-yard requirement and the rear buffer squeeze the feasible location for a detached ADU.** An ADU inside the principal dwelling, or over an attached/detached garage positioned forward of the buffer, is the cleaner path.
- **Second kitchens:** not separately regulated. The operative constraint is AS-05(B)(2) — an internal accessory dwelling **may not have a separate exterior entrance as its only access**. A second kitchen with interior connection to the main house reads as an in-law suite rather than a separate unit. Confirm the Zoning Administrator's interpretation in writing, since AS-05(A) gives that office explicit discretion to classify.
- ⚠️ **Note the moratorium interaction:** Resolution 2026-153 freezes acceptance of **conditional use** applications related to boarding homes, group homes, personal care homes, short-term rentals, and community living arrangements through Dec 31, 2026. An ADU/in-law suite is not on that list, but it *is* a conditional use and the definitions are actively being rewritten — see §7.3 and §11 C5.

### 4.5 Accessory structures generally (Sec. 6.9, AS-02 — single-family districts)

`[OFFICIAL]` Permitted accessory structures include: antennas/satellite dishes >4 ft diameter; attached and detached decks and patios; gazebos; pools, hot tubs, saunas; detached garages and workshops; mini-barns, sheds, storage buildings; pole barns, horse barns, animal shelters and cages; and similar structures related to the primary use. Excluded from the definition: swing sets, mailboxes, lamp posts, doghouses, tree houses.

**Location rules (AS-01/AS-02(D)):**
1. No encroachment on any platted easement without written consent of the easement holder
2. ⭐ **No accessory structure in any operable or reserve septic field**
3. Minimum **10 ft separation** between a detached accessory structure and any other structure
4. Minimum **5 ft from side and rear property lines** (unless otherwise required)
5. **No accessory structure may be established before the primary structure exists** (AS-02(A))

Swimming pools (AS-07): minimum **10 ft from side and rear property lines.**

### 4.6 Nonconforming lot status — why the lot-depth issue is probably survivable

The lot was platted in **1988**. Appendix A **Article 9 — Nonconforming Structures, Lots, and Uses** governs legally-created lots that no longer meet current dimensional standards. `[OFFICIAL]` (article confirmed present in the code's structure)

`[ESTIMATE]` My read: a 1988 lot of record that satisfies both J.W. Smith-specific tests (≥50,000 SF, ≥400 ft depth) but technically exceeds RS-180's 2.5× max-depth ratio is almost certainly a **legal nonconforming lot of record** and buildable. But I did not retrieve Article 9's operative text, so **this needs confirmation** — it is question 1 on the call list.

### 4.7 Other overlay districts — one to check

Clayton County maintains several overlay districts in Article 4, including a **"Panhandle Area Overlay District" (Sec. 4.39–4.48)** with its own residential land use standards. Given that the HOA bylaws locate Waterpointe **"on Panhandle Road at Northbridge Road,"** this overlay may apply.

`[UNVERIFIED]` I could not confirm overlay membership: the county's `PEZ_OverlayAreas` map service **exposes no queryable layers** (returns "Layer not found"), and the parcel's `OVERLAY = WATERPOINTE` field is an assessor *neighborhood* code, not a zoning overlay. **Ask Planning & Zoning whether the Panhandle Area Overlay applies to parcel 05050A A003.**

---

## 5. Waterpointe HOA — Waterpointe Community Association, Inc.

### 5.1 Identity and structure

`[OFFICIAL]` Official site: [waterpointehoa.com](https://waterpointehoa.com/)

| Attribute | Finding |
|---|---|
| Legal name | **Waterpointe Community Association, Inc.** |
| Entity type | Georgia **nonprofit** corporation, organized under **O.C.G.A. § 14-3-1 et seq.** |
| Declarant | **Deer Glen Forest, Inc.** (or transferee/assignee) |
| Original construction | **1988** |
| Phases | **Four**, each with its own recorded Protective Covenants |
| Location (per bylaws) | "on **Panhandle Road at Northbridge Road** in the area of **Land Lots 50, 51, 78 & 79 of the 5th District of Clayton County, Georgia**" |
| Bylaws current version | **As Amended April 18, 2021** |
| Amenities | **Private swimming pool, tennis courts, clubhouse** |
| Management company | **None found** — self-managed by a volunteer Board of Directors |

The HOA describes itself as "One of **Clayton County's** finest family residential communities… bordering a **250 acre lake**" — independently corroborating both the county and the reservoir identity. `[OFFICIAL]`

### 5.2 ⭐ Membership is NOT mandatory — this is unusual and materially important

`[OFFICIAL]` **Bylaws, Article III(c) — Inactive Resident Members**, verbatim:

> "Even though all owners of lots in Waterpointe are entitled to membership in the Association, **such membership is not compulsory and owners shall not be required to maintain membership.** Any owner who does not desire to maintain active membership, or who otherwise fails to be current on all of his, or her, financial obligations to the Association, shall have the status of an Inactive Resident Member. **Inactive Resident Members shall have no right to use the Waterpointe Recreation Area or the facilities located thereon.**"

**Four membership classes** (Article III): Declarant Member (Deer Glen Forest, Inc.); Active Resident Members; Inactive Resident Members; Non-Resident Members.

> **Why this matters.** Most Georgia subdivision HOAs are mandatory, with dues secured by a lien running with the land. Waterpointe's is **voluntary for amenity access**. Non-payment converts you to Inactive status and forfeits pool/tennis/clubhouse rights — it does **not** create a perpetual personal assessment obligation going forward.
>
> **But the two things are separate, and this is the trap:** the **recorded Protective Covenants still run with the land and remain enforceable against every lot regardless of HOA membership status.** Declining membership gets you out of the dues and the amenities; it does **not** get you out of the architectural controls, use restrictions, or maintenance obligations. Plan accordingly.

**Reinstatement is not free.** An Inactive Member returning to Active status must pay "all unpaid financial obligations… which would have otherwise been payable… **during the three full calendar years immediately preceding**" the year active status is sought (Article III(c)). So lapsing and rejoining costs up to 3 years of back dues.

Also note Article VIII's anti-avoidance clause: a member who is Active when dues become due "cannot avoid payment by converting his Membership to Inactive Status," remains **personally liable**, and the Association may sue for the amount plus interest and reasonable attorney's fees.

### 5.3 Dues — and a cap that favors a vacant-lot buyer

`[OFFICIAL]` **Bylaws Article VIII — Membership Dues and Assessments**, as drafted (baseline from Jan 1, 1989):

| Class | Annual charge (dues + assessments combined) |
|---|---|
| Active Resident Member — house complete, C.O. issued by Clayton County as of Jan 1 | **$240.00** |
| **Active Resident Member — lot not built on / house not complete (no C.O. as of Jan 1)** | **$100.00** |
| Non-Resident Member | $240.00 |

- Payable **between January 1 and January 31** each year.
- Non-payment by Jan 31 → Active membership **automatically converts to Inactive**; a Non-Resident membership simply expires.
- After the Declarant ceased to be sole voting member, the Board sets the amount and payment date — **except**: ⭐ *"The Board of Directors shall **not**, however, have the authority to increase the dues and assessments which must be paid by an Active Resident Member who has not built upon his lot or whose house has not been completed."*

> **So the vacant-lot rate appears to be contractually capped at $100/year** while the lot remains unbuilt. That is a genuinely favorable holding-cost term for a land buyer. **Verify the current actual billed amount with the Board** — bylaws text and current practice can diverge.

**Fines:** the Board may impose "reasonable fines **not to exceed a total of Twenty-Five Dollars ($25.00) per day**" for violations of the bylaws or Rules and Regulations, collected by individual assessment, with **each day a separate offense**. The Board may also suspend recreational facility use for non-payment or violations. (Article VII)

**Conveyance protection:** no Association-owned real property may be conveyed, encumbered or hypothecated without written consent of **at least 75% of lot owners** — Active or Inactive (Article IX). This protects the pool/tennis/clubhouse parcels from being sold off by a board.

**Cross-check against listing data.** `[LISTING]` An aggregator reports Waterpointe HOA fees of **$13–$39/month** ($156–$468/yr). [HomesByMarco — Waterpointe](https://www.homesbymarco.com/subdivisions/waterpointe-in-hampton-ga) That bracket is broadly consistent with ~$240/yr for a built home, but it is MLS-derived and should not be relied on. The bylaws figure is the better anchor.

### 5.4 Recorded covenants — ⭐ the subject lot is governed by the Unit 3 declaration

The tax record identifies the lot as **Unit 3, Lot 23**, so the **Unit 3 Protective Covenants** are the operative declaration.

`[OFFICIAL]` **Recording references, per the HOA's own "About Us" page:**

| Phase | Recording |
|---|---|
| First two covenants | **Fulton County** records — Book **1446**, Pages 494–504; and Book **1553**, Pages 793–802 |
| After 1992 (Clayton County) | Book **1774**, Pages 680–694; and Book **09403**, Pages 318–331 |

The HOA states: *"In 1992, the jurisdictional authority was transferred to Clayton County and recorded in the appropriate property book."* `[OFFICIAL]` [waterpointehoa.com/about-us](https://waterpointehoa.com/about-us)

⚠️ **Flag:** the claim that the first two declarations were recorded in **Fulton County** is odd for a Clayton County subdivision and may be an error on the HOA's website. Have the title examiner verify all four chains — see §11 C4.

**Documents available for download** `[OFFICIAL]` from [waterpointehoa.com/newsletter/-documents](https://waterpointehoa.com/newsletter%2F-documents):
- `Protective_Covenents_Unit_1.pdf`
- `Waterpointe_covenents_Phase_2.pdf`
- **`Unit_3_Protective_Covenents.pdf`** ← **governs the subject lot**
- `Unit_4_Protective_Covenants.pdf`
- `Waterpointe By Laws As amended April 18, 2021.doc`
- `HOA Building Modification 2025.pdf` — architectural review form

⚠️ **I could not read the covenant content.** All four covenant PDFs are **scanned images with no text layer**, and no OCR engine was installable in this environment. The bylaws (a Word/RTF file) I could read in full, which is the source of §5.2–5.3. **The Unit 3 covenants must be read by you or your attorney** — they will contain the architectural controls, minimum square footage, exterior material requirements, setback covenants (which may be stricter than zoning), and any use restrictions including possible rental restrictions. This is a priority item.

**Architectural review:** an **Architectural/HOA Building Modification** process exists (2025 form on the site). Expect to need HOA approval for new construction in addition to county permits.

**Published rules from the HOA site** `[OFFICIAL]`: no visitor parking on grass or street except for special events (violations fined); exterior maintenance required (pressure washing, painting, gutters, mailbox); yards maintained (grass cut, weeds treated, shrubs/hedges trimmed, beds neat, no overhang into street).

### 5.5 Georgia Secretary of State corporate registry

`[UNVERIFIED]` **NOT RETRIEVED.** [ecorp.sos.ga.gov](https://ecorp.sos.ga.gov) is protected by a Cloudflare challenge that blocks automated access from this environment; the search returned only a "Just a moment…" interstitial. I could not confirm the entity's current registration status, control number, registered agent, or annual-registration standing.

**What I can say:** the bylaws self-describe the entity as "**Waterpointe Community Association, Inc., a non-profit Georgia Corporation**" organized under O.C.G.A. § 14-3-1 et seq. `[OFFICIAL]`

**Please check manually** at [ecorp.sos.ga.gov/BusinessSearch](https://ecorp.sos.ga.gov/BusinessSearch) searching "Waterpointe Community Association". Confirm the entity is **Active/Compliant** — an administratively dissolved HOA has impaired ability to enforce covenants or collect, which cuts both ways for a buyer.

---

## 6. Utilities

### 6.1 Water — CCWA

`[OFFICIAL]` **Clayton County Water Authority** is the water provider; it is also the reservoir owner. 1600 Battle Creek Road, Morrow, GA 30260 · **(770) 960-5200**

`[ESTIMATE]` Public water is almost certainly available on Edgewater Drive — the street is a built-out 1988 subdivision with numerous occupied homes, and RS-180 Sec. 3.6 states public water/sewer connection "is preferred." **Not independently confirmed at the street level.**

**2026 residential rates, effective with usage from January 1, 2026** `[OFFICIAL]` [CCWA New 2026 Rates](https://www.ccwa.us/1311/New-2026-Rates):

| Water — single family (conservation rates) | |
|---|---|
| Base rate | **$15.06/month** |
| 1–3,000 gal | $3.53 per 1,000 gal |
| 4,000–7,000 gal | $8.50 per 1,000 gal |
| 8,000–20,000 gal | $10.53 per 1,000 gal |
| Over 20,000 gal | $12.64 per 1,000 gal |

| Sewer — single family (conservation rates) | |
|---|---|
| Base rate | **$16.07/month** |
| 0–3,000 gal | $3.83 per 1,000 gal |
| Over 3,000 gal | $9.03 per 1,000 gal |

A typical 4,000 gal/month water + sewer customer saw a **$5.24/month increase** in the 2026 adjustment. A monthly **stormwater fee** is billed in addition to water and sewer.

**Connection / tap fees: NOT PUBLISHED.** `[UNVERIFIED]` CCWA does not post a tap/connection fee schedule. Its Engineering page states the Engineering Section "responds to customer inquiries about sewer or water availability and provides estimates for connecting to the CCWA system, **including connection fees, tap fees, meter costs and other charges**." Quotes are provided on request only.

→ **Call CCWA Engineering at (770) 960-5207** (or email via the page) for a written meter quote and connection-fee estimate for parcel 05050A A003. `[OFFICIAL]` [CCWA Engineering/Developer Information](https://www.ccwa.us/258/Engineering-Developer-Information)

Also relevant: **CCWA Standard Specifications (PDF)** and **CCWA Stormwater Development Guidelines (PDF)** are linked from that page, and Zoning Sec. 4.5(A)(4) requires all development in the small watershed to comply with **CCWA Guidelines**.

### 6.2 Sewer vs. septic — genuinely unresolved, and it matters

This is the most consequential open question in the report, and the evidence points in **both** directions.

**Pointing toward sewer:**
- ⭐ **Zoning Sec. 4.5(D)(5):** for lots abutting J.W. Smith Reservoir, *"**Sanitary sewer to be installed unless EPD indicates such sewer should not be installed.**"* `[OFFICIAL]`
- RS-180 Sec. 3.6: "Connection to public water and sewer **is preferred**." `[OFFICIAL]`
- CCWA operates **1,400 miles of sewer lines** and three water reclamation facilities. `[OFFICIAL]`
- Georgia Rule 511-3-1-.03(a): connection to public sewer **is mandatory** if available within **200 ft of the property line** or in an abutting right-of-way. `[OFFICIAL]`

**Pointing toward septic:**
- The zoning ordinance devotes an entire section (Sec. 6.6) to septic lot-size standards and explicitly contemplates septic within drinking water supply watersheds.
- Sec. 4.5(D)(3) bars septic within the 150-ft buffer — a rule that only has work to do if septic is contemplated on these lots.
- Large lots (1–2 acres) in a 1988 subdivision is a classic septic development pattern.

`[UNVERIFIED]` **I could not locate a CCWA sewer service area map or availability data for Edgewater Drive.** CCWA publishes no sewer availability map; its full sitemap contains no such resource.

→ **This is the #1 item to resolve.** Call CCWA Engineering, **(770) 960-5207**, and ask specifically: *is gravity sanitary sewer available in the Edgewater Drive right-of-way, within 200 feet of parcel 05050A A003?* The answer determines whether §6.3 applies at all, and it swings development cost substantially in either direction (sewer tap + possible main extension vs. septic design, soil work, and permitting).

### 6.3 Septic (if applicable) — requirements, setbacks, and bedroom count

**Permitting authority:** `[OFFICIAL]` **Clayton County Health District, Office of Environmental Services** — administers permits, inspections, and complaints for on-site sewage management systems. **(678) 610-7469**. [Clayton County Health District — Wastewater Management](https://www.claytoncountypublichealth.org/environmental-health/wastewater-management/)

> ⚠️ Beware when searching: **Clayton County, Iowa** (claytoncountyia.gov) dominates search results for "Clayton County septic." The Georgia agency is **claytoncountypublichealth.org**. Several otherwise-plausible search results are for the wrong state.

#### A. Local lot-size standards — Zoning Sec. 6.6, Septic Tank Standards (ST)

`[OFFICIAL]` [Municode Sec. 6.6](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART6DEST_S6.6SETASTST) — applies to **all districts**:

| Water source | Minimum lot size for septic |
|---|---|
| Non-public individual water supply (private well) | **43,560 SF (1 acre)** |
| **Public water supply system** | **25,000 SF of usable soil** |

> **(A)** Those minimums are "for the typical size home (**3 or 4 bedroom**) with basic appurtenances such as: driveway, minimum number of trees, and water supply line. **If larger homes, swimming pools, tennis courts or outbuildings, etc. are proposed** to be constructed or if trees would interfere with installation…, the Clayton County Board of Health **may require larger lots** to assure useable soil area or proposal may not be approved."
>
> **(B)** The following areas are **NOT counted** toward minimum lot size: road rights of way; private or public easements (power line, pipeline) that exclude installation; **"any area deemed undisturbed by any county or governmental office"**; flood control and management features (retention/detention ponds); any access portion less than 30 ft wide; soil conditions that exclude installation; **bodies of water**; and ⭐ **"land within 50 feet of a lake, river, stream, wetland or other bodies of water"** and similar limiting factors.
>
> **(C)** "**No single-family residence shall be permitted on a lot of less than 25,000 square feet of usable surface area to be served by septic tank(s), regardless of the zoning district classification.** With respect to existing platted lots, the Clayton County Board of Health will evaluate each individual request for a permit **on a case-by-case basis.** This restriction on lot size does not apply to residential development served by community sewer systems. Further, ⭐ **no septic tanks or drainfields will be permitted within a drinking water supply watershed buffer.**"
>
> **(D)** No physical development of the lot or installation of a system may begin without first obtaining a **construction permit from the County Health Department**.
>
> **(E)** "In instances where a larger lot is required by the district standard than this section, the larger requirement shall apply."

**Applying §6.6 to the subject lot** `[ESTIMATE]`:

| Step | Area |
|---|---|
| Gross lot area | 57,943 SF |
| Less 150-ft reservoir buffer ("deemed undisturbed" + express septic prohibition) | ≈ −20,000 SF |
| **Approx. remaining usable** | **≈ 37,900 SF** |
| Required (public water) | 25,000 SF |
| Required (private well) | 43,560 SF |

→ **With public water, septic appears feasible** with roughly 12,900 SF of margin before deducting road ROW and easements. **With a private well, it would likely fail.** Note the 50-ft-from-water exclusion is already subsumed within the 150-ft buffer deduction, so there is no double-count. **The Board of Health evaluates existing platted lots case-by-case (§6.6(C)) — a soil/site evaluation by a licensed soil classifier is the only way to settle this.**

#### B. State setbacks — Ga. Comp. R. & Regs. Chapter 511-3-1

`[OFFICIAL]` [Georgia DPH Chapter 511-3-1, On-Site Sewage Management Systems (PDF)](https://dph.georgia.gov/document/publication/envhealthonsiteruleschapter511-3-1jan2016pdf/download) · [Environmental Health Rules index](https://www.dph.georgia.gov/environmental-health/environmental-health-rules-and-regulations)

**Septic TANK minimum separations:**
| From | Distance |
|---|---|
| **Lakes, ponds, streams, water courses, and other impoundments** | **25 ft** |
| Geothermal boreholes | 25 ft |
| Pressure water supply lines | 10 ft |
| **Property line** | **10 ft** |
| Drainage ditch or embankment | 15 ft |
| Hardscape, drives, swimming pools, building foundations | 10 ft (recommended) |
| Wells/springs | Locate downgrade if physically possible |

**Absorption field (drainfield) minimum separations:**
| From | Distance |
|---|---|
| Existing or proposed wells, springs, **or sinkholes** | **100 ft** |
| **Normal water level of any impoundment, tributary, stream, or other body of water** (incl. ponded wetland areas) | **50 ft** |
| Geothermal boreholes | 50 ft |
| Water supply lines; buildings **with** basements | 10 ft |
| Buildings **without** basements, other structures, drives, hardscape, **property lines** | 5 ft |
| Embankment, pool foundation, drainage ditch, trash pits | 15 ft |

Also: minimum **24 inches of vertical separation** from the trench bottom to seasonal groundwater table, rock, or impervious layer — greater if groundwater contamination potential is indicated. Where a water supply line crosses or comes within 10 ft of the field, it must be installed at least 12 inches above. The County Board of Health may allow lesser or require greater distances based on topography, site configuration, subsurface soils, or groundwater interference.

#### C. ⭐ How bedroom count is determined, and how it sizes the system

`[OFFICIAL]` Rule 511-3-1:
- The permit application must state the **"Number of bedrooms in the dwelling,"** or the number of persons served for non-residential uses, or other sewage flow/water usage data. **Bedroom count is a declared design input on the permit application, verified against the submitted house plans** — it is not derived from square footage.
- **Tank capacity:** *"The liquid capacity of septic tanks for single family dwellings shall be **one thousand gallons for one, two, three or four bedrooms** and **250 additional gallons for each bedroom over four**."*
- **Capacity must be increased by 50% if a garbage grinder (disposal) is used.**
- **Two-compartment tanks are required**, with the first compartment at least 2/3 of liquid capacity.

| Bedrooms | Minimum tank |
|---|---|
| 1–4 | 1,000 gal |
| 5 | 1,250 gal |
| 6 | 1,500 gal |
| 7 | 1,750 gal |
| + garbage grinder | ×1.5 |

> **Practical note for this lot:** RS-180 requires ≥1,800–2,000 SF heated, and neighboring Waterpointe homes run 2,592–6,010 SF with 4–6 bedrooms `[LISTING]`. A 5–6 bedroom house on septic needs a 1,250–1,500 gal tank **and** triggers Sec. 6.6(A)'s "larger homes… may require larger lots" provision. Design the house and the septic field together, early.

Required supporting info also includes surface drainage and piping, nature of the facility, location of all water supplies/geothermal boreholes/utilities/trash pits on or off the lot, and soil characteristics including seasonal high groundwater and rock occurrence.

**Subdivision approval:** Rule 511-3-1-.14 bars selling, leasing, or beginning physical development of a lot in a subdivision until the County Board of Health has issued **written approval of plans for water supply and sewage disposal**. For a 1988 subdivision this was presumably done at platting, but the individual lot permit is still required.

**Certified professionals:** Georgia maintains lists of certified septic installers, pumpers, and **soil classifiers** — linked from the Clayton County Health District page.

### 6.4 Electricity

`[OFFICIAL]` **Central Georgia EMC (CGEMC)** — a member-owned cooperative serving **over 69,000 billed accounts across 16 counties, explicitly including Clayton, Fayette, and Henry**. New service: **(770) 775-7857**, Mon–Fri 8 am–5 pm. [CGEMC Service Area](https://www.cgemc.com/service-area) · [Establish Service](https://www.cgemc.com/establish-service) · [Rates](https://www.cgemc.com/rates)

`[ESTIMATE]` CGEMC is the most likely provider for this location given its stated Clayton County territory and the property's rural-fringe position. **Georgia Power** also serves large parts of Clayton County and cannot be ruled out. Georgia Power notes it froze rates until 2029 (July 2025) and lowered rates ~$50/yr for a typical residential customer in May 2026. `[OFFICIAL]` [georgiapower.com](https://www.georgiapower.com/)

⚠️ **Georgia has no retail electric choice for residential customers** — territory is assigned by statute. Confirm the serving utility by calling CGEMC with the parcel ID before assuming. Note also **Snapping Shoals EMC** serves parts of Henry County but I found no evidence of Clayton County panhandle territory. `[UNVERIFIED]`

Regulator / territory reference: [Georgia PSC — Electric](https://psc.ga.gov/utilities/electric/) · [PSC — EMC and Municipal Electric Systems](https://psc.ga.gov/utilities/electric/emc-and-municipal-electric-systems/)

### 6.5 Natural gas and propane

`[OFFICIAL]` **Atlanta Gas Light (AGL)** is the distribution utility for most of Georgia (~1.8 million customers) and its ZIP-level service area tool indicates **AGL offers service in ZIP 30228**, with the caveat *"Areas within this ZIP code may vary."* [AGL Service Area](https://www.atlantagaslight.com/company/our-service-area.html)

`[UNVERIFIED]` **Street-level natural gas availability on Edgewater Drive is NOT confirmed.** A 1988 large-lot subdivision on a rural fringe may well have no gas main. **Call AGL to confirm whether a main fronts the property** before specifying gas appliances.

Georgia's gas market is **deregulated for the commodity**: AGL owns and maintains the pipes and bills delivery charges, while you select a certified marketer for the gas itself (e.g. [True Natural Gas](https://www.truenaturalgas.com/true-natural-gas-service-area-map)). Marketers offer variable, fixed (typically 12–24 month), and discounted rates priced per therm; watch for exit fees and automatic rollover to variable rates at contract end. `[OFFICIAL]` [AGL Pricing and Rate Plans](https://www.atlantagaslight.com/residential/pricing-and-rate-plans.html)

**Propane:** `[UNVERIFIED]` If no gas main is present, propane is the standard alternative in this market, with tanks either leased or owned and multiple regional suppliers competing. I did not verify specific local suppliers or current pricing. Note that a buried propane tank would be an "accessory structure"/feature subject to the septic-field and 150-ft buffer restrictions.

### 6.6 Internet / broadband

`[UNVERIFIED]` **I could not obtain authoritative address-level broadband availability.** The **FCC National Broadband Map** API blocked automated location queries from this environment (HTTP 403 on the location endpoint; the block-level summary endpoints returned 404). I confirmed the map's current data vintage is the **December 31, 2025 biannual filing**.

→ **Check it yourself — it is the authoritative source and takes 30 seconds:** [broadbandmap.fcc.gov](https://broadbandmap.fcc.gov/) — enter the full address. The map reports every provider's claimed technology and maximum advertised speeds at that specific location, plus a challenge process if the data is wrong.

For reference, the parcel's census block GEOID is **130630406361000** (state 13 / county 063 / tract 040636 / block 1000). `[OFFICIAL]` Census

**Providers advertising service in the Hampton / 30228 area** — all `[ESTIMATE]`/`[UNVERIFIED]` at this address, since ZIP-level marketing claims routinely overstate coverage on rural fringes:

| Provider | Technology | Notes |
|---|---|---|
| **AT&T** | Fiber and/or DSL/fixed | AT&T states **"AT&T Fiber is available in parts of Hampton, GA"** and directs users to check by address — an explicit partial-coverage caveat. `[OFFICIAL]` [att.com/local/fiber/georgia/hampton](http://att.com/local/fiber/georgia/hampton) |
| **Xfinity / Comcast** | Cable | States it "provides internet service in the Hampton area." Xfinity's own serviceability guidance notes an address may be unserviceable if **"more than 300 feet from our physical network"** — a real risk on a large wooded lot. `[OFFICIAL]` [xfinity.com/local/ga/hampton](https://www.xfinity.com/local/ga/hampton), [serviceability](https://www.xfinity.com/support/articles/determining-serviceability) |
| **Spectrum** | Cable (fiber-fed coax) | Marketed in the area. `[ESTIMATE]` |
| **T-Mobile / Verizon** | 5G fixed wireless | Commonly available where cable is not. `[UNVERIFIED]` |
| **Starlink** | LEO satellite | Available in select areas, self-install, no contract. `[ESTIMATE]` |

**Do not assume fiber.** AT&T's own "available in parts of" language plus Xfinity's 300-ft rule mean a vacant wooded lot at the end of a 1988 subdivision is exactly the profile where a new drop may require construction at the owner's cost. Verify by address, and ask about installation/construction charges for a **vacant** parcel specifically — availability at a neighbor's built house does not guarantee availability at an unimproved lot.

---

## 7. Short-term rentals

### 7.1 ⭐ Bottom line: a non-owner-occupied STR is NOT permitted

Clayton County regulates STRs, and the regime is **owner-occupancy-based**. A pure investment/absentee short-term rental is not an allowed use in unincorporated Clayton County.

### 7.2 The ordinance

`[OFFICIAL]` **Ordinance 2019-22**, approved by the Board of Commissioners **February 5, 2019**, creating **Chapter 22 (Businesses), Article XII — Short Term Rental Units, Sec. 22-900**. Drafted "to address short-term rental operations throughout **unincorporated Clayton County**."

Source: [Clayton County Short-Term Rental Unit License Checklist & Supplemental Form (PDF)](https://www.claytoncountyga.gov/download/99/business-and-alcohol-license-forms/29667/short-term-rental-unit-license-checklist-supplemental-form.pdf) · Code: [Municode Ch. 22](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_CH22BU)

**What qualifies as a Short-Term Rental Unit:**
1. **Non-subsidized** (not Section 8 or other federally funded grants)
2. ⭐ **"Owner-occupied property & structure, meaning, it cannot be a rented or leased"**
3. "Shall be located inside or adjacent to its owner-occupied [structure] located on the same property"
4. Eligible structures: Houses (single-family attached or detached); Condominiums/Townhomes (**must be owned, not rented or leased**)

**License requirements:**
- Unit may be rented to the same tenant for a period of **less than thirty (30) days** — this is the definition of the regulated term, so there is effectively **no minimum stay** below 30 days
- Owner, platform, **or managing operator** must obtain a **County Business License**, and **the BL number must appear in any advertisement** of the rental unit
- License valid for **one (1) year** from date of issuance
- **The property cannot be advertised before a license is issued**

**Required reviews:** Zoning Approval · Fire Marshal Approval · **Tax Commissioner Approval (verifies the address on your driver's license against the deed/tax record** — i.e. an active owner-occupancy test) · Business License Review

**Required inspections:** Fire Marshal Inspection · Building Inspection

**Operating conditions (from the supplemental form):**
- Cannot be subsidized by any federal, state, and/or local funding
- Must obtain County Business License
- **Must be owner occupied and cannot be conducted within a rental property**
- Same-tenant stays under 30 days
- ⭐ **All parking must be accommodated on the same lot** (no street parking) — note the HOA separately fines street/grass parking (§5.4)
- Must be inspected by the Building Official and Fire Marshal
- ⭐ Must **post the County Noise Ordinance (Chapter 62 — Offenses and Miscellaneous Provisions) in a visible location inside the unit**
- Business license number in **any** advertisement
- Non-compliance **may result in revocation of the business license**

**Occupancy limits:** `[UNVERIFIED]` **No explicit occupancy cap appears** in the license checklist or supplemental form. Practical limits will come from the Fire Marshal inspection and building code egress/bedroom count. The full text of Sec. 22-900 may contain more; I was not able to retrieve that section's operative text.

### 7.3 ⚠️ A moratorium is currently in force

`[OFFICIAL]` **Resolution No. 2026-153**, adopted **July 2026**, establishes "a moratorium on the acceptance of any applications related to boarding homes, group homes, personal care homes, **short term rentals** and community living arrangements in Clayton County."

[Resolution 2026-153 (PDF)](https://www.claytoncountyga.gov/wp-content/uploads/wpfd/preview_files/2026-153(4a7d0a7210a4d80f1867a99bc88cc2c6).pdf)

Operative terms:
- **Section 2(a):** moratorium on receipt and acceptance by county staff of applications for **rezoning, conditional use, or site development permits** as they relate to the development of those uses
- **Section 2(b):** duration **until December 31, 2026**, or until a modified ordinance is adopted concerning these uses, **unless extended for good cause**
- **Section 2(d):** no effect on approvals or permits previously issued, or development plans previously approved; does not affect permits or site plan reviews that received preliminary or final approval, or for which consultations with county staff occurred on or before the effective date
- **Section 2(e):** any application accepted in violation is **"deemed in error, null and void and of no effect whatsoever"**
- **Section 3:** a **vested-rights exemption process** exists — a written request with verified supporting data may be reviewed by the Zoning Administrator; applicants may file for exemption, with a public hearing before the Board of Commissioners within 30 days of receipt. The Board may grant an exemption where the proposal conforms to the *proposed* ordinances/plan. An exemption merely allows staff to accept and process the application; it confers no rights and is not final approval.

The County's stated purpose is to **revise the definitions** of these uses "to better delineate between these land uses and to determine the type and amount of said developments consistent with current development patterns."

**Related moratorium:** `[OFFICIAL]` **Resolution No. 2026-120** (extended **June 2, 2026**) continues a moratorium on applications for **new construction of single-family residential subdivisions or multi-family residential developments**, until the County adopts a revised Code or **December 31, 2026**, whichever first occurs. [Planning & Zoning](https://www.claytoncountyga.gov/government/community-economic-development/planning-zoning/)

→ `[ESTIMATE]` Res. 2026-120 targets **subdivision and multi-family development applications**, not a single-lot building permit on an existing lot of record, so a one-house build should fall outside it. **But confirm with Planning & Zoning**, because the wording is broad and the county is mid-rewrite.

**Also in flight:** a **full Zoning Ordinance rewrite** is underway — [engagesycamore.mysocialpinpoint.com/claytonzoningrewrite](https://engagesycamore.mysocialpinpoint.com/claytonzoningrewrite) — plus Initiation Resolution **2025-177** (approved Aug 19, 2025) concerning **minimum lot sizes**, and separate moratoria on gas stations and convenience stores (Res. 2026-162). `[OFFICIAL]` **Every zoning conclusion in this report is a snapshot of a code that is actively being rewritten.**

### 7.4 Taxes

**Clayton County hotel/motel excise tax: 8%.** `[OFFICIAL]` The county's Hotel/Motel Tax Report Form (rev. 9-2025) shows **"Tax Due (8%)"**, less a **collection fee of 3% of tax due**, plus penalty if late. Remitted monthly to Clayton County Community & Economic Development Department, 121 S. McDonough Street, Annex 2, Jonesboro, GA 30236. The form requires rooms occupied, rooms available, percent occupancy, average room rate, gross total room rentals, permanent guest rentals, and taxable rentals.

[Clayton County Hotel/Motel Tax Report Form (PDF)](https://www.claytoncountyga.gov/download/99/business-and-alcohol-license-forms/29679/hotel-motel-tax-report-form.pdf)

**Georgia state-level STR taxes** `[OFFICIAL]`:
- **State and local sales tax** applies to accommodations.
- **Georgia $5/night state hotel-motel fee** applies to lodging (O.C.G.A. § 48-13-50.3) — `[ESTIMATE]` generally applicable, but exemptions exist; confirm applicability to STRs with a Georgia tax advisor.
- **Local hotel-motel excise tax** authority: **O.C.G.A. § 48-13-51**. A rate of 3% or less requires only a local ordinance; rates above 5% require a specific act of the Georgia General Assembly. Clayton County's 8% sits in the band requiring state authorization. `[OFFICIAL]` [Georgia DCA — Hotel-Motel Tax ordinance guidance](https://dca.georgia.gov/document/publications/ordinance-guidance-51a1-1-3-tax/download)
- **Income tax** on rental earnings.
- Marketplace facilitators (Airbnb/Vrbo) collect some but not necessarily all of these — **the county ordinance makes the owner, platform, or managing operator responsible for the business license**, and the hotel/motel tax form is filed by the operator.

> ⚠️ Do not confuse Clayton **County** with the **City of Clayton** (Rabun County, north Georgia), which has its own 8% hotel-motel tax authorized by **HB 60 (2023)** following its Resolution 2022-3. Several search results conflate the two. Those documents do **not** apply here.

### 7.5 STR conclusion

| Question | Answer |
|---|---|
| Permitted? | **Only as an owner-occupied STR.** A non-owner-occupied investment STR is not an allowed use. |
| Permit required? | **Yes** — County Business License + Zoning, Fire Marshal, Tax Commissioner and Business License reviews, plus Fire Marshal and Building inspections |
| Minimum stay? | None imposed; the ordinance *regulates* stays of **under 30 days** |
| Occupancy limits? | **NOT FOUND** in published materials; practically set by Fire Marshal/building code |
| Hotel-motel tax? | **8%** county, less 3% collection fee, plus state sales tax and the state lodging fee |
| Currently applying? | ⚠️ **Blocked by moratorium (Res. 2026-153) through at least Dec 31, 2026** |
| HOA angle | ⚠️ **The Unit 3 covenants may independently prohibit short-term rentals — unread (§5.4). Check before relying on any STR plan.** |

---

## 8. Hobby farming

### 8.1 ⭐ Chickens: permitted — Clayton County has a dedicated ordinance

`[OFFICIAL]` **Clayton County Zoning Ordinance Sec. 6.42 — Chicken Keeping Ordinance** (Ord. No. 2017-41, § 16, 5-30-17). [Municode Sec. 6.42](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_APXAZO_ART6DEST_S6.42CHKEOR)

**Purpose:** "to allow for keeping of poultry in single-family residential districts within the County, provided that certain requirements are met."
**Scope:** "effective in the area of Clayton County, GA. **outside incorporated cities and towns**" — i.e. exactly this parcel.
**Permitted in:** AG, ER, and **RS-180** (`P`). Not permitted in RS-110 or any other district.

**Sec. 4 — Requirements, verbatim:**
> a. **Minimum lot size: 18,000 square feet**
> b. **Four (4) chickens per 18,000 square feet** of property are permitted **up to a maximum of twelve (12) chickens**
> c. Chickens may only be kept on properties with an **occupied residence**
> d. **No roosters** or **on-site slaughter** allowed
> e. Hen house/coop can be located **within the side and rear areas only**
> f. Hen house/coops must have **at least four square feet per chicken**
> g. Chickens shall be **contained (fenced)** on the lot; the containment area shall be on the **side and rear areas only** and limited to **no more than forty percent of the lot**
> h. **Setback — minimum of 20 feet from all property lines**
> i. **No on-site chicken sales** (or sale of other permitted fowl)
> j. All coops and surrounding areas properly maintained and kept clean so as not to become a nuisance; **coops and feed secured at all times** to prevent nuisance with mice, rodents and pests

**Sec. 5 — Permitted activities:** "Keeping of chickens for **personal consumption of eggs**."

**Applied to this lot** `[ESTIMATE]`: 57,943 SF ÷ 18,000 = 3.2 → 3 increments × 4 = 12 → **capped at the maximum of 12 hens.** Coop needs ≥48 SF for 12 birds, sited in the side or rear area, ≥20 ft from every property line, fenced run ≤40% of the lot (≤23,177 SF). Requires an occupied residence first — **you cannot keep chickens on the vacant lot before building the house.**

### 8.2 Goats and other livestock: NOT permitted

`[OFFICIAL]` In the Article 3 Agricultural Uses matrix, **"Keeping of livestock"** is `P` in **AG only** and `N` in **RS-180**. Likewise `N` in RS-180: agricultural crop production/processing/storage, agricultural product sales, grazing and pasture land, riding academies and stables, kennels, confined animal feeding operations.

→ **Goats are not an allowed use on this lot.** Changing that would require rezoning to AG — which would be inconsistent with the subdivision, the covenants, and the current residential moratorium.

### 8.3 Ducks: ambiguous

`[UNVERIFIED]` Sec. 6.42 is titled "Chicken Keeping Ordinance" and its definition covers only *Chicken: Gallus domesticus*. However, Sec. 4(i) prohibits "No on-site chicken sales **(or sale of other permitted fowl)**" — language implying other fowl may be permitted somewhere in the code. The Article 3 use matrix lists only "Keeping of chickens." **The ordinance neither clearly permits nor clearly prohibits ducks.** Ask the Zoning Administrator for a written interpretation.

### 8.4 Rabbits: not addressed in zoning

`[UNVERIFIED]` **NOT FOUND.** Rabbits appear in neither the Article 3 use matrices nor Sec. 6.42. They may be treated as household pets (RS-180 accessory uses include "shelters or enclosures for household pets") or as livestock depending on number and purpose. **Chapter 14 — ANIMALS** of the county code is the other place to check; I confirmed the chapter exists but did not retrieve its operative text. Also check the Clayton County **Animal Control** ordinance. [Animal Control](https://www.claytoncountyga.gov/services/animal-control)

### 8.5 Bees: not addressed

`[UNVERIFIED]` **NOT FOUND.** No beekeeping provision appears in Sec. 6.42 or the Article 3 use matrices. Georgia has a state **Beekeeping Act** that limits local regulation of beekeeping in some circumstances — relevant but not researched here. Check Chapter 14 and ask Planning & Zoning.

### 8.6 ⚠️ The HOA covenants are the likely binding constraint

Even where zoning permits chickens, **the Waterpointe Unit 3 Protective Covenants very likely restrict or prohibit poultry and livestock** — animal restrictions are near-universal in 1988-era Georgia subdivision declarations of this type. Sec. 4.6(E)'s conflict rule and standard covenant law both mean **the more restrictive of zoning and covenant governs.** Since I could not read the covenants (§5.4), treat zoning permission as the **ceiling**, not the answer.

### 8.7 Hobby farming summary

| Animal | Zoning status in RS-180 | Authority |
|---|---|---|
| **Chickens (hens)** | ✅ **Permitted — up to 12**, with conditions | Sec. 6.42 `[OFFICIAL]` |
| Roosters | ❌ Expressly prohibited | Sec. 6.42(d) `[OFFICIAL]` |
| On-site slaughter | ❌ Expressly prohibited | Sec. 6.42(d) `[OFFICIAL]` |
| **Goats / livestock** | ❌ **Not permitted** (AG only) | Art. 3 use matrix `[OFFICIAL]` |
| **Ducks** | ⚠️ Ambiguous | `[UNVERIFIED]` |
| **Rabbits** | ⚠️ Not addressed in zoning | `[UNVERIFIED]` |
| **Bees** | ⚠️ Not addressed | `[UNVERIFIED]` |
| *All of the above* | ⚠️ **Subject to HOA covenants — unread** | §5.4 |

---

## 9. Radon

`[OFFICIAL]` **Clayton County, Georgia is EPA Radon Zone 2 — moderate potential.**

I determined this by rendering the official EPA map PDF at high resolution and sampling the county's fill color against the legend swatches programmatically. Clayton County reads RGB (250,160,0) — matching the **Zone 2 orange** legend swatch (249,160,0), not the Zone 1 red (200,24,24).

Source: [EPA Map of Radon Zones — Georgia (PDF)](https://www.epa.gov/sites/default/files/2014-08/documents/georgia.pdf) · [EPA Map of Radon Zones](https://www.epa.gov/radon/epa-map-radon-zones-0)

| Zone | Meaning | Counties |
|---|---|---|
| **Zone 1** (red) | Predicted average indoor screening level **> 4 pCi/L** | In metro Atlanta: **Cobb, Fulton, DeKalb, Gwinnett** |
| **Zone 2** (orange) | Predicted average **≥ 2 and ≤ 4 pCi/L** | ⭐ **Clayton**, and also Henry, Fayette, Spalding, Newton, Rockdale, Coweta, Butts |
| Zone 3 (yellow) | Predicted average **< 2 pCi/L** | Most of south Georgia |

> **Worth noting:** the county correction in §0 does **not** change the radon answer. **Clayton and Henry are both Zone 2.** This is one of the few items where the jurisdictional error was harmless.

**EPA's own caveats, which matter here:**
- The map was developed in **1993** using indoor radon measurements, geology, aerial radioactivity, soil parameters, and foundation types. It is dated.
- *"The Map of Radon Zones should not be used to determine if individual homes need to be tested."*
- *"**All homes should be tested, regardless of zone designation.**"*
- Fix your home at **≥ 4 pCi/L**; consider fixing between **2 and 4 pCi/L**.
- EPA directs users to consult **USGS Open-File Report 93-292-D, "Preliminary Geologic Radon Potential Assessment of Georgia"** ([doi:10.3133/ofr93292D](https://doi.org/10.3133/ofr93292D)) for **intra-county variation** — important because a single county-wide zone masks local geology.

**Practical implication for new construction.** Zone 2 does not mandate radon-resistant construction under Georgia's building code, but the incremental cost of passive radon-resistant new construction (RRNC) — a sub-slab vent mat, sealed membrane, and a capped vertical stack — is low at the framing stage and expensive to retrofit. Given Zone 2 status *and* the Piedmont crystalline bedrock beneath this site (§10), which is the granitic/gneissic rock type most associated with elevated radon in Georgia, **passive RRNC is a sensible specification**, with post-occupancy testing to decide whether to activate the stack with a fan.

`[UNVERIFIED]` **Georgia-specific county radon measurement data: NOT RETRIEVED.** The Georgia radon program (administered through UGA Cooperative Extension) publishes test-result summaries, but I did not obtain verified Clayton County average pCi/L figures from a primary state source. Third-party aggregators report a Georgia statewide average around 7 pCi/L, but that figure is `[UNVERIFIED]` and self-selected-sample data — do not rely on it. **Test the finished house.**

---

## 10. Sinkholes, karst, and geology

### 10.1 ⭐ Conclusion: not karst, and sinkhole risk is negligible

**Clayton County is in the Georgia Piedmont, underlain by crystalline metamorphic bedrock.** Karst and dissolution sinkholes require soluble bedrock — limestone, dolomite, gypsum, or other evaporites. **None is present here.**

### 10.2 Bedrock at the parcel — point query

`[OFFICIAL]` I ran a geologic point query at the parcel's interior coordinate (-84.36980879, 33.41612567):

| Attribute | Value |
|---|---|
| **Map unit** | **Biotitic Gneiss / Mica Schist / Amphibolite** |
| **Lithology** | Major: amphibolite, biotite gneiss, mica schist |
| **Age** | **Precambrian to Paleozoic** |
| **Source** | **Georgia Geological Survey** (a branch of EPD, Georgia DNR), *Digital Geologic Map of Georgia (ver. 2)*, 1999, updated Oct 2000, scale 1:500,000 |

Retrieved via the [Macrostrat geologic map API](https://macrostrat.org/api/v2/geologic_units/map?lat=33.41612567&lng=-84.36980879&scale=medium), which serves the Georgia Geological Survey compilation. Data license CC-BY 4.0.

These are **hard, crystalline, non-soluble metamorphic rocks** — the classic Piedmont assemblage. This independently confirms the "Piedmont crystalline rock?" hypothesis in the brief. ✅

### 10.3 USGS karst mapping

`[OFFICIAL]` The USGS national karst map is built from "the presence of soluble bedrock lithologies, **carbonate and evaporite rocks**, or low-viscosity lava extrusive volcanic rocks… the most important factors in developing karst or volcanic pseudokarst."

- [USGS Karst Map of the Conterminous United States — 2020](https://www.usgs.gov/media/images/karst-map-conterminous-united-states-2020)
- [USGS SIR 2008-5023, Weary — national karst map methodology (PDF)](https://pubs.usgs.gov/sir/2008/5023/pdf/07weary.pdf)
- [USGS — Karst Aquifers](https://www.usgs.gov/mission-areas/water-resources/science/karst-aquifers)
- [USGS — Current and future sinkhole susceptibility in karst and pseudokarst areas](https://www.usgs.gov/publications/current-and-future-sinkhole-susceptibility-karst-and-pseudokarst-areas-conterminous)

Georgia's genuine karst is in the **northwest** (Valley and Ridge — Walker, Catoosa, Dade, Chattooga counties) and the **Coastal Plain / Dougherty Plain** in the southwest (Albany/Dougherty County area), where Ocala Limestone produces real sinkholes. **The Piedmont — including Clayton County — is not karst terrain.** `[ESTIMATE]` (reasoned from `[OFFICIAL]` lithology + `[OFFICIAL]` USGS karst criteria; I could not render the national karst map at county scale to read the polygon directly.)

### 10.4 What the geology *does* mean for this site

Ruling out sinkholes is not the same as ruling out geotechnical issues. Piedmont crystalline terrain has its own well-known characteristics:

- **Saprolite.** Piedmont bedrock weathers in place to deep clayey residual soil. Depth to competent rock is highly variable over short distances — **10 ft in one boring, 60 ft in another 50 ft away.** Plan a geotechnical investigation with multiple borings across the actual building footprint.
- **Shallow rock / blasting risk.** The converse problem: rock near the surface drives up excavation cost for basements, footings, utility trenches, and especially **septic drainfield installation**. Rule 511-3-1 requires **24 inches of vertical separation to rock** beneath the trench bottom — shallow rock can disqualify an otherwise acceptable area.
- **Perched groundwater and seeps.** Common at the saprolite/rock interface on sloped lake-adjacent lots; affects basement waterproofing and drainfield suitability (the same 24-inch separation applies to seasonal groundwater).
- **Slope stability and erosion.** The listing describes a "**gentle rolling**" wooded lot `[LISTING]`, which is favorable. Still, this is a lake-adjacent slope inside a drinking water supply watershed — erosion and sedimentation control will be scrutinized (§11.3).
- **Radon.** Granitic and gneissic Piedmont rocks are the lithologies most associated with elevated indoor radon in Georgia — ties directly to §9.

**Flood:** `[OFFICIAL]` The county parcel record flags **FLOODPLAIN: NO**. Verify against FEMA directly: [FEMA Map Service Center](https://msc.fema.gov/portal/home). For floodplain and drainage questions Clayton County directs inquiries to **CCWA at (678) 422-5145 ext. 5508**. `[OFFICIAL]`

> One flood-adjacent consideration the FEMA map will not show: the parcel sits **immediately upstream-adjacent to a "High hazard" dam** (NID GA03893). High hazard means failure "will probably cause loss of human life" **downstream** — a lot upstream of the dam is not in the failure inundation path, so this is **not** a direct risk to this parcel. Official inundation mapping lives in the dam's Emergency Action Plan, held by CCWA and the Georgia Safe Dams Program.

---

## 11. Building permits, land disturbance, and construction

### 11.1 Permitting authority and process

`[OFFICIAL]` **Clayton County Department of Community & Economic Development** — Building Permits & Inspections. **(770) 477-3569**. 121 South McDonough St., Jonesboro, GA 30236.
[Building Permits](https://www.claytoncountyga.gov/government/community-economic-development/building-permits/) · [Residential Building Permit Application (PDF)](https://www.claytoncountyga.gov/download/91/building-permits/29691/residential-permit-application.pdf) · [Permit Requirements tool](https://cda.claytoncountyga.gov/PermitRequirements/24) · [Community Development Assistant / Zoning Assistant](https://cda.claytoncountyga.gov/ZoningAssistant)

**Published process sequence for a new residential build** `[OFFICIAL]`:
1. **Application submittal** with supporting documents per the Document Requirements Matrix
2. **Reviews** — Zoning Approval → **Tree Ordinance** → Site Plan and supporting documents
3. **Permit issuance**
4. Construction mobilized and initiated
5. **Inspections** — called in sequentially
6. **Certificate of Occupancy** — issued when applicable codes are met and all inspections approved

**Site plan requirement:** "Site Plan is required for all residential construction. Site Survey is accepted for residential construction on an improved property." → **This lot is unimproved, so a full site plan is required, not just a survey.**

A **Tree Ordinance** review is part of the process; a **Residential Tree Removal Application** is **no charge**, and **Tree Harvesting** is $50 minimum ($1.00/acre). A **Tree Preservation Ordinance** is published ($20). Relevant here — the lot is "nicely wooded" `[LISTING]`.

**Applicable codes:** Clayton County publishes a [Code Requirements sheet (PDF)](https://www.claytoncountyga.gov/wp-content/uploads/2022/09/CLAYTON-COUNTY-CODE-REQUIREMENTS.pdf) and **Chapter 18 — Buildings and Building Code Regulations** ([Municode](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_CH18BUBUCORE)). Georgia adopts the International Codes with state amendments.

Separate trade permits with their own fee schedules exist for [Electrical](https://www.claytoncountyga.gov/download/91/building-permits/29692/electrical-permit-application.pdf) (new residential computed on square-foot area), [HVAC](https://www.claytoncountyga.gov/download/91/building-permits/29690/hvac-permit-application.pdf), and plumbing. Fire/EMS [Plans Review](https://www.claytoncountyga.gov/download/91/building-permits/29693/county-fire-ems-plans-review-application.pdf) is **$0.10 per sq ft**.

### 11.2 Planning & zoning fee schedule (current)

`[OFFICIAL]` [Clayton County Planning & Zoning Fees](https://www.claytoncountyga.gov/government/community-economic-development/planning-zoning/fees/)

| Item | Fee |
|---|---|
| **Conditional Use Permit** (needed for an ADU) | **$500** |
| Rezoning — single-family residential, <3 acres | $500 |
| Rezoning — 3–10 acres / >10 acres | $1,000 / $1,500 |
| Zoning Modifications (conditions or modified site plans) | $500 |
| Land Use Plan Amendment | $500 |
| **Board of Appeals Variance or Administrative Appeal** | **$400** |
| Minor Subdivision | $250 |
| Preliminary Plat Review | $500 |
| Final Plat Review | $250 min. (first 5 lots), $50 each additional |
| **Zoning Verification Letter** | **$100 per parcel** |
| Fence and Wall Permit | $25 (≤1,000 linear ft) / $75 (>1,000 ft) |
| Residential Tree Removal Application | **No charge** |
| Tree Harvesting | $50 min. ($1.00/acre) |
| Zoning Ordinance (printed copy) | $50 |
| Subdivision Regulations / Tree Preservation Ordinance | $20 / $20 |
| Development Procedures | **No charge** |
| *Resubmittal surcharge* | **+$150 for each submittal following initial review** |

⚠️ **Note that +$150 resubmittal fee** — on a constrained lake lot with buffer issues, plan to get the site plan right the first time.

### 11.3 Land disturbance

`[OFFICIAL]` **Clayton County Department of Transportation and Development — Land Development Division.** Interim Director: Keith Rohling, P.E. 7960 North McDonough Street, Jonesboro, GA 30236 · **(770) 477-3674**
[Land Development](https://www.claytoncountyga.gov/government/transportation-and-development/land-development/)

Its stated role: "Review plans for new residential, commercial and industrial developments; **Issues clearing and grading permits**; Inspects residential, commercial and industrial site developments."

- **Clayton County 2007 Land Disturbance and Right-of-Way Construction Guideline Books** — purchasable from the Land Development Office for **$50.00** (cash or check to Clayton County Board of Commissioners), or downloadable from the page.
- A [Plan Review Check List (PDF)](https://www.claytoncountyga.gov/download/93/land-development/29451/plan-review-checklist.pdf) is published; note it requires information for **"a distance of 200 feet, minimum, outside property lines."**
- **Chapter 38, Article II — Soil Erosion and Sedimentation Control** governs E&S. Georgia's Erosion and Sedimentation Act imposes a **25-ft undisturbed buffer along state waters**, and any encroachment requires an **EPD buffer variance** (Zoning Sec. 4.6(C)). EPD routinely processes such variances in Clayton County — see e.g. [EPD Clayton County buffer variance public notices](https://epd.georgia.gov/document/document/bv-031-24-03-clayton-county-public-notice/download).
- **Stormwater:** CCWA performs development plan review and inspections for stormwater infrastructure, under the **Post-Development Stormwater Management** ordinance (Chapter 38, Article V) and **Chapter 25 — Stormwater Management**. **CCWA Stormwater Development Guidelines (PDF)** is the governing technical document, and Zoning Sec. 4.5(A)(4) mandates compliance with CCWA Guidelines in the small watershed. `[OFFICIAL]`

> `[ESTIMATE]` A single-family home on an existing lot of record typically disturbs under 1 acre and so usually falls below the threshold for a state NPDES construction stormwater permit (GAR100001 et seq., generally 1+ acre). But this lot is **1.33 acres inside a drinking water supply watershed adjacent to a public drinking water reservoir** — expect heightened E&S scrutiny regardless, and confirm NPDES applicability with Land Development based on your actual disturbed area.

### 11.4 Development impact fees

`[OFFICIAL]` **Clayton County has a development impact fee program: Code Chapter 88 — Development Impact Fees**, Article I, Sec. 88-1 et seq., adopted by the Board of Commissioners under the Georgia Development Impact Fee Act (**O.C.G.A. § 36-71-1 et seq.**). [Municode Ch. 88](https://library.municode.com/ga/clayton_county/codes/code_of_ordinances?nodeId=PTIICOCLCOGE_CH88DEIMFE)

⚠️ **The fee amounts are NOT published in the code.** The chapter's editor's note states: *"The development impact fee schedule is attached to the ordinance from which this chapter derives as **Attachment A** and is incorporated herein by reference as if fully set out at length. A copy of Attachment A is **on file and available for inspection** in the offices of the city."*

`[UNVERIFIED]` **Impact fee dollar amount per single-family dwelling unit: NOT FOUND.** It is not online. The code defines a "dwelling unit" broadly (single-family detached home, townhouse, duplex unit, apartment, condominium, "or any other type of domicile intended for long-term human occupancy") and ties fees to the county's **Capital Improvements Element**.

→ **Request Attachment A** from Community & Economic Development, (770) 477-3569, and ask for the **current per-dwelling-unit impact fee** for a single-family detached home in unincorporated Clayton County.

`[UNVERIFIED]` **The residential building permit fee schedule itself** is likewise not published as a simple table; building permit fees are typically valuation- or square-footage-based. Request a written fee estimate with the permit application.

### 11.5 Property taxes

`[OFFICIAL]` Clayton County 2025 **net millage rate: 14.552**. [Estimate Property Tax Bill](https://www.claytoncountyga.gov/government/tax-commissioner/estimate-property-tax-bill/) · Tax Commissioner (770) 477-3311

`[ESTIMATE]` At the current assessed value of **$24,000** (40% of the $60,000 appraised value, per Georgia's standard 40% assessment ratio):

**$24,000 ÷ 1,000 × 14.552 ≈ $349/year** as vacant land.

This will rise substantially once a house is built and reassessed. Note the parcel record carries `CUVA: YES` — a Conservation Use Valuation Assessment flag, which is unusual for a vacant residential subdivision lot and may be a data artifact. ⚠️ **If a CUVA covenant genuinely encumbers this parcel, it is a 10-year covenant with breach penalties, and building a house could trigger them.** Verify with the Tax Assessor — see §12.

### 11.6 Realistic development path and sequence

`[ESTIMATE]` Recommended order of operations:

1. **Boundary and topographic survey** — establish the true rear line against CCWA's parcel, locate the 150-ft buffer line, confirm frontage and depth, and locate any stream.
2. **Written zoning verification letter** ($100) stating RS-180, confirming lot-of-record status under Article 9, confirming whether the Panhandle Area Overlay applies, and confirming how the county measures the 150-ft buffer.
3. **CCWA Engineering written response** on sewer availability (§6.2) and a water/sewer connection fee estimate.
4. **If septic:** soil evaluation by a certified soil classifier, then Health Department construction permit (§6.3).
5. **Geotechnical borings** across the proposed footprint (§10.4).
6. **HOA architectural review** via the Building Modification process (§5.4), and read the Unit 3 covenants first.
7. **Site plan + building permit** application; E&S/land disturbance permit from Land Development.
8. Build to ≥1,800 SF (1-story) or ≥2,000 SF (2-story) heated, ≤35 ft tall, within 35% total impervious coverage.

---

## 12. ⚠️ Contradictions, conflicts, and data gaps

Flagging every inconsistency I found, as requested.

**C1 — The 150-ft buffer has two different measurement datums in the same ordinance.**
Sec. 4.5(D)(3): "150-feet protection buffer **adjoining the reservoir property**."
Sec. 4.6(E): "150-feet protection buffer adjoining the reservoir property **from the normal full-pool elevation**."
Because CCWA owns ~33 ft of upland between the lot and the water, these two readings differ by ~33 ft of buildable depth (~4,400 SF of lot area). Sec. 4.6(E)'s own conflict clause says **the more restrictive governs**, so assume measurement from the rear lot line. **Get the county's written interpretation.**

**C2 — MLS "private access to lake" vs. CCWA Rule 5.**
A Waterpointe listing advertises "private access to lake" `[LISTING]`; CCWA's published regulations state "**Access to the reservoir shall be made only at the entrance gate**" and prohibit wading/swimming/bathing `[OFFICIAL]`. **Trust the official regulation.** Do not pay a premium for private water access.

**C3 — RS-180 maximum lot depth conflicts with the J.W. Smith minimum lot depth — a genuine ordinance conflict.**
- Sec. 3.6: **Maximum** lot depth = **2.5 × lot width**. At ~147.5 ft of frontage → max depth ~**369 ft**.
- Sec. 4.5(D)(2): lots abutting J.W. Smith must have a **minimum** depth of **400 ft**.
- The subject lot is **~417 ft** deep — it satisfies 4.5(D)(2) and violates 3.6.
- **These two rules are mathematically irreconcilable for any lot narrower than 160 ft.** A 147.5-ft-wide lot literally cannot comply with both.
Sec. 4.5(D)(2) does contain a 10% hardship allowance "due to the configuration of the reservoir property." `[ESTIMATE]` The lot's 1988 plat date most likely makes this moot via nonconforming-lot-of-record protection (Article 9), but **this is the first question to put to the Zoning Administrator.**

**C4 — HOA says the first two declarations were recorded in Fulton County.**
For a Clayton County subdivision that is anomalous and may be a website error. Books 1446/1553 (claimed Fulton) and Books 1774/09403 (Clayton). **Title examiner must verify all four chains.** `[OFFICIAL]` as to what the HOA states; the underlying fact is `[UNVERIFIED]`.

**C5 — Two active moratoria and a full zoning rewrite.**
Res. 2026-153 (STR/group homes — conditional use applications frozen) and Res. 2026-120 (residential subdivision/multi-family applications frozen), both nominally through **Dec 31, 2026**, both extendable, plus an active **Zoning Ordinance rewrite** and Initiation Resolution 2025-177 on **minimum lot sizes**. **Every zoning figure in this report is a snapshot and could change.** Re-verify before closing.

**C6 — Sewer vs. septic is unresolved and the ordinance leans toward sewer.**
Sec. 4.5(D)(5) says sanitary sewer "**to be installed** unless EPD indicates such sewer should not be installed," yet the code also contains detailed septic lot-size rules that contemplate septic on watershed lots. **Unresolved — highest-priority call.** (§6.2)

**C7 — `CUVA: YES` on a vacant residential lot.**
Possibly a data artifact; possibly a real Conservation Use covenant with 10-year term and breach penalties. **Verify with the Tax Assessor.**

**C8 — "Club Lake" vs. "J.W. Smith Reservoir."**
The lobe fronting this lot carries the GNIS name "Club Lake" (GNIS 00312768) while CCWA and the county ordinance call the water body J.W. Smith Reservoir. Same water body; two names. Expect to see both in surveys, title work, and NHD-derived mapping.

**C9 — The Snoflo/NID mirror page misstates the location.**
Its prose says "Fayetteville, Georgia" in one sentence and "Clayton County" in another. The **tabular NID fields** (GA03893, Shoal Creek, 1984, 250 ac, 42.5 ft) are the reliable content; I relied only on those.

### Items I could not verify — stated plainly

| Item | Status | Why |
|---|---|---|
| **Unit 3 Protective Covenants content** | **NOT READ** | All four covenant PDFs are scanned images with no text layer; no OCR available in this environment. **High priority — read these.** |
| **Georgia SOS corporate registration for the HOA** | **NOT RETRIEVED** | ecorp.sos.ga.gov blocked by Cloudflare challenge |
| **CCWA reservoir management plan** | **NOT FOUND online** | Required by state Rule 391-3-16-.01(8); it is the document that actually decides docks and adjacent-owner access. Request from CCWA. |
| **CCWA water/sewer tap and connection fees** | **NOT PUBLISHED** | Quote-on-request only; call (770) 960-5207 |
| **CCWA sewer service area map / Edgewater Dr availability** | **NOT FOUND** | No map published |
| **Development impact fee amount** | **NOT PUBLISHED** | Chapter 88 "Attachment A" is inspection-only |
| **Residential building permit fee schedule** | **NOT PUBLISHED** as a table | Request written estimate |
| **Address-level broadband availability** | **NOT RETRIEVED** | FCC National Broadband Map API returned 403/404 to automated queries. Check manually at broadbandmap.fcc.gov |
| **Street-level natural gas availability** | **NOT CONFIRMED** | AGL confirms ZIP 30228 only, with "areas may vary" caveat |
| **Panhandle Area Overlay District applicability** | **NOT CONFIRMED** | County's `PEZ_OverlayAreas` service exposes no queryable layers |
| **Zoning Article 9 (nonconforming lots) text** | **NOT RETRIEVED** | Confirmed the article exists; operative text not pulled |
| **Sec. 22-900 full STR text** | **NOT RETRIEVED** | Worked from the official license checklist + supplemental form instead |
| **Reservoir depth (surveyed)** | **DOES NOT EXIST** | No national bathymetric survey for US reservoirs; bounded by 42.5 ft dam height |
| **Ducks / rabbits / bees** | **NOT FOUND** in zoning | Check Code Chapter 14 (Animals) and ask Planning & Zoning |
| **STR occupancy limits** | **NOT FOUND** | Not in published license materials |
| **Georgia state radon data for Clayton County** | **NOT RETRIEVED** | EPA Zone 2 confirmed; county-level pCi/L averages not obtained from a primary state source |
| **Electric provider confirmation** | **NOT CONFIRMED** at parcel | CGEMC serves Clayton County; Georgia Power also possible |

---

## 13. Verification call list

In priority order. Reference **Parcel 05050A A003, Unit 3 Lot 23, Waterpointe, 12396 Edgewater Dr** on every call.

| # | Who | Number | Ask |
|---|---|---|---|
| 1 | **CCWA Engineering** | (770) 960-5207 | **Is sanitary sewer available within 200 ft of the parcel / in the Edgewater Dr ROW?** Written water & sewer connection/tap/meter fee estimate. Request the **reservoir management plan**. Are private docks or adjoining-owner lake access permitted in any form? Is a buffer work/access permit program available? |
| 2 | **Clayton County Planning & Zoning** (Zoning Administrator Tyler L. McSwain) | (770) 477-3569 | Buy the **$100 Zoning Verification Letter**. Confirm: lot-of-record status under Article 9 given the 2.5×-width depth conflict (C3); **how the 150-ft buffer is measured** (C1); whether the **Panhandle Area Overlay** applies; whether Res. 2026-120 affects a single-lot permit; ADU/second-kitchen interpretation; ducks/rabbits/bees. |
| 3 | **Clayton County Health District, Environmental Services** | (678) 610-7469 | Septic feasibility on this lot; required soil evaluation; usable-area calculation given the 150-ft buffer; bedroom-count limits. |
| 4 | **Waterpointe HOA Board** | via [waterpointehoa.com](https://waterpointehoa.com/) | Current actual dues for a **vacant lot** (bylaws cap at $100); confirm membership is still non-compulsory; **Unit 3 covenant copy**; architectural review requirements; any rental restrictions. |
| 5 | **Clayton County Community & Econ. Dev.** | (770) 477-3569 | **Chapter 88 Attachment A impact fee schedule**; residential building permit fee estimate; STR moratorium status after Dec 31, 2026. |
| 6 | **Clayton County Land Development** | (770) 477-3674 | Land disturbance / clearing & grading permit requirements; NPDES applicability; E&S expectations in a water supply watershed; 2007 Guideline Books ($50). |
| 7 | **Clayton County Tax Assessor** | (770) 477-3311 | **Resolve the `CUVA: YES` flag** — is there a real Conservation Use covenant? Confirm current assessed value and millage. |
| 8 | **Central Georgia EMC** | (770) 775-7857 | Confirm serving electric utility for this parcel; new-service line extension cost. |
| 9 | **Atlanta Gas Light** | via [atlantagaslight.com](https://www.atlantagaslight.com/) | Is there a gas main on Edgewater Dr? |
| 10 | **Title attorney** | — | Examine all four covenant chains incl. the **Fulton County** anomaly (C4); confirm no CCWA easements/flowage rights encumber the lot; confirm Deed Bk 12617 Pg 653. |

**Self-serve checks:** [FCC National Broadband Map](https://broadbandmap.fcc.gov/) (address-level broadband) · [ecorp.sos.ga.gov](https://ecorp.sos.ga.gov/BusinessSearch) (HOA entity status) · [FEMA MSC](https://msc.fema.gov/portal/home) (flood) · [Clayton County property card](https://publicaccess.claytoncountyga.gov/Datalets/Datalet.aspx?mode=&UseSearch=no&pin=05050A%20A003)

---

## 14. Summary scorecard

| Topic | Finding | Confidence |
|---|---|---|
| **Jurisdiction** | **Unincorporated Clayton County** — not Henry, not Hampton city | ✅ Confirmed ×4 |
| **Reservoir owner** | **CCWA** — not HCWA | ✅ Confirmed ×3 |
| Reservoir | J.W. Smith, 250 ac, Shoal Creek, built 1984, high-hazard earth dam | ✅ Official |
| Zoning | **RS-180**, 18,000 SF min lot, 30/10/25 ft setbacks, 35% max coverage, 35 ft height | ✅ Official |
| Min. house size | **1,800 SF (1-story) / 2,000 SF (2-story) heated** | ✅ Official |
| Lot vs. J.W. Smith rules | **Passes** both ≥50,000 SF and ≥400 ft depth | ✅ Measured |
| **Controlling constraint** | **150-ft reservoir protection buffer** — no septic, no substantial structure | ✅ Official |
| Buildable depth | ≈237 ft after buffer + front setback | `[ESTIMATE]` |
| Lake access | **No private dock, no swimming, no gas motors, gate access only** | ✅ Official |
| Lot touches water? | **No** — ~33 ft of CCWA land intervenes | ✅ Measured |
| HOA | Waterpointe Community Assn. — **membership NOT compulsory**; vacant-lot dues capped **$100/yr** | ✅ Official (bylaws) |
| HOA covenants | ⚠️ **Unread — scanned images.** Priority item | ❌ Gap |
| Water | CCWA; base $15.06/mo + tiered | ✅ Official |
| Sewer vs. septic | ⚠️ **Unresolved** — ordinance leans sewer | ❌ Gap |
| Septic feasibility | Likely OK with public water (~37,900 SF usable vs. 25,000 required); fails with a well | `[ESTIMATE]` |
| Electric | Central Georgia EMC (likely) | `[ESTIMATE]` |
| Gas | AGL serves ZIP 30228; street-level unconfirmed | ⚠️ Partial |
| Broadband | ⚠️ Verify at FCC map; do not assume fiber | ❌ Gap |
| **STR** | **Owner-occupied only** + business license; **moratorium to Dec 31, 2026**; 8% hotel tax | ✅ Official |
| **Chickens** | ✅ **Permitted, up to 12 hens**, 20 ft setbacks, no roosters (Sec. 6.42) | ✅ Official |
| Goats/livestock | ❌ **Not permitted** in RS-180 | ✅ Official |
| **ADU / in-law suite** | ✅ **Permitted as Conditional Use** ($500), min 800 SF, rear yard if detached (Sec. 6.9 AS-05) | ✅ Official |
| **Radon** | **EPA Zone 2** (moderate, 2–4 pCi/L) — same for Clayton and Henry | ✅ Official |
| **Karst/sinkholes** | ❌ **Not karst.** Piedmont biotite gneiss/mica schist/amphibolite | ✅ Official |
| Geotech watch-items | Variable saprolite depth, shallow rock, perched groundwater | `[ESTIMATE]` |
| Flood | County flags **NO**; verify at FEMA | ✅ Official |
| Impact fees | Chapter 88 exists; **amount not published** | ❌ Gap |
| Property tax (vacant) | ≈ **$349/yr** at $24,000 assessed × 14.552 mills | `[ESTIMATE]` |
| Zoning stability | ⚠️ **Active rewrite + 2 moratoria** — re-verify before closing | ✅ Official |

---

### Methodology note

Findings were developed by querying live primary sources: the Clayton County ArcGIS REST services (parcels, zoning, municipal boundaries, hydrography), the US Census geocoder, Georgia Secretary of State rules (391-3-16-.01, 511-3-1), the Clayton County Code of Ordinances via Municode (current through Sep 10, 2026), CCWA and HCWA published documents, the USACE National Inventory of Dams, the EPA Map of Radon Zones, and the Georgia Geological Survey geologic map. Parcel geometry and distances were computed directly from the official polygon and cross-checked against the county's own reported perimeter (agreement within 0.1%). Table-image ordinance exhibits (RS-180 standards) and the EPA radon map were read visually from rendered official source files; the radon zone was additionally verified by programmatic pixel sampling against the legend. Where a source could not be reached, that is stated explicitly rather than inferred.

*Report compiled October 2026. Zoning, fee, rate, and moratorium information is time-sensitive. This is research, not legal, engineering, surveying, or tax advice.*
