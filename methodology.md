# Research Methodology
## DT Business Analytics Assignment — Pune, Basket B
**Prepared by:** Mahak (GitHub: mahak19m)
**Date:** May 2026

---

## City & Segment Selection

### City: Pune
**Justification:** Pune is one of India's strongest cities for Basket B research for three structural reasons:
1. **Life sciences cluster density** — Pune has Hinjewadi (IT + biotech), Chakan (manufacturing), and Lonavala/Pimpri-Chinchwad (pharma/chemical plants). The city has a critical mass of USFDA-approved plants, IVD manufacturers, and specialty pharma companies.
2. **Academic and R&D backbone** — CSIR-NCL (National Chemical Laboratory), Serum Institute, and multiple pharmaceutical R&D centers create spillover companies and spin-offs that fit the Federer profile.
3. **Promoter-driven mid-size manufacturing** — unlike Mumbai (too many large corporates and HQ offices) or Hyderabad (heavy Pharma City concentration), Pune has a healthy density of Rs.50-500Cr founder-led manufacturers.

**City boundary applied:** I counted companies with HQ, primary R&D, or primary manufacturing in Pune district including Pimpri-Chinchwad, Hinjewadi, Lonavala, and Bhosari MIDC. Companies with only a sales office in Pune were excluded.

### Segment: Basket B
Segments researched:
- **Medical devices** (IVD platforms, implants, surgical instruments) — strongest density in Pune
- **Complex APIs and regulated pharma** (sterile injectables, specialty formulations — NOT generic bulk APIs)
- **Specialty food and nutraceutical ingredients** (enzymes, probiotics, Vitamin D3, botanical extracts)
- **Animal health and veterinary biologics** (feed additives, veterinary ingredients)
- **Hybrid seeds and specialty agri-inputs** (hybrid seed R&D, biopesticides — limited Pune presence)

---

## Research Process

### Phase 1: Universe Generation (75-100 companies)

**Sources used in order of signal quality:**

1. **Screener.in** — Used to find BSE/NSE listed companies with Pune headquarters. Filtered by market cap (Rs.50Cr–Rs.3000Cr as proxy for revenue range), then manually checked each against Basket B sector tags. Key search: "Maharashtra healthcare," "Maharashtra medical devices," "Maharashtra specialty pharma."

2. **MCA/Tofler** — For private (unlisted) companies, searched Tofler for Pune-registered companies in NIC codes:
   - 2100 (pharmaceutical products)
   - 2109 (other pharmaceutical products — includes specialty ingredients)
   - 3250 (medical instruments and devices)
   - 0111 (seed crops — for agri-inputs)
   Filtered by revenue range and sorted by EBITDA to find growing companies.

3. **Built In Pune (builtinpune.in)** — Curated list of biotech, healthtech, and pharma companies in Pune with basic company descriptions. Used as a discovery layer before deeper verification.

4. **MCCIA (Mahratta Chamber of Commerce)** — Industry association membership list for Pune manufacturers. Useful for finding non-listed, privately held manufacturers that don't appear in Screener or Tofler.

5. **LinkedIn Company Search** — Searched "medical devices Pune," "specialty pharma Pune," "nutraceutical ingredients Pune" with employee count filters (50–2000 employees as proxy for Rs.50-500Cr revenue range). Verified hiring activity and job posting density.

6. **IndiaMart and Indiamart Manufacturer Listings** — Used specifically for nutraceutical and agri-input segment where many companies are unlisted and don't appear in financial databases. Filtered for "Manufacturer" type (not trader/distributor) with Pune address.

7. **BIRAC (Biotechnology Industry Research Assistance Council) grant database** — Public list of BIRAC-funded companies; used to find science-founder companies (PhD-founded biotech/agri startups) in Pune region with early evidence of IP.

8. **Export Import Data (DGFT portal)** — Searched IEC codes for Pune-address companies exporting under HS codes for medical devices (9018–9022), pharmaceutical APIs (2934–2941), and food ingredients (2106, 3302) in the Rs.50Cr+ range. Export activity is a C6 growth signal and also signals regulatory maturity.

---

### Phase 2: First-Pass Filtering (E1 + E2 gates)

For every company found in Phase 1, I applied two quick filters before spending time scoring:

**E1 check:** Does the company have its own plant/facility/manufacturing infrastructure?
- Method: Check the website for "manufacturing," "plant," "facility," or "our products." Cross-check IndiaMart listing type (Manufacturer vs Trader). Check MCA NIC code.
- Eliminated: analytical instrument resellers, pharma marketing companies, CROs, hospital chains, testing labs.

**E2 check:** Is the primary operational presence in Pune (not just registered office)?
- Method: Cross-check website "contact us" address vs MCA registered office address. For listed companies, check annual report facility details.
- Eliminated: Companies with only Pune sales offices (Alkem, Lupin, etc.), Delhi/Mumbai HQ companies with Pune distribution only.

