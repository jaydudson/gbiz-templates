# Research Scan Skill

## When to use
When the client asks for a sourced research brief on a specific topic, competitor, supplier, trend, or public page.

## Required inputs and access
- A clear topic or question from the client
- Access to Firecrawl (preferred) or regular web search as fallback
- Optional: specific URLs or source list the client supplies

## Sequence of work
1. Confirm the exact question and any constraints (depth, sources to prefer or avoid, length).
2. Prefer Firecrawl (or installed MCP / structured tool) to fetch and extract relevant pages. Choose the lightest tool that answers the question (see Firecrawl tool guide below).
3. If Firecrawl is unavailable, fall back to regular web search and note it.
4. Synthesise a short brief using the deliverable schema. Include source titles or URLs for every material claim.
5. Flag uncertainty or missing data. Do not invent.
6. Present the brief and stop. Wait for the next request.

## Firecrawl tool guide (token-efficient)
Use the lightest tool that gets the answer. Prefer local files after extraction so later questions do not re-fetch the same pages.

- **map** — Discover all (or filtered) URLs on a domain in one cheap call. Use first when you need to understand a site or pick specific pages before scraping. Does not pull full page content.
- **scrape** — Pull clean markdown (or structured fields) from one known URL. Default for a single page or a short list of known pages.
- **search** — Find relevant pages from a query, optionally with content. Use when you do not yet have URLs.
- **crawl** — Follow links and extract content across a section or site. Use only when you truly need many pages; set a tight limit. Prefer map + selective scrape for most research.
- **batch / download** — After mapping, extract only the pages you need and save them locally. Better than crawling a whole site when you want a subset.
- **interact / browser** — For pages that need clicks, forms, or dynamic content. Use sparingly; higher cost and complexity.
- **parse** — Turn an already-downloaded PDF, doc, or spreadsheet into text. Prefer this over re-scraping when the file is local.

Rule of thumb: map or search first to find the right pages, then scrape only what is needed. Keep results local. Stay inside the free-tier credit budget (1,000 credits/month on the free plan).

## How to validate
Every material claim has a source. The brief matches the deliverable format. No money spent, no external accounts changed, no keys exposed.

## What to return
The short sourced brief only.

## What requires approval
Setting up or changing Firecrawl credentials. Expanding into ongoing monitoring, paid plans, or broader agency-style work.
