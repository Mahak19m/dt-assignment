# Part B: Sourcing Strategy + 1000-Company Proposal
## DT Business Analytics Assignment
**Prepared by:** Mahak (GitHub: mahak19m)
**Date:** May 2026

---

# Question 1: Sourcing Methods

How would I find Federer companies across India beyond Google search?

---

## Method 1: Screener.in with Custom Filters

**What it is:** India's best-in-class financial screening tool for BSE/NSE listed companies.

**Why it works for this ICP:**
- Filter by industry sector (healthcare, specialty chemicals, agri-inputs), revenue band (Rs.50-500Cr market cap as proxy), and city using headquarters filter.
- Companies on Screener are public — you get revenue trends, ROCE, debt levels, promoter holding percentage (high promoter holding = promoter-driven, a positive Federer signal), and investor transcripts.
- High promoter holding (>60%) on Screener is a direct proxy for "not PE-controlled."

**Limitation:** Only covers listed companies (~5000 BSE/NSE listed). The most interesting Federer companies are often private — Screener misses them entirely.

---

## Method 2: MCA/Tofler NIC Code Mining

**What it is:** India's Ministry of Corporate Affairs registers all companies. Tofler and Zauba Corp provide searchable access by NIC code, state, and revenue band.

**Why it works for this ICP:**
- NIC codes like 2100 (pharma), 3250 (medical devices), 2106 (food ingredients), 0111 (seed crops) map directly to Basket B.
- Filter by state + revenue range (paid Tofler Pro subscription gives revenue data).
- Unlisted companies that Screener doesn't cover show up here — this is where private Federer companies hide.

**Specific NIC codes for Basket B:**
- 2100: Pharmaceutical products (filter out bulk generic by cross-checking company description)
- 2109: Other pharma products (specialty APIs, nutraceutical ingredients)
- 3250: Medical/surgical/dental instruments (IVD, implants)
- 0111: Seed crops (hybrid seeds)
- 2106: Food preparations NEC (specialty food ingredients, nutraceuticals)
- 2120: Veterinary medicines

**Limitation:** Revenue data on Tofler is often 1-2 years delayed (companies file late). NIC codes are self-reported and sometimes miscoded.

---

## Method 3: Industry Association Membership Lists

**What they are:** Sector bodies publish member directories — these concentrate Federer-profile companies.

**Key associations for Basket B:**
- **FICCI Health Services / AIMED (Association of Indian Medical Device Industry)** — medical device manufacturers
- **ABLE (Association of Biotechnology Led Enterprises)** — biotech, IVD, specialty diagnostics
- **FSII (Federation of Seed Industry of India)** — hybrid seed companies
- **AVMA (Animal Vaccination Manufacturers Association)** — veterinary biologics
- **ASSOCHAM Nutraceuticals Council** — nutraceutical ingredient manufacturers
- **Pharmexcil (Pharma Export Promotion Council)** — exporters of pharma and APIs (high-signal: Federer companies often export)

**Why it works:** Association membership requires minimum operational size and demonstrates industry participation — both positive Federer signals. Member directories are often free on association websites.

**Limitation:** Some members are large MNCs (auto-disqualify); some associations have outdated directories. Requires manual filtering.

---

## Method 4: USFDA and EU-GMP Establishment Databases

**What they are:** US FDA publishes a free searchable database of all foreign establishments approved to ship drugs/devices to the US. EMA (European Medicines Agency) similarly publishes EU-GMP certified sites.

**Why it works for this ICP:**
- USFDA approval is a near-perfect C3 differentiation signal — only technically capable manufacturers get and maintain it.
- Filter by India + product type (API, finished dosage, device) + state.
- Cross-reference the establishment address with revenue data (Tofler) to find Rs.50-500Cr companies in the list.

**Process:**
1. Go to FDA.gov → Establishment Inspection Program → search "India" + pharmaceutical
2. Export list, filter by state (Maharashtra for Pune, etc.)
3. Cross-reference company name against Tofler for revenue data
4. Eliminate >Rs.500Cr companies (Lupin, Sun, Cipla etc. will appear — discard)

**Limitation:** Only covers export-oriented pharma/device companies; misses domestic-focused specialty manufacturers. Does not cover agri-inputs, nutraceuticals, or animal health.

