# Iteration 128 — Ancestry Direct-Record Access Probe + Search-Engine Challenge Check (2026-04-07 01:22 UTC)

## Focus
Highest-value next lead under the current priority list: **direct access paths for the two top Ancestry records** plus another pass at **Chicago immigration / naturalization spillover**.

Priority records probed:
1. **Bienvenido Daquigan Fernandez** — Ancestry collection **60901**, record **#48547169** (SS Applications and Claims)
2. **Pablo Fernandez + Marta Villanueva** — Ancestry collection **60130**, record **#4029022** (Philippines marriages)

## Methods
Because OpenClaw `web_search` kept failing with `fetch failed`, this iteration used:
- direct HTTP requests to Ancestry record URLs
- direct HTTP request to the NARA Chicago naturalization page
- DuckDuckGo HTML fallback for public-search spillover

### URLs tested
- `https://www.ancestry.com/search/collections/60901/records/48547169`
- `https://www.ancestry.com/discoveryui-content/view/48547169:60901`
- `https://www.ancestry.com/search/collections/60130/records/4029022`
- `https://www.ancestry.com/discoveryui-content/view/4029022:60130`
- `https://www.archives.gov/chicago/finding-aids/naturalization-records.html`
- DuckDuckGo HTML queries for Bienvenido / Pablo+Marta / Ancestry record-number spillover

## Results

### 1) Ancestry direct record URLs are blocked here by a security-deny layer
Both high-priority records returned a redirect to Ancestry security-deny pages rather than usable record content:

- **Bienvenido SS record #48547169**
  - `HTTP/2 302`
  - redirected to `/security/deny.aspx?dbid=60901...&h=48547169`
- **Pablo + Marta marriage #4029022**
  - `HTTP/2 302`
  - redirected to `/security/deny.aspx?dbid=60130...&h=4029022`

The alternate `discoveryui-content/view/...` URLs only 301-redirected back to the same blocked search/record URLs.

**Important operational conclusion:** the new Ancestry resource is real, but from this automation environment the record pages are not merely paywalled — they are currently intercepted by a **security/deny gate** before any useful metadata is exposed.

### 2) No leaked metadata was visible in the blocked Ancestry response bodies
The returned body previews were generic "Join Ancestry" / site-shell HTML and did **not** expose names, dates, parents, or collection fields for either target record.

So this environment still cannot extract even a partial preview for:
- Bienvenido's SS application (#48547169)
- Pablo + Marta's marriage record (#4029022)

### 3) DuckDuckGo HTML fallback is now challenge-blocked too
DuckDuckGo HTML requests returned **HTTP 202** with an anomaly/bot challenge page rather than parseable results.

This means the public-search fallback has degraded further:
- earlier runs produced sparse/no results
- this run produced a **human verification puzzle** instead of search results

So public spillover search is now blocked at the search-engine layer as well.

### 4) NARA Chicago remains reachable and still confirms the naturalization window
The NARA Chicago naturalization page again returned **HTTP 200**.
Key live text reconfirmed:
- **Petition indexes** exist
- **Declarations** exist
- **Petitions** exist
- Northern District / Chicago naturalization coverage remains the relevant live path
- **USCIS** still holds duplicate copies of post-1906 petitions and post-1991 inquiries usually go there

No new genealogical facts were unlocked, but the Chicago naturalization path remains the strongest reachable non-paywalled U.S. lead.

## Conclusions
- **No new genealogical facts** were unlocked this iteration
- But the access map is now tighter than before:
  - **NARA Chicago page = reachable**
  - **FamilySearch = 403 blocked** (prior iterations)
  - **MyHeritage = anti-bot blocked** (prior iteration)
  - **Ancestry direct record URLs = security/deny redirect**
  - **DuckDuckGo HTML fallback = anomaly challenge / HTTP 202**
  - **OpenClaw web_search = fetch failed**

## Best next actions (unchanged, but now more strongly justified)
1. **Manual browser access to Ancestry #48547169** — still the single best unlock
2. **Manual browser access to Ancestry #4029022** — still the best path to extend the Fernandez line one generation further
3. **Manual FamilySearch browser session (Adrian26448)**
4. **NARA Chicago index lookup / staff-assisted search** for Bienvenido's naturalization record

## Status
- Significant new genealogy: **No**
- Significant new access-state finding: **Yes**
- Discord report sent: **No** (operational update only; no family-tree breakthrough)