**Auto-disqualifiers applied:**
- Revenue > Rs.500Cr: Eliminated Serum Institute, Lupin, Wockhardt, Syngene (Biocon subsidiary)
- PE/VC ownership: Eliminated Aragen (GHO Capital), any recent PE-acquired company
- MNC subsidiaries: Eliminated Thermo Fisher India, Ajinomoto India, MSD Animal Health India
- Generic/bulk pharma: Eliminated companies primarily making generic tablets, branded generics, or commodity APIs

---

### Phase 3: Deep Scoring

For each company that passed E1 + E2, I researched each criterion:

**C3 (Differentiated):**
- Checked patents on Indian Patent Office database
- Checked DSIR recognition list (DSIR website publishes recognized R&D labs)
- Checked USFDA warning letter database (absence + inspection history confirms compliance)
- Checked for "first in India," "only in India" claims with corroborating third-party sources

**C4 (Decision-Maker Quality):**
- LinkedIn founder/MD profiles for education and career background
- MCA director listing for appointment dates (to verify gen-2 appointments)
- Press/interview mentions of ERP, SAP, structured costing language

**C5 (Growing Sector):**
- PLI scheme eligibility list (Ministry of Pharmaceuticals, Ministry of Food Processing)
- Ministry of Commerce export data by HS code
- Industry reports (IBEF, CARE Ratings) for sector-level tailwind confirmation

**C6 (Growth Signals):**
- LinkedIn job postings (last 6 months filter) — counted open roles
- Company press releases/news section on website
- Tofler revenue trend (year-over-year for last 2-3 years where available)

**C7 (Systems Maturity):**
- LinkedIn job postings mentioning SAP/ERP/Oracle
- LinkedIn employee profiles with SAP/ERP skills in the company
- USFDA/EU-GMP approval (strong proxy — compliance requires batch record systems equivalent to ERP)
- Annual reports mentioning IT infrastructure investments

**C8 (Leadership Succession):**
- MCA director list with appointment dates
- LinkedIn company page for C-suite other than founder
- Press coverage of promoter transition or professional management appointment

---

## What I Learned About the Pune Basket B Landscape

**Key findings:**

1. **Regulated pharma is the strongest Basket B segment in Pune.** Pune has a disproportionate number of USFDA + EU-GMP approved manufacturers (Indoco, Emcure, Marksans plant, Gennova) compared to most Indian cities outside Hyderabad. This is the highest-signal Basket B segment here.

2. **Medical devices is improving but concentrated.** IVD (Mylab, Gennova) is strong; orthopedic implants (Biorad Medisys) exist but are private. Large device MNCs (Philips, Siemens, Becton Dickinson) have Pune offices but are not ICP targets.

3. **Nutraceutical ingredients are underrepresented in databases.** Many specialty enzyme and probiotic manufacturers in Pune are unlisted and don't appear on Screener — IndiaMart and direct manufacturer directories were essential for finding them (Hi Tech BioSciences, Zytex).

4. **Agri-inputs are mostly outside Pune proper.** Hybrid seed companies (Nath Bio-Genes, Maharashtra Hybrid Seeds) and biopesticide startups (Bioprime) exist in the Pune region but their operations tend to be in Aurangabad, Nashik, or rural Maharashtra — not Pune city. This segment had a high E2 failure rate.

5. **The 30% yield estimate is accurate.** From approximately 80 companies investigated, approximately 25 passed all gates. Major failure modes:
   - Revenue > Rs.500Cr (eliminated ~15 companies including Serum, Lupin, Wockhardt, Syngene)
   - MNC subsidiary (eliminated ~10 companies)
   - E1 failure — service company or trader (eliminated ~10 companies)
   - E2 failure — city mismatch (eliminated ~8 companies)
   - PE-owned (eliminated ~3 companies)
   - Insufficient activity / stale company (eliminated ~5 companies)

---

## Confidence and Limitations

**High confidence scores:** Indoco Remedies, Emcure Pharmaceuticals, Gennova Biopharmaceuticals, Mylab Discovery — all verified through multiple public sources (annual reports, regulatory databases, press coverage).

**Moderate confidence scores:** Biorad Medisys, Fermenta Biotech, Hi Tech BioSciences — operational evidence is strong but financial data and systems maturity required direct verification (private companies with limited public filings).

**Low confidence / borderline:** Aaroha Lifesciences, Fermentech India — limited public data; included as borderline with recommendation for direct verification before active outreach.

**What I would do with more time:**
- Call each company's listed landline to verify operational presence
- Pull full Tofler financial reports (paid) for revenue verification
- Use LinkedIn Sales Navigator for deeper decision-maker profiling
- Cross-reference USFDA inspection database for all pharma companies to verify approval status currency