---

## Method 5: Trade Fair and Expo Exhibitor Lists

**What they are:** Industry expos publish exhibitor lists before and after each event — these are free and extremely useful.

**Key expos for Basket B:**
- **Medica India / MedEx India** — medical device exhibitors (mostly manufacturers)
- **Analytica India** — analytical instruments, diagnostics, life science tools
- **India Agri Show / Krishi Unnati Mela** — agri-input companies including hybrid seeds and biopesticides
- **CPhI India (Pharma Expo)** — pharma ingredients, APIs, nutraceutical ingredients
- **Poultry India** — animal health and nutrition companies

**Why it works:** Companies that pay to exhibit at industry expos are operationally active, growth-oriented, and accessible by definition. Exhibitor lists with booth numbers, company descriptions, and contact details are often available post-event on the expo website.

**Limitation:** Expos capture a specific snapshot in time; some smaller companies can't afford exhibition fees even if they qualify.

---

## Method 6: DSIR Recognition List

**What it is:** India's Department of Scientific and Industrial Research (DSIR) publishes a list of DSIR-recognized R&D labs — companies whose in-house R&D meets government-verified standards.

**Why it works:** DSIR recognition is a direct C3 + C4 proxy — it means the company has invested in documented, structured R&D capability. Every DSIR-recognized company in the Rs.50-500Cr range is worth investigating as a Federer candidate.

**Process:** Download the DSIR recognition list from dsir.gov.in → filter by NIC code and state → cross-reference against Tofler for revenue data.

**Limitation:** Many DSIR-recognized companies are large (>Rs.500Cr) — requires revenue filtering.

---

## Method 7: LinkedIn Outbound Search with Boolean Filters

**Why it works:** LinkedIn company search with boolean filters (industry + headcount + geography) lets you find private companies not in financial databases.

**Search template:**
`"Founder" OR "Managing Director" AND ("Pune" OR "Hyderabad") AND ("medical device" OR "diagnostic" OR "nutraceutical") AND (company size: 51-500 employees)`

The employee count filter (51-500) is a reliable proxy for Rs.50-300Cr revenue in manufacturing.

**Limitation:** Requires LinkedIn Sales Navigator for full boolean search (paid); company employee counts self-reported; doesn't filter by revenue directly.

---

# Question 2: The 1000-Company Proposal

**Goal:** Build a list of 1000 ICP-qualified Federer companies in India within 1 month.

---

## Framing

The challenge is not finding 1000 company names — that's easy. The challenge is qualifying 1000 companies against the Federer criteria (E1, E2, C3–C8) at sufficient confidence that DT can act on the list without wasting outreach effort.

My approach is a **3-stage funnel:**
1. **Universe generation** — build a raw list of 8000-10000 potential companies using automated data sourcing
2. **Machine pre-qualification** — use AI + rule-based screening to reduce to ~3000 candidates
3. **Human-AI hybrid deep qualification** — score each of 3000 against Federer criteria to arrive at 1000 qualified prospects

Expected yield: 8000 raw → 3000 pre-qualified → 1000 ICP-qualified (12.5% final yield — consistent with the 30% stated in the assignment, applied twice through a two-stage filter)

---

## Week-by-Week Plan

### Week 1: Build the Raw Universe (Target: 8000 companies)

**Day 1-2: Set up data infrastructure**
- Write Python script to pull BSE/NSE company list from Screener.in API (or scrape systematically)
- Set up Tofler Pro account (or use Zauba Corp free tier)
- Download DSIR recognition list, USFDA India establishment list, Pharmexcil member list
- Get API access to LinkedIn (or set up Sales Navigator with boolean templates)

**Day 3-5: Bulk data sourcing**

Source 1 — **Screener.in scrape** (all BSE/NSE listed companies in target sectors):
- Industries: Healthcare Equipment, Pharmaceuticals, Agrochemicals, Food Products
- Market cap filter: Rs.30Cr–Rs.3000Cr (conservative, will refine)
- Expected yield: ~800 listed companies

