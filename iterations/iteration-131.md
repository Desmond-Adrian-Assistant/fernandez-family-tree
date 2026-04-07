# Iteration 131 — USCIS Genealogy Request Mechanics Clarified (2026-04-07 02:31 UTC)

## Focus
Pursue the **Chicago 1981 immigration / naturalization** lead one step further by checking the live official **USCIS Genealogy request mechanics** and how they interact with the already-confirmed NARA Chicago naturalization path.

## Methods
- Attempted targeted `web_search` queries for USCIS Genealogy, NARA Chicago naturalization, and Mariano's guerrilla-file bundle
- Because `web_search` failed repeatedly with `fetch failed`, used direct HTTP fetches against reachable official pages:
  - `https://www.uscis.gov/records/genealogy`
  - `https://www.uscis.gov/records/genealogy/requesting-records`
  - `https://www.archives.gov/chicago/finding-aids/naturalization-records.html`

## Findings

### 1) USCIS Genealogy request page adds an important practical constraint
The live USCIS **Requesting Records** page states that the Genealogy Program makes **five series** available to requesters and that requests are accepted **online as well as through the mail**.

Most importantly, the page explicitly says:
- **"To request a record or file you MUST provide a file number."**

This is operationally important for Bienvenido Fernandez.

### 2) The five USCIS historical record series are now cleanly confirmed
The live USCIS pages explicitly identify the Genealogy Program record series as:
- **C-Files** — naturalization certificate files
- **Alien Registration Forms (AR-2s)** — 1940-1944
- **Visa Files** — July 1, 1924 to March 31, 1944
- **Registry Files** — March 2, 1929 to March 31, 1944
- **A-Files** — immigrant files created or consolidated since **April 1, 1944**

For Bienvenido's reported **1981 Chicago immigration**, the historically relevant USCIS bucket would therefore be an **A-file**, not a visa file / registry file / AR-2.

### 3) USCIS Genealogy is useful — but not a magic substitute for a name-only archive search
The newly fetched request page makes clear that the Genealogy Program is not simply an open public name-search interface from this environment.

Because the live page requires a **file number** to request a record copy, the practical path becomes:
- first obtain or infer the relevant file number from another source if possible
- then use USCIS Genealogy for the actual record request

This means USCIS Genealogy remains an official path, but it is **less self-sufficient than it initially appeared**.

### 4) NARA Chicago remains the stronger reachable name-based archive lead for the 1981 Chicago path
The live NARA Chicago page again confirms that for **Illinois, Northern District, Chicago**, it still holds:
- **Petition indexes: 1872-1991**
- **Declarations of intention: 1872-1991**
- **Petitions: 1872-1991**

And the same page notes that **USCIS holds duplicate copies of naturalization petitions created after September 26, 1906**.

### 5) Updated operational interpretation
Combining Iterations **130** and **131**:
- Bienvenido's likely immigration-era federal file type = **A-file**
- But that A-file is **not yet at NARA** because of the **100-years-after-birth-year** transfer rule
- USCIS Genealogy is the official custodian path, **but its request page requires a file number for a record/file request**
- Therefore the easiest currently documented name-driven archive path remains **NARA Chicago naturalization index lookup**

## Negative / limiting results
- All three targeted `web_search` attempts failed with **`fetch failed`**
- No direct Bienvenido-specific file number was exposed from reachable official sources
- No new genealogical identities, dates, or relationships were unlocked this run

## What changed
This iteration did not add new family-tree facts, but it tightened the process map:

### Best current archive sequence for Bienvenido
1. **NARA Chicago naturalization index lookup** — best documented name-based archive route
2. If a naturalization / certificate / case number is found, use that to support a **USCIS Genealogy request**
3. Treat current USCIS Genealogy as a **number-driven retrieval path**, not a fully self-contained name-only discovery path

## Best next actions
1. **Manual Ancestry #48547169** — Bienvenido SS application
2. **NARA Chicago naturalization index lookup** for Bienvenido Fernandez / Bienvenido D. Fernandez
3. If a federal number is surfaced, use it for **USCIS Genealogy** follow-through
4. **Manual Ancestry #4029022** — Pablo Fernandez + Marta Villanueva marriage
