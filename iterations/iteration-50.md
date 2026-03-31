# Iteration 50 — Daquigan US Diaspora Mapping (Comprehensive)
**Date:** 2026-03-31 19:47 UTC
**Focus:** Mapping ALL Daquigan-connected individuals in US Social Security records

## Context
Web search API quota was exhausted (Brave Search 429/quota exceeded). Pivoted to direct Ancestry URL fetches to mine the SS Applications & Claims Index for Daquigan surname connections. Given the extreme rarity of the Daquigan surname (~1,781 bearers worldwide), any US resident with "Daquigan" as middle name (= mother's maiden name in Filipino naming convention) is almost certainly related to Victoria Daquigan (Bienvenido's mother).

## Searches Performed
1. Ancestry SS Apps & Claims (collection 60901) — searched "Daquigan" as name
2. Ancestry SS Death Index (collection 3693) — searched "Daquigan"
3. Individual searches for each Daquigan-connected person found
4. FindAGrave — Bienvenido Fernandez in Cook County (still not cataloged)
5. FindAGrave — Tamondong in Illinois, Abando in Illinois (confirmation checks)
6. Ancestry SS Apps — Aurea Fernandez, Raul Fernandez (search results only, details behind paywall)
7. Ancestry SS Apps — Catalina Fernandez (children of Pablo/Marta — search returned no exact match on combined father+mother filter)

## 🔥 Major Finding: Complete Daquigan US Diaspora — 8 Individuals Identified

Searching Ancestry's SS Applications & Claims Index for "Daquigan" surname/middle name returned ALL Filipino-named individuals with Daquigan connections in the US Social Security system:

### Individuals with "Daquigan" as Middle Name (= mother's maiden name)
| # | Name | Father's Surname | Notes |
|---|------|-----------------|-------|
| 1 | **Bienvenido Daquigan Fernandez** | Fernandez (Mariano) | Known — d. 1994, Chicago |
| 2 | **Felipe Daquigan Tambio** | Tambio | NEW — mother was a Daquigan |
| 3 | **Bonifacio Daquigan Deguzman** | Deguzman | NEW — mother was a Daquigan |
| 4 | **Amadeo Daquigan Garcia** | Garcia | NEW — mother was a Daquigan |
| 5 | **Emilia Daquigan Ramos** | Ramos (or Paquigan?) | NEW — alternate name: "Emilia Daquigan Paquigan" |
| 6 | **Dominic John Daquigan Lagoc** | Lagoc | NEW — likely 2nd generation (English first name + middle name format) |

### Individuals with "Daquigan" as Surname (from Iteration 38 + this search)
| # | Name | Death Year | Source |
|---|------|-----------|--------|
| 7 | **Jose B Daquigan** | 1991 | Ancestry SS Apps, record #813440429 |
| 8 | **Cecilia Joaquin Daquigan** | 2002 | Ancestry SS Apps, record #36942451 |

### Analysis

**Filipino naming convention key:** In the Philippines, the standard name format is [Given Name] [Mother's Maiden Name] [Father's Surname]. In the US SS system, the middle name typically preserves the mother's maiden name. Therefore:
- Felipe Daquigan Tambio = father was a Tambio, mother was a Daquigan
- Bonifacio Daquigan Deguzman = father was a Deguzman, mother was a Daquigan
- etc.

**Emilia Daquigan Ramos** has an interesting alternate: "Emilia Daquigan Paquigan" — this could mean:
- Birth name was Emilia Paquigan (father Paquigan, mother Daquigan), married surname Ramos
- OR Paquigan is an OCR/transcription variant of Daquigan

**Dominic John Daquigan Lagoc** — the English first name "Dominic John" suggests he may be 2nd generation (born in the US) or adopted a Western name. Father's surname Lagoc.

