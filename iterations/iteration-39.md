# Iteration 39 — Ancestry Tree Discovery + Immigration/WWII Records Search
**Date:** 2026-03-31 05:54 UTC (12:54 AM CDT)
**Focus:** Immigration records (Chicago 1981), Mariano Fernandez WWII records, Tamondong family trees, Ancestry SS record access

## Constraints This Iteration
- **Brave Search API quota exhausted** (2000/2000 for plan) — no web searches available
- Used direct URL fetching for Ancestry, FamilySearch, Geni, NARA, FindAGrave, Fold3
- Most genealogy sites (FamilySearch, Ancestry trees, Geni profiles) require JS rendering or login — limited data extractable

## Key Findings

### 🔥 NEW: Ancestry Tree #68186126 Contains Bienvenido Daquigan Fernandez
- **URL:** https://www.ancestry.com/family-tree/person/tree/68186126/person/42177724137
- This is a **separate Ancestry tree** from the FamilySearch tree (which is maintained by John Zander Magday/Kristine8553)
- The search results preview shows redacted fields: Father [xxxxxx xxxxxx], Mother [xxxxxxx xxxxxxxx xxxxxxxxx], Children [xxxx xxxxxxx], Birth [x xxx], Death [xx xxx xxxx]
- **CRITICAL:** The Birth field shows "x xxx" format (short) and the Death shows "xx xxx xxxx" — suggesting birth may be just day+month (March 22?) and death is full date
- Birth place shows: Philippines
- Death year: 1994
- **ACTION REQUIRED:** Adrian must log into Ancestry World Explorer trial to view this tree's full details — it may contain siblings, additional children, or different source information than the FamilySearch tree

### Geni: Juan & Luis Tamondong — Brothers Confirmed
- **Luis Tamondong** — Geni profile ID: 6000000016169609781
  - Husband of **Fausta Tamondong** (endogamous marriage — same surname)
  - Father of **Florencia Godoy** + 3 private profiles + 1 other
  - **Brother of Juan Tamondong** (confirmed sibling relationship on Geni)
- **Juan Tamondong** — Geni profile ID: 6000000016169609747
  - Brother of Luis Tamondong
  - **This could be Adrian's ancestor Juan Tamondong (~1850)** who married Juana Paglingayen
  - Profile requires Geni login to view full details (parents, children, dates)
  - The endogamous marriage (Luis married a Tamondong) and the Godoy married name (Florencia Godoy) could help trace descendants
  
### Immigration Record Searches — ALL NEGATIVE
- **Ancestry Passenger Lists (Collection 7488):** Only covers through 1957 — too early for 1981 immigration
- **Ancestry Immigration category search:** Zero results matching Bienvenido Fernandez + Philippines + Illinois
- **NY State/Federal Naturalization Records (Collection 2280):** Only covers through 1943
- **INS records for post-1965 arrivals:** Not digitized on Ancestry
- **Assessment:** The 1981 immigration records likely exist in:
  1. **USCIS A-files** (Alien Registration files) — requestable via FOIA by direct family members
  2. **INS records at NARA** — but post-1957 arrivals not yet digitized
  3. **Illinois naturalization records** — Cook County Clerk's office, not online
  4. Bienvenido's **SS Application (record #48547169)** should contain immigration-adjacent data (when SSN was issued → approximate arrival date)

### Mariano Fernandez WWII Records — NEGATIVE (Online)
- **NARA AAD (Access to Archival Databases):** Site has been restructured; old search URL returns 404
- **NARA Catalog API:** Failed to return results
- **Fold3 (military records):** Requires JS rendering, no data extractable
- **PVAO (Philippine Veterans Affairs Office):** Cloudflare-blocked
- **FindAGrave for Mariano Fernandez + Philippines:** 56 results found, but none matching our Mariano (b. ~1905, Pangasinan/Tarlac)
- **Assessment:** Mariano's WWII service records are almost certainly in:
  1. **NARA Record Group 407, Entry 1087** — Philippine guerrilla and PA files
  2. Specifically **Files 185-1 through 185-30** (Army of the Agno) or **File 308-23** (ECLGA/PTMD)
  3. Requesting requires physical visit to NARA College Park, MD, or a written request via SF-180 form
  4. As noted in previous iterations, Raul Fernandez (as grandson) could submit SF-180 with documentation

### Aurea Fernandez Immigration Search — NEGATIVE
- Ancestry immigration category search returned no Philippine/Illinois matches
- One Aurea in an Ancestry tree (tree #157406842) married to "Manuel Bernardo Fernandes" — NOT our family (different person)

## Searches Performed
1. Ancestry Collection 60901 (SS Apps) — confirmed Bienvenido record #48547169 exists (known)
2. Ancestry Immigration category — zero results for Bienvenido + Philippines + Illinois
3. Ancestry Passenger Lists (7488) — only pre-1957 records
4. Ancestry Naturalization Records (2280) — only pre-1943 records
5. Ancestry WWII Draft Cards (1002) — searched Raul Fernandez, no Philippine/Illinois match
6. Ancestry Tree #68186126 — NEW: contains Bienvenido with family (requires login)
7. FamilySearch record search — requires login (JS-rendered)
8. FamilySearch tree GW9H-FMJ (Mariano) — requires login
9. NARA Catalog API — failed
10. NARA AAD — restructured, old URL broken
11. Fold3 — requires JS rendering
12. PVAO — Cloudflare blocked
13. FindAGrave for Mariano Fernandez + Philippines — 56 results, no match
14. Geni: Luis Tamondong profile — confirmed brother of Juan Tamondong
15. Geni: Juan Tamondong profile — exists but requires login for details
16. Geni: Carlina Tamondong — search blocked by cookie wall

## Action Items for Adrian
1. **HIGHEST PRIORITY:** Log into Ancestry World Explorer trial → view record #48547169 (Bienvenido's SS Application) AND tree #68186126 (new family tree)
2. **Log into FamilySearch (Adrian26448)** → search Cook County Deaths 1871-1998 for Bienvenido Fernandez (1994)
3. **Ask Raul:** Did Mariano Fernandez serve in WWII guerrillas? If yes, could submit SF-180 to NARA for military records
4. **Consider FOIA request** to USCIS for Bienvenido's A-file (immigration file) — available to direct family members
5. **Create Geni account** → access Juan Tamondong profile (6000000016169609747) for full family details

## Status
- Iteration count: 39/65
- Web search quota: EXHAUSTED for this billing cycle
- Next best leads requiring Adrian's direct access: Ancestry login (SS record + tree), FamilySearch login (Cook County deaths), USCIS FOIA (immigration file)
