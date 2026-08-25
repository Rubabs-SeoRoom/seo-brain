---
id: fund-search-fundamentals
title: Search Fundamentals
type: concept
status: seed
created: 2026-08-25
updated: 2026-08-25
tags: [seo-fundamentals, crawling]
next: [tech-crawling]
sources: []
owner: me
---

# Search Fundamentals

> A search engine is a machine that finds documents, understands what they mean, and ranks them by how well they answer a query — through three sequential stages: crawling, indexing, and ranking.

## Why it matters

Every tactic in this repository is downstream of this one idea. "Improve my SEO" is meaningless until you can say which of the three stages you're actually trying to influence. A page that can't be **crawled** never gets a chance to be **indexed**. A page that isn't **indexed** never gets a chance to be **ranked**. Clients (and beginners) conflate all three into one vague fear — "Google doesn't like my site" — and the job of an SEO is to diagnose which stage is actually broken before touching anything else.

## How it works

Search engines run three distinct, sequential processes:

1. **Crawling** — automated bots (Googlebot, Bingbot) discover URLs by following links and reading sitemaps, then download the content of each page.
2. **Indexing** — the search engine processes what it crawled: renders the page, extracts text and structured data, evaluates canonical signals, and decides whether (and how) to store it in its index — the searchable database of all known pages.
3. **Ranking** — at query time, the engine retrieves candidate pages from the index and orders them using hundreds of signals (relevance, authority, quality, user experience, freshness, and more), then assembles a results page that may mix traditional listings with SERP features.

```
Crawl → Index → Rank
(can they find it) → (do they understand and store it) → (do they show it, and where)
```

A page can fail at any one stage independently of the others. It can be perfectly crawlable and still never get indexed (thin or duplicate content). It can be indexed and still never rank (low relevance or authority). Diagnosis always starts by isolating which stage is the actual bottleneck — usually with `site:` search, Search Console's URL Inspection tool, and a crawl of the site itself.

## How I apply it

*(Draft — replace with your own working method once you've applied this on a real site or client.)*

When a page underperforms, I check the stages in order rather than jumping straight to ranking tactics:

1. Is it crawlable? (robots.txt, internal links, no accidental noindex/blocking)
2. Is it indexed? (`site:` search, Search Console coverage report)
3. If indexed but not ranking — only then do I look at relevance, quality, and authority signals.

This ordering stops me from wasting time optimizing content on a page Google never actually indexed in the first place.

## Common mistakes

*(Draft — add real mistakes from your own journal as you make them, and link the entries below.)*

- Treating "not ranking" and "not indexed" as the same problem — they require completely different fixes.
- Assuming a page is crawlable because it loads fine in a browser; bots and browsers don't always see the same thing (see [Rendering](../02-technical-seo/rendering.md) once written).
- Optimizing on-page content for a page that's blocked in robots.txt — no amount of content quality matters if the crawl stage never happens.

## Connections

- **Prerequisites:** none — this is the entry point of Chain 1
- **Related:** —
- **Next:** [Crawling](../02-technical-seo/crawling.md)
- **Used in:** —

## Sources

## Changelog
- 2026-08-25 — v1.0 created (seed)