Source 2 — **MCA/Tofler NIC code extract** (private companies):
- NIC codes: 2100, 2109, 3250, 0111, 2106, 2120, 2090 (specialty chemicals adjacent)
- States: MH, TG, GJ, KA, TN, MP, UP, PB, RJ, WB
- Revenue filter: Rs.20Cr–Rs.600Cr (slightly wider than ICP — will narrow in Stage 2)
- Expected yield: ~5000 companies

Source 3 — **Trade expo exhibitor lists** (manual + semi-automated):
- CPhI India, AIMED Expo, Medica India, Analytica India, Poultry India, Krishi Unnati Mela
- Extract exhibitor tables from PDF catalogs using Python (pdfplumber or Tabula)
- Expected yield: ~1000 unique companies not in Tofler data

Source 4 — **USFDA India establishment list + DSIR list**:
- Direct download and parse
- Expected yield: ~800 companies (significant overlap with sources above — deduplication removes ~500)

Source 5 — **LinkedIn scrape via Sales Navigator or Phantombuster**:
- Boolean search for company type by industry + city + headcount
- Expected yield: ~1500 companies (after deduplication)

**Total after deduplication: ~8000-9000 raw companies**

**Day 6-7: Deduplication and basic cleaning**
- Python dedup on company name + CIN number
- Remove companies with no website (auto-disqualify)
- Remove obviously large companies (Tata, Reliance, Sun Pharma — by name match)

---

### Week 2: AI-Powered Pre-Qualification (Target: 3000 companies)

**Approach:** Use Claude (via API) with a structured prompt to evaluate each company against E1, E2, and a quick C3/C5 proxy — reducing 8000 to ~3000.

**Step 1: Enrich company data**
For each company in the raw list, use a Python script to:
- Scrape the company website homepage and "about" page (using requests + BeautifulSoup)
- Extract: what they make, city, any certification mentions (ISO, USFDA, EU-GMP, DSIR), any R&D mentions
- Pull basic financial data from Tofler (revenue band, year-on-year change)

**Step 2: Claude API batch scoring**

Prompt template sent to Claude API for each company:
```
Company: [name]
Website about-page text: [scraped text]
Revenue band: [from Tofler]
City/state: [from MCA]

Based on the above, evaluate:
1. E1 (Producer gate): Does this company produce products in-house? (YES/NO/UNCLEAR)
2. E2 (City): Is primary operational presence in India? (YES/NO)
3. Auto-disqualify: Is this a generic pharma company, MNC subsidiary, or PE-owned? (YES/NO/UNCLEAR)
4. C3 proxy: Is there evidence of technical differentiation (certifications, patents, specialized equipment, proprietary products)? (STRONG/MODERATE/WEAK/NONE)
5. C5 proxy: Is this sector experiencing growth tailwinds (PLI, export markets, China+1)? (YES/NO)

Return JSON: {"e1": "YES/NO/UNCLEAR", "e2": "YES/NO", "auto_disqualify": "YES/NO/UNCLEAR", "c3_proxy": "STRONG/MODERATE/WEAK/NONE", "c5_proxy": "YES/NO"}
```

