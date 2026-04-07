# Iteration 129 — Live NARA Corroboration Pass: Mariano WWII + Chicago Naturalization (2026-04-07 02:16 UTC)

## Focus
Use directly reachable NARA pages to corroborate the highest-value public leads still available from this environment:
1. **Mariano Fernandez WWII path**
2. **Bienvenido Fernandez Chicago naturalization path**
3. **Tamondong/Mapandan corroboration**

## Methods
Because `web_search` / `web_fetch` have been unreliable and DuckDuckGo HTML is now challenge-gated, this iteration used direct HTTP fetches against NARA pages from the shell.

### Live pages checked
- `https://www.archives.gov/chicago/finding-aids/naturalization-records.html`
- `https://www.archives.gov/research/military/ww2/philippine/guerrilla-list-1.html`
- `https://www.archives.gov/research/military/ww2/philippine/guerrilla-list-2.html`
- `https://www.archives.gov/research/military/ww2/philippine/guerrilla-list-3.html`

## Findings

### 1) NARA Chicago naturalization path re-confirmed from live page
The NARA Chicago naturalization finding-aid page was directly reachable and still explicitly states that for **Illinois, Northern District, Chicago** the archive holds:
- **Petition indexes: 1872-1991**
- **Declarations of intention: 1872-1991**
- **Petitions: 1872-1991**

The same live page also explicitly states that **USCIS holds duplicate copies of post-1906 naturalization petitions** and that most post-1991 inquiries should go to USCIS.

**Implication:** Bienvenido Fernandez's reported 1981 Chicago arrival still sits squarely inside a live, directly corroborated naturalization search window.

### 2) Mariano WWII file path tightened from official NARA guerrilla-unit lists
The live NARA guerrilla unit pages directly corroborated all three major file paths already suspected for Mariano Fernandez's wartime area:

- **HQ Tarlac Military Area, LGAF — file 102-22**
- **AIB, Tarlac West Sector — file 304**
- **1st Mapandan Co. (Independent) — file 202**

These were all extracted from the official NARA guerrilla lists during this run.

### 3) Army of the Agno path re-confirmed from live NARA lists
The same live guerrilla lists again confirm the Pangasinan-side path:
- **Army of the Agno, 1st Organized Pangasinan Corps, Fil-American Guerrillas — file 185-1**
- Other Army of the Agno sub-files remain visible on the list as expected (for example later 185-series entries)

This matters because Mariano's life bridged **Gerona, Tarlac** and the wider **San Carlos / Pangasinan** network, so the current best WWII request bundle is still:
- **102-22** (HQ Tarlac Military Area, LGAF)
- **304** (AIB, Tarlac West Sector)
- **202** (1st Mapandan Co. (Ind))
- **185-series** (Army of the Agno)

## Negative / limiting results
- DuckDuckGo HTML fallback still returns **HTTP 202 challenge pages**, not usable public search results.
- No direct online NARA name hit for **Mariano Fernandez** was found in this run.
- No new genealogical person/date/place facts were unlocked beyond the documentary corroboration above.

## Operational conclusion
This iteration did **not** produce a new ancestor identity or date.
But it did strengthen the project in a useful way:
- The **Chicago naturalization** path for Bienvenido is still live and clearly documented from a primary source.
- The **Mariano WWII request packet** can now be stated with even higher confidence using live NARA corroboration for:
  - **102-22**
  - **304**
  - **202**
  - **185-series**

## Best next actions
1. **Manual Ancestry #48547169** — Bienvenido SS application
2. **Manual Ancestry #4029022** — Pablo Fernandez + Marta Villanueva marriage
3. **NARA Chicago index lookup** for Bienvenido naturalization
4. **SF-180 / archive request for Mariano** citing files **102-22, 304, 202, and 185-series**
