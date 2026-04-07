# Iteration 130 — Official USCIS / NARA Immigration-Path Clarification (2026-04-07 02:29 UTC)

## Focus
Pursue the **Chicago 1981 immigration / naturalization** lead using only directly reachable official sources, since Ancestry and FamilySearch remain blocked from this environment.

## Methods
Used direct HTTP fetches against official pages from:
- `uscis.gov`
- `archives.gov`

Pages checked:
- `https://www.uscis.gov/records/genealogy`
- `https://www.archives.gov/research/immigration/aliens`
- `https://www.archives.gov/chicago/finding-aids/naturalization-records.html`

## Findings

### 1) USCIS Genealogy is an official active path for deceased immigrants
The live USCIS Genealogy page explicitly states that it is a **"fee-for-service program"** that provides researchers access to historical immigration and naturalization records of **deceased immigrants**.

Operationally, this confirms an official route still exists for Bienvenido Fernandez's immigration/naturalization paper trail outside Ancestry.

### 2) Bienvenido's A-file is NOT currently at NARA
The live National Archives **Alien Files (A-Files)** page states that A-files become eligible for transfer to NARA custody **100 years after the immigrant's year of birth**.

Because Bienvenido was born in **1937**, an A-file for him would not become NARA-transfer eligible until **2037**.

**Implication:**
- A current NARA A-file search is **not** the right path for Bienvenido
- The current federal-record path should be:
  1. **USCIS Genealogy / record request** for deceased-immigrant records
  2. **NARA Chicago naturalization index lookup** for the Northern District of Illinois

### 3) NARA Chicago naturalization route remains valid
The live NARA Chicago naturalization page still shows that for **Illinois, Northern District, Chicago**, the archive holds:
- **Petition indexes: 1872-1991**
- **Declarations of intention: 1872-1991**
- **Petitions: 1872-1991**

This keeps Bienvenido's reported **1981 Chicago arrival** squarely inside a documented naturalization-search window.

## What this changes
This iteration did not unlock new family names or dates, but it **did** narrow the correct archive strategy:

### Best current federal path for Bienvenido
- **USCIS Genealogy / record request** = best path for immigration / alien-file style records of a deceased immigrant
- **NARA Chicago** = best path for naturalization index / petition lookup
- **Do not spend time on current NARA A-file searches for Bienvenido** — by the Archives' own rule, that transfer window does not open until **2037**

## Negative / limiting results
- `web_search` continued failing with `fetch failed`
- No direct online name-level hit for Bienvenido Fernandez was unlocked from USCIS/NARA pages
- No new genealogical person/date/place facts were discovered this run

## Operational conclusion
The Chicago/1981 lead is now cleaner:
- **Naturalization** → NARA Chicago
- **Immigration / deceased immigrant records** → USCIS Genealogy
- **A-file at NARA** → not yet applicable for Bienvenido because **1937 birth year ⇒ 2037 transfer eligibility**

## Best next actions
1. **Manual Ancestry #48547169** — Bienvenido SS application
2. **USCIS Genealogy / record request** for Bienvenido Fernandez
3. **NARA Chicago naturalization index lookup** for Bienvenido Fernandez / Bienvenido D. Fernandez
4. **Manual Ancestry #4029022** — Pablo Fernandez + Marta Villanueva marriage