**Pre-qualification filter:** Keep companies where:
- E1 = YES or UNCLEAR (don't discard UNCLEAR yet — human reviews in Week 3)
- E2 = YES
- auto_disqualify = NO or UNCLEAR
- c3_proxy = STRONG or MODERATE
- c5_proxy = YES

**Expected yield:** ~3000-3500 companies pass this filter (out of 8000)

**Step 3: Quality check sample**
Manually verify 200 random companies from the pre-qualified list. Measure false positive rate (companies that passed AI filter but would fail human review). Adjust Claude prompt if false positive rate > 20%.

---

### Week 3: Deep Scoring (Target: Score 3000 companies, identify top 1500)

**Approach:** For 3000 pre-qualified companies, run a deeper enrichment + AI scoring pass for all 6 Federer criteria.

**Enrichment per company (automated):**
- LinkedIn company page scrape: employee count trend, recent job postings (SAP/ERP mentions), leadership names/titles
- LinkedIn decision-maker search: founder/MD profile — education (IIT/NIT/BITS/PhD), career history
- Google news search (SerpAPI or similar): last 18 months mentions — facility expansion, new certifications, new product launches, export wins
- MCA director data: recent director appointments (proxy for succession/gen-2 join date)

**Scoring pass:** Claude API with enriched data, scoring C3–C8 as Weak/Moderate/Strong for each criterion, summing to Federer score.

**Output:** A scored list of 3000 companies with Federer scores from 0–100.

**Quality control — human review triggers:**
- Any company with C7 = Strong AND C4 = Weak (unusual — flag for human review)
- Any company with revenue band > Rs.400Cr (near ceiling — manual revenue verification)
- Any company with "UNCLEAR" on E1 or auto-disqualify

**Cut-off:** Keep companies scoring ≥ 55 (C-band and above) → expect ~1500 companies

---

### Week 4: Final Qualification + Verification (Target: 1000 verified ICP companies)

**Goal:** Reduce 1500 scored companies to 1000 with verified data points.

**Step 1: Spot-verification of top 1500**
For each of 1500 companies, verify 3 critical data points:
- Confirm website is active and not a placeholder (automated — status code check)
- Confirm revenue band is in range (Tofler cross-check — flag if >Rs.500Cr)
- Confirm not recently acquired by PE or larger group (Google news search: "[company name] acquisition" in last 12 months)

**Step 2: Hard disqualification pass**
- Revenue confirmed > Rs.500Cr → remove (expect ~150 companies to be eliminated here as fast-growing companies that crossed the ceiling)
- Website inactive → remove
- Recent PE acquisition confirmed → remove

**Step 3: Personalization hook generation**
For each of the 1000 surviving companies, use Claude API to generate a personalization hook (1-2 sentence specific detail for outreach email line 1) — same format as the assignment's company profiles.

**Step 4: Final quality audit**
Random sample 100 companies from the final 1000. Manually verify:
- E1 status
- Revenue band
- Federer score accuracy (C3–C8)
- Personalization hook accuracy

Target: >85% accuracy on manual verification. If below 85%, iterate on Claude prompts.

---

## Summary: Expected Yield at Each Stage

| Stage | Companies | Action |
|-------|-----------|--------|
| Raw universe | 8,000–9,000 | Data collection + dedup |
| After AI pre-qualification | ~3,000 | E1/E2/auto-disqualify + C3/C5 proxy |
| After deep scoring | ~1,500 | Full C3–C8 Federer scoring |
| After verification | **~1,000** | Revenue confirm + activity check |

---

## Tools Required

| Tool | Purpose |
|------|---------|
| Python (requests, BeautifulSoup, pandas) | Web scraping, data cleaning, deduplication |
| Tofler Pro | Private company financial data (NIC code + revenue extract) |
| Claude API (Anthropic) | AI-powered batch scoring at each stage |
| LinkedIn Sales Navigator | Decision-maker discovery and education background |
| SerpAPI / Google Search API | News search for growth signals per company |
| Phantombuster | LinkedIn company data extraction at scale |
| Screener.in | Listed company screening with financial filters |
| USFDA Establishment Database | Free — direct download from FDA.gov |
| DSIR Recognition List | Free — dsir.gov.in |
| Pharmexcil member directory | Free — pharmexcil.com |

---

## Quality Control Philosophy

The key risk in this process is **false positives** — companies that score well in AI screening but turn out to be traders, MNC subsidiaries, or revenue-misclassified on deeper check. My quality control approach is:

1. **Sample and calibrate at each stage** — before moving from one stage to the next, manually verify 100-200 random outputs and measure error rate. Adjust AI prompts if error rate > 15%.

2. **Conservative thresholds on ambiguous signals** — when Claude marks a company UNCLEAR on E1 or auto-disqualify, route to human review rather than defaulting to pass or fail.

3. **Revenue verification at the end** — revenue data from Tofler can be 1-2 years old. Fast-growing companies in hot sectors (defence, biotech, diagnostics) may have crossed Rs.500Cr since the last filing. Always cross-reference the most recent press release or annual report for companies scoring > 70 in the Federer band to confirm they're still within the ICP range.

4. **Two-person spot check on final 1000** — before the list is considered "submission-ready," a second analyst should independently verify 100 randomly selected companies. Agreement > 85% = list is ready. Below 85% = return to scoring and recalibrate.
