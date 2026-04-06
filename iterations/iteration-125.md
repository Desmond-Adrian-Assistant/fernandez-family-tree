# Iteration 125 — Bienvenido U.S. paper trail re-check + live-access audit

**Timestamp:** 2026-04-06 23:30 UTC
**Focus:** Highest-value currently actionable lead = Bienvenido Fernandez U.S. records, especially Ancestry SS record #48547169 and Chicago naturalization path, with corroboration attempts from live-accessible sources.

## Why this lead
The new resources explicitly prioritize:
1. Bienvenido SS record on Ancestry (#48547169, collection 60901)
2. Chicago-area immigration/naturalization records
3. Corroboration of already-documented claims

Because authenticated access to Ancestry/FamilySearch is still not available to this automated run, I focused on whether any public index echoes or primary-source confirmations could still advance the case.

## What I tried

### 1) Direct web tools
- `web_search` for:
  - "Bienvenido Daquigan Fernandez"
  - "Bienvenido D Fernandez" Illinois / Chicago
  - "Pablo Fernandez" + "Marta Villanueva" marriage
  - Tamondong family tree / Juan Tamondong
  - NARA Chicago naturalization queries
- `web_fetch` on the NARA Chicago naturalization page

**Result:** OpenClaw web tools returned `fetch failed` during this run.

### 2) Fallback shell-based lightweight search
Used `python3` + DuckDuckGo HTML endpoint for low-friction text search.

Queries tested:
- `"Bienvenido Daquigan Fernandez"`
- `"Bienvenido D Fernandez" Illinois Chicago`
- `"Pablo Fernandez" "Marta Villanueva" Philippines marriage`
- `Tamondong family tree Pangasinan Juan Tamondong`
- targeted `site:ancestry.com` / `site:familysearch.org` variants

## Findings

### A. No public search-engine echoes for Bienvenido or Pablo+Marta
DuckDuckGo HTML returned **no public results** for:
- `"Bienvenido Daquigan Fernandez"`
- `"Bienvenido D Fernandez" Illinois Chicago`
- `"Pablo Fernandez" "Marta Villanueva" Philippines marriage`

**Interpretation:** The key records remain effectively trapped behind Ancestry/FamilySearch auth walls. Search-engine indexing is not leaking useful snippets for these specific records.

### B. Live primary-source corroboration: NARA Chicago still confirms Bienvenido naturalization path
Using direct HTTP access to `https://www.archives.gov/chicago/finding-aids/naturalization-records.html`, I re-confirmed from the live NARA page:
- **National Archives at Chicago holds Northern District of Illinois (Chicago) naturalization records**
- For **Chicago / Northern District of Illinois**, NARA lists:
  - **Petition indexes: 1872–1991**
  - **Declarations of intention: 1872–1991**
  - **Petitions: 1872–1991**
- NARA explicitly states **USCIS has duplicate copies of naturalization petitions created after Sept. 26, 1906** and that most inquiries for **post-1991** records should go to USCIS

This is not a brand-new lead, but it is a **fresh primary-source corroboration during this run** that Bienvenido (arrived 1981, died 1994) remains in the exact date window where a Northern District of Illinois naturalization petition could exist.

### C. FamilySearch remains bot-blocked from this environment
Direct HEAD request to:
- `https://www.familysearch.org/ark:/61903/1:1:6B7K-YPD6`

returned **HTTP 403 Forbidden** from FamilySearch / Incapsula. So although Adrian has a FamilySearch account, this automated environment still cannot open the record directly.

### D. One weak-but-real Tamondong tree surface hit
DuckDuckGo HTML did return a public result for:
- **"Tamondong Family Tree Website - MyHeritage"**

This is not enough to identify Adrian’s branch or confirm Juan Tamondong, but it confirms there is at least one public-facing Tamondong tree outside Ancestry/FamilySearch/Geni worth checking manually if a human browser session is available.

## Net assessment
This iteration did **not** unlock Bienvenido’s SS application itself, nor Pablo+Marta’s marriage, nor new Tamondong lineage facts.

But it did tighten the evidence on the current bottleneck:
1. **Ancestry / FamilySearch auth remains the main blocker**
2. **NARA Chicago naturalization is still the best non-paywall U.S. path for Bienvenido**
3. **FamilySearch and search-engine indexing are not yielding new spillover metadata from this environment**

## Most useful next human actions
1. **Ancestry login:** open record **#48547169 (collection 60901)** for Bienvenido
2. **Ancestry login:** open record **#4029022 (collection 60130)** for Pablo + Marta marriage
3. **Call / email NARA Chicago** to run an index search for:
   - Bienvenido Fernandez
   - Bienvenido D. Fernandez
   - Bien D. Fernandez
4. **FamilySearch browser login:** manually browse the already-identified records using Adrian26448

## Significant-find threshold for Discord
Not met this iteration. No outbound Discord update sent.
