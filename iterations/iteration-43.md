# Iteration 43 — Eduardo's Spouse Confirmed + Catalina Search + Search API Exhausted

**Timestamp:** 2026-03-31 10:53 UTC (5:53 AM CDT)
**Focus:** Pablo & Marta's children corrections, Tamondong Geni profiles, Catalina Fernandez deep search
**Trigger:** Cron job v2, priority (b) Tamondong family trees + (c) Pablo & Marta children

## Key Finding: Iluminado Bautista = Eduardo's SPOUSE (CORRECTION)

### Previous Understanding (Iteration 41-42)
- Iteration 41 listed "Iluminado" as a "NEW Name (Relationship Uncertain)" — possibly another sibling
- Iteration 42 theorized the third name on marriage records = spouse, noted Iluminado's masculine name as "odd for wife"

### Corrected Finding
The Ancestry search results page for `father=Pablo_Fernandez&mother=Marta_Villanueva` displays the record fields **explicitly**:

```
Name: Eduardo Fernandez
Spouse: Iluminado Bautista
Mother: Marta Villanueva
Father: Pablo Fernandez
```

**Iluminado Bautista is unambiguously Eduardo's SPOUSE** — confirmed by the field label "Spouse" on the Ancestry search preview.

### About the Name "Iluminado"
- "Iluminado/a" in Filipino Spanish tradition can be either masculine OR feminine
- The feminine form **"Iluminada"** exists, but OCR/indexing may have dropped the final -a
- Full name pattern: **Iluminado/Iluminada Bautista** married Eduardo Fernandez (son of Pablo + Marta)
- **Bautista** = very common Filipino surname (from Spanish "Baptist"), suggesting a mainstream Pangasinan family

### Updated Pablo & Marta Villanueva Family (Corrected)
1. **Josefa Fernandez** (b. 1901) — married **Ildefonso [surname unknown]** (Ancestry record 665092)
2. **Eduardo Fernandez** (b. 1903) — married **Iluminado/a Bautista** (Ancestry record 1346541)
3. **Mariano Fernandez** (b. 1905) — married (1st) Victoria Daquigan; (2nd) Dionicia Capinding (Ancestry record 3179793)
4. **Catalina Fernandez** (b. ~1895-1910) — married [spouse unknown] (Ancestry record 1085806)

**Iluminado is NOT a sibling** — corrects iteration 41/42 speculation.

## Catalina Fernandez Marriage Record — Still Behind Paywall

- Ancestry record 1085806 (collection 60130: Philippines, Select Marriages)
- Search preview confirms: first result for `Catalina Fernandez + father Pablo Fernandez + mother Marta Villanueva`
- Marriage date, marriage place, and spouse name all redacted (xxxxx pattern)
- **Requires Adrian's Ancestry World Explorer login to view full details**
- Among ~20 "Catalina Fernandez" marriages in the Philippines collection, record 1085806 is the ONLY match for Pablo/Marta parentage

## Josefa Fernandez — Second Marriage Record Identified?

- Ancestry record #3773825 appeared in fuzzy search for Josefa Fernandez
- When searching with exact match on parent names, returns zero — confirming this is a DIFFERENT Josefa Fernandez
- The correct record remains #665092 ("Josefa Fermandez" — OCR misspelling), married Ildefonso

## Geni Juan & Luis Tamondong — Blocked

- Geni profile IDs confirmed: Juan=6000000016169609747, Luis=6000000016169609781
- Geni.com blocks web scraping — returns empty HTML
- **Requires a Geni.com login to view profile details** (dates, parents, locations, children)
- Action item: Adrian should create a free Geni account or use existing Google login to access these profiles

## FamilySearch — Blocked (JS-Required)

- FamilySearch tree pages and search results require JavaScript rendering
- Cannot access Pablo Fernandez (GW9H-MP7) or Tamondong search results via web_fetch
- **Requires login-based browser access** — Adrian's FamilySearch account (Adrian26448) has access