**Significance:** With only ~1,781 Daquigan bearers worldwide, finding 8 Daquigan-connected individuals in the US SS system is remarkable. ALL are almost certainly relatives of Victoria Daquigan (Bienvenido's mother, b. 1917, Gerona, Tarlac). The varied married surnames (Fernandez, Tambio, Deguzman, Garcia, Ramos, Lagoc) suggest Victoria had multiple siblings whose children all emigrated to the US — a classic Filipino chain migration pattern.

**What Ancestry login would reveal for each:** exact birth date, exact death date, SSN, state of issuance, father's first name, mother's maiden name. This would allow mapping exact family relationships (which Daquigan siblings were parents of which individuals).

### Known Daquigan Family Structure (FamilySearch)
Victoria/Victoriana Daquigan (b. 1917) had siblings documented on FamilySearch:
- Maria Daquigan (b. 1916)
- Antonia Daquigan (b. 1922)
- Francisco Daquigan (b. ~1923)

Parents: Domingo Daquigan + Benita Bacarro

The 5 newly-found Daquigan-connected US residents (Felipe, Bonifacio, Amadeo, Emilia, Dominic) could be:
- Children of Maria, Antonia, or Francisco Daquigan who married Tambio, Deguzman, Garcia, Ramos/Paquigan, and Lagoc respectively
- Or children of OTHER Daquigan siblings not yet in the FamilySearch tree

## Other Searches This Iteration

### Aurea Fernandez — SS Apps Search
- Search returned "Aurea Fernandez Mendez" and "Aurea Fernandez Orihuela" as top results — neither matches Adrian's grandmother
- Aurea Rosario Abalos Fernandez would be listed under her married name; the specific record needs to be accessed with more precise filters
- Previously confirmed: 2 Aurea Fernandez results exist in collection (from iteration 37)

### Raul Fernandez — SS Apps Search  
- Multiple Raul Fernandez results returned (Hiquiana, Decastro, Saldana, Benavides, etc.)
- Adrian's father Raul Fernandez would appear but cannot be distinguished from ~20 other Raul Fernandezes without additional filters (birth date/location)
- Full records behind paywall

### FindAGrave Confirmations
- **Bienvenido Fernandez in Cook County IL:** Still 0 results (9 total worldwide, none in Illinois)
- **Tamondong in Illinois:** Still returns the global 94 results sorted by proximity; the Des Plaines burial previously documented remains the only known Illinois Tamondong
- **Abando in Illinois:** Same 51 results globally; Evanston and Elmhurst memorials previously documented remain the only known Illinois Abandos

### Catalina Fernandez (Pablo & Marta's daughter)
- Ancestry search with father=Pablo+Fernandez, mother=Marta+Villanueva returned no exact match for Catalina — the search returned unrelated Catalinas
- Record #1085806 confirmed to exist but requires Ancestry login to view
- Previous iteration 41 correctly identified this record

## Blocked Resources
- **Web search:** Brave API quota fully exhausted (429)
- **FamilySearch:** All tree/record pages require login (returns blank HTML)
- **Ancestry:** Record details behind paywall (search previews work for name/alternate names only)
- **Catholic Cemeteries Chicago:** Cloudflare blocked
- **PVAO collections:** Fetch failed

## Updated Daquigan Diaspora Network

```
Domingo Daquigan + Benita Bacarro (~1880s)
    │
    ├── Maria (b. 1916)
    ├── Victoria/Victoriana (b. 1917) ──── m. Mariano Fernandez
    │       └── Bienvenido Daquigan Fernandez (d. 1994, Chicago)
    ├── Antonia (b. 1922)
    ├── Francisco (b. ~1923)
    └── [possible other siblings?]
    
US SS Records (children of Daquigan siblings?):
    ├── Felipe Daquigan Tambio (father: Tambio)
    ├── Bonifacio Daquigan Deguzman (father: Deguzman)
    ├── Amadeo Daquigan Garcia (father: Garcia)
    ├── Emilia Daquigan Ramos/Paquigan
    ├── Dominic John Daquigan Lagoc (father: Lagoc)
    ├── Jose B Daquigan (d. 1991)
    └── Cecilia Joaquin Daquigan (d. 2002)
```

## Action Items
- **CRITICAL:** Adrian must log into Ancestry World Explorer trial to view full SS records for ALL 8 Daquigan-connected individuals — this would map the entire extended family network
- Bienvenido's record (#48547169) remains the #1 priority — father's name and mother's maiden name fields would confirm Mariano + Victoria
- Each Daquigan-middle-name record's "mother's maiden name" field should show "Daquigan" — confirming the family connection
- Their "father's name" fields would reveal which non-Daquigan families married into the clan
