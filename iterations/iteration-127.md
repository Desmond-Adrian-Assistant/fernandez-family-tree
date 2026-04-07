# Iteration 127 — Tamondong Public-Tree Surface + Access-State Recheck (2026-04-07 00:55 UTC)

## Focus
Highest-value unexplored public lead from the current plan: **Tamondong family trees outside Ancestry/FamilySearch**, especially the weak public MyHeritage surface noted in Iteration 125, while re-checking whether the environment can directly reach priority record systems.

## Methods
Because OpenClaw `web_search` / `web_fetch` failed repeatedly with `fetch failed`, this iteration used direct HTTP checks via `curl`/Python as fallback.

### Targets checked
1. **NARA Chicago naturalization page**
   - https://www.archives.gov/chicago/finding-aids/naturalization-records.html
2. **MyHeritage Tamondong public-tree search surface**
   - https://www.myheritage.com/research/category-10953/family-trees?query=Tamondong
3. **FamilySearch marriage ARK already known for Bienvenido + Aurea**
   - https://www.familysearch.org/ark:/61903/1:1:6B7K-YPD6
4. Public-search fallbacks for:
   - Tamondong family tree / MyHeritage / Pangasinan
   - Bienvenido Daquigan Fernandez / Ancestry #48547169
   - Pablo Fernandez + Marta Villanueva / Ancestry #4029022
   - Bienvenido Chicago 1981 immigration
   - Mariano Fernandez WWII / Tarlac / Pangasinan

## Results

### 1) NARA Chicago remains directly reachable from this environment
- `curl -I` to the NARA Chicago naturalization page returned **HTTP 200**
- This keeps **NARA Chicago** as the strongest live, non-paywalled U.S. research path for Bienvenido's naturalization records
- No new genealogical facts were extracted from the page in this pass, but live reachability was reconfirmed

### 2) MyHeritage Tamondong tree surface is currently bot-blocked here
- `curl -I` to the MyHeritage Tamondong family-tree search returned **HTTP 200**, but the body was only an **Incapsula anti-bot page**
- Returned HTML was a minimal anti-bot stub, not search results
- So the earlier public-search-engine hint that a Tamondong family tree exists on MyHeritage is still plausible, but **not retrievable from this automation environment**

### 3) FamilySearch ARK remains blocked
- `curl -I` to the known Bienvenido+Aurea marriage ARK returned **HTTP 403 Forbidden**
- Confirms again that FamilySearch browser-authenticated content is inaccessible from this environment even when the exact record URL is known

### 4) Public-search fallback produced no usable spillover
- DuckDuckGo HTML fallback returned no parseable result entries for the five targeted searches above
- This means there is still **no public search-engine spillover** usable here for:
  - Bienvenido SS application #48547169
  - Pablo + Marta marriage #4029022
  - Chicago 1981 immigration lead
  - Mariano WWII records
  - Tamondong family tree lead

## Conclusions
- **No new genealogical facts** were unlocked this iteration
- The main new value is a sharper access map:
  - **NARA Chicago = reachable**
  - **FamilySearch = 403 blocked**
  - **MyHeritage = anti-bot blocked**
  - **OpenClaw web_search/web_fetch = currently failing with `fetch failed`**
- This further narrows the best next human/manual actions to:
  1. **Ancestry #48547169** — Bienvenido Daquigan Fernandez SS application
  2. **Ancestry #4029022** — Pablo Fernandez + Marta Villanueva marriage
  3. **Manual FamilySearch browser session (Adrian26448)**
  4. **NARA Chicago contact/search** for naturalization index lookup

## Status
- Significant new genealogy: **No**
- Discord report sent: **No** (nothing substantial enough)