## FindAGrave Results

- **Bienvenido Fernandez + Illinois + 1994 death**: Still NO match (not cataloged)
- **Tamondong + Illinois**: Zero results — previously identified Des Plaines burial may have been from a different search path
- **Catalina Fernandez + Pangasinan**: 31 results, one in Calasiao, Pangasinan — but the search location filter actually returns worldwide results (FindAGrave quirk). The Calasiao result needs individual memorial investigation.
- **Abalos + Pangasinan**: 776 results including Calasiao (×3), Binmaley (×2), Aguilar (×2), San Fabian — confirms broad Abalos presence across Pangasinan

## Search API Quota Exhausted

- Brave Search API returned 429 (quota exceeded: 2001/2000)
- Web search unavailable for remainder of this iteration
- All research conducted via direct URL fetches to Ancestry, FindAGrave, Geni, FamilySearch, WikiTree, bonarae.net

## WikiTree Tamondong — Empty

- WikiTree has a page for the Tamondong surname but no actual profiles

## Newspapers.com — Behind Paywall

- "Bienvenido Fernandez" + Chicago (1990-1995): 0 results
- "Tamondong Pangasinan" (1900-1960): 0 results
- Both require paid Newspapers.com subscription to view any results

## PVAO (Philippine Veterans Affairs) — Blocked

- `collections.pvao.mil.ph` connection failed (likely Cloudflare protection)
- Cannot search Mariano Fernandez WWII records online

## Summary of Actionable Items for Adrian

1. **🔴 HIGH: Log into Ancestry** — View these records:
   - Bienvenido SS record #48547169 (collection 60901) — full birth/death dates, parents, SSN
   - Catalina Fernandez marriage record #1085806 (collection 60130) — spouse name, date, location
   - Josefa Fernandez marriage record #665092 — confirm Ildefonso's full surname
   - Ancestry tree #68186126 — may contain new family members
   - Eduardo Fernandez marriage record #1346541 — confirm marriage date/place, "Iluminada" spelling

2. **🟡 MEDIUM: Log into Geni.com** — View Juan Tamondong profile (6000000016169609747) for dates, parents, children

3. **🟡 MEDIUM: Log into FamilySearch** — Browse Pangasinan civil registration images for Tamondong records

## Searches Performed
1. Geni.com Juan Tamondong profile (blocked - JS required)
2. Geni.com Luis Tamondong profile (blocked - JS required)
3. FamilySearch tree GW9H-MP7 Pablo Fernandez (blocked - JS required)
4. FamilySearch Tamondong birth search (blocked - JS required)
5. Ancestry Bienvenido SS record (redirect to login)
6. FindAGrave Tamondong + Illinois (0 results)
7. Fold3 Mariano Fernandez (Cloudflare blocked)
8. Newspapers.com Tamondong Pangasinan (0/paywall)
9. Newspapers.com Bienvenido Chicago (0/paywall)
10. FindAGrave Catalina Fernandez Pangasinan (31 results, 1 in Calasiao)
11. FindAGrave Bienvenido Fernandez Illinois 1994 (0 results)
12. FindAGrave Fernandez + Calasiao (36,885 fuzzy)
13. FindAGrave Abalos + Pangasinan (776 results)
14. bonarae.net genealogy pages (site restructured, genealogy pages broken)
15. WikiTree Tamondong (no profiles)
16. Ancestry Pablo+Marta children search → **Eduardo married Iluminado Bautista (confirmed spouse)**
17. Ancestry Catalina Fernandez + Pablo/Marta (record 1085806 confirmed, behind paywall)
18. Ancestry Josefa Fernandez + Pablo/Marta exact (0 exact matches — confirms 665092 is fuzzy match)
19. PVAO Philippine veterans search (connection failed)
20. MyHeritage Tamondong (failed to load)
21. Catholic Cemeteries Chicago (Cloudflare blocked)
