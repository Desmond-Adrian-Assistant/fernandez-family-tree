# Iteration 62: NARA NUMIDENT Search + Ancestry/FamilySearch Blockers Assessment

**Timestamp:** 2026-04-03 15:05 UTC (10:05 AM CDT)
**Focus:** Priority (a) Bienvenido SS record access + NARA NUMIDENT free database search + Assessment of all blocked resources
**Searches performed:** ~25

## Key Finding: NARA NUMIDENT Database — FREE but Bienvenido NOT Found

### What is NUMIDENT?
The NARA Access to Archival Databases (AAD) at aad.archives.gov hosts the Social Security NUMIDENT files — the same underlying data as Ancestry's Collection 60901 — **completely FREE**. The database contains:
- **Application (SS-5) Files, 1936-2007**: Full name, DOB, place of birth, father's name, mother's maiden name
- **Death Files, 1936-2007**: Name, DOB, DOD, residence ZIP code
- **Claim Files, 1936-2007**: Benefit claims

### Search Results
| Database | Search Terms | Results |
|----------|-------------|---------|
| NARA Death Files (E-G) | BIENVENIDO + FERNANDEZ | **0 of 5,246,105** |
| NARA Application Files (E-G) | BIENVENIDO + FERNANDEZ | **0 records** |

### Why Bienvenido May Be Missing from NUMIDENT
1. **Late SSN issuance**: Bienvenido arrived in the US in 1981 and died in 1994 — only 13 years in the US. His SSN may have been issued late or through a non-standard process.
2. **Name spelling variations**: The records may list him as "BIEN", "BIENUENDO", or "BEN" (known alternate spellings from previous Ancestry searches).
3. **Incomplete coverage**: NUMIDENT doesn't contain ALL Social Security records — the FAQ explicitly states "These files do not contain records of all deaths."
4. **The Ancestry record #48547169 exists in collection 60901** — this is the same NUMIDENT data but Ancestry may have a more complete version or different processing. The NARA public version may be a subset.

### 🔴 Critical Realization: Ancestry Paywall = #1 Blocker for ALL Remaining Research

The following 20+ records ALL require Adrian's Ancestry World Explorer login:

#### Highest Priority (red)
| Record ID | Collection | Person | Contains |
|-----------|-----------|--------|----------|
| 48547169 | 60901 (SS Apps) | Bienvenido | **Birth date, death date, SSN, father's name, mother's maiden name** |
| 4029022 | 60130 (Marriages) | Pablo + Marta | Their OWN marriage record — may reveal Pablo's parents (one generation further back!) |
| 1085806 | 60130 (Marriages) | Catalina Fernandez | New sibling's spouse name, marriage date/place |
| 1165555 | 60130 (Marriages) | Aniceto Fernandez | New sibling's spouse, confirmed same register as Pablo (#1165552) |
| 1090125 | 60130 (Marriages) | Hilario Abalos | Marriage details + parents |
| 2494854 | 60130 | Cosme Abalos | Aurea's sibling |
| 2494041 | 60130 | Maria Abalos | Aurea's sibling |
| 68186126 | Ancestry Trees | Bienvenido | Second family tree from different contributor |

#### Medium Priority (yellow)  
- Records for Aurea's other 5 siblings (Feliciana, Francisco, Dominador, Marina, Maria R.)
- Pablo's death 1955 (#1575015), Marta's death 1955 (#362831)
- SSDI records for "A.B. Fernandez" (#18996711) and "B. Fernandez" (#18998749) — 1994 Illinois deaths

### Other Blocked Resources (unchanged)
| Resource | Issue | Status |
|----------|-------|--------|
| FamilySearch tree/records | Requires login (Adrian26448 account exists) | Blocked for web_fetch |
| Catholic Cemeteries Chicago | Cloudflare anti-bot | Blocked |
| Geni.com profiles | Incapsula anti-bot | Blocked |
| PVAO guerrilla records | Site inaccessible | Blocked |
| FamilySearch Cook County Deaths | Requires auth | Blocked |

### Searches That Returned 0 Results
- "Pablo Fernandez" "Marta Villanueva" marriage Philippines
- "Mariano Fernandez" WWII guerrilla Pangasinan Tarlac
- SSDI "Bienvenido" Fernandez death 1994 Illinois
- "Hilario Abalos" "Filomena Rosario" Philippines
- FamilySearch "Carlina Tamondong" OR "Jose Abalos"

### New Resource Discovered: NARA NUMIDENT (Free)
Even though Bienvenido wasn't found, the NARA AAD NUMIDENT database at aad.archives.gov/aad/series-description.jsp?s=5057 is a FREE alternative to Ancestry for searching ~97 million deceased persons' Social Security records. Could be useful for:
- Searching for Jose B Daquigan (d. 1991) 
- Searching for Francisco M Daquigan (d. 1970)
- Searching for other family members

### Steve Morse One-Step SSDI Tool
stevemorse.org/ssdi/ssdi.html provides a free aggregated SSDI search across multiple databases (Ancestry, FamilySearch, GenealogyBank, MyHeritage, cancelthesefunerals). However, it requires JavaScript rendering — cannot be used via web_fetch.

## Assessment: Project Status at 62 Iterations

**All online research avenues for the Fernandez-Cervantes family tree are effectively EXHAUSTED without:**
1. **Adrian logging into Ancestry World Explorer** to unlock 20+ critical records
2. **Adrian logging into FamilySearch (Adrian26448)** to access Cook County Deaths + parish records
3. **Physical actions**: Ordering Cook County death certificate ($17), visiting Catholic Cemeteries Chicago website in browser, submitting SF-180 for Mariano's WWII records

**No significant new finds are possible through web search alone.** The research has reached the paywall ceiling.

## Recommendation
The next iteration should NOT be a blind web search. Instead, the cron prompt should be updated to reflect that **the project is paused pending Adrian's Ancestry access**. The 65-iteration cap in CRON_PROMPT.md should be enforced — this is iteration 62 and no new ground can be broken without account-gated resources.
