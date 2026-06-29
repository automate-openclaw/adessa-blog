# Adessa SEO Content Roadmap — June 2026

## Goal
Build durable organic visibility around AI marketing, AI advertising, automated social media, and high-intent operator use cases while keeping Adessa positioned broadly as "AI marketing on autopilot."

## Status Snapshot — 2026-06-29
- Production crawlability is healthy by curl. `/`, `/blog`, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, `/blog/ai-campaign-launch-checklist`, `/blog/ai-marketing-for-saas-startups`, and `/blog/weekly-marketing-plan-with-ai` returned `200` with zero redirects and no `noindex` or `X-Robots-Tag` blocker detected.
- Latest posts checked live:
  - `/blog/ai-campaign-launch-checklist` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
  - `/blog/ai-marketing-for-saas-startups` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
  - `/blog/weekly-marketing-plan-with-ai` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
- `robots.txt` allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- `sitemap.xml` currently includes 49 URLs, including all 14 live blog posts, `/compare`, compare detail URLs, `/for`, use-case URLs, and `/tools/acos-calculator`.
- Google Search Console data could not be checked. The local Google OAuth refresh succeeds for `automate.openclaw@gmail.com`, but the refreshed token does not include Search Console/Webmasters scope. Search Console API calls fail with `403 PERMISSION_DENIED` / `ACCESS_TOKEN_SCOPE_INSUFFICIENT` for `SitesService.List` and `SearchAnalyticsService.Query`, so no top query/page, click, CTR, indexing, or crawl data was read.
- Bing Webmaster data is still unavailable locally. No Bing/Webmaster config path, environment hint, or CLI was found.
- App-code SEO notes for a separate approved pass:
  - Homepage still does not emit a canonical tag in the live HTML while `/blog`, blog posts, `/compare`, and `/for` do.
  - `llms.txt` still says "AI-powered advertising platform for small businesses" and lists small-business-specific audience bullets. Broaden this to match the current positioning preference: "AI marketing on autopilot" without limiting the product to small businesses.

## Content Shipped Last Week
- 2026-06-23 — **AI Marketing for SaaS Startups: Build a Demand Loop Before You Hire a Team**
  - Intent: high-intent ICP support for lean founders evaluating marketing automation.
  - Internal links: `/blog/weekly-marketing-plan-with-ai`, `/pricing`, `/for/saas`.
- 2026-06-25 — **AI Campaign Launch Checklist for Platform-Ready Ads**
  - Intent: practical workflow content aligned with Adessa's "website in -> campaigns out" proof loop.
  - Internal links: `/blog/ai-advertising-platform`, `/for`, `/pricing`.

## This Week's Publisher Plan
- Tuesday 2026-06-30 — **AI Marketing for Fashion Brands: Turn Drops, Content, and Retargeting Into a Weekly Loop**
  - Status: planned.
  - Target keyword: `AI marketing for fashion brands`
  - Intent: high-intent ICP/use-case education for operators with product launches, seasonal drops, creator assets, and repeat purchase loops.
  - Angle: show how fashion brands can turn product drops, offer windows, creator content, email/social promotion, paid creative, retargeting, and weekly review into one repeatable campaign rhythm without fake performance claims.
  - Internal links: `/for`, `/pricing`, `/blog/ai-campaign-launch-checklist`, `/blog/automated-social-media-marketing`, and `/blog/marketing-automation-for-lean-teams`.
- Thursday 2026-07-02 — **Sponsored Products vs Sponsored Brands: Which Amazon Ad Type Should You Use First?**
  - Status: planned.
  - Target keyword: `Sponsored Products vs Sponsored Brands`
  - Intent: Amazon PPC education with commercial adjacency for sellers deciding what to launch or clean up first.
  - Angle: explain when each ad type fits, how budget, product readiness, branded search, creative assets, and ACOS/TACOS should influence the decision; no fake benchmarks or vendor comparisons.
  - Internal links: `/for/amazon-sellers`, `/tools/acos-calculator`, `/blog/what-is-acos-amazon`, and `/blog/how-to-lower-acos-on-amazon`.

## Priority Clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — published
- AI Social Media Tools vs AI Marketing Platforms — published
- Marketing Automation for Lean Teams: A Practical Buyer's Guide — published
- Weekly Marketing Plan with AI: What to Decide, Draft, Launch, and Review — published 2026-06-18
- AI Campaign Launch Checklist: From Business URL to Platform-Ready Ads — published 2026-06-25

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — published
- What Is ACOS? A Plain-English Guide for Amazon Sellers — published
- Sponsored Products vs Sponsored Brands — planned 2026-07-02
- Best Amazon PPC Software for Small Sellers in 2026 — hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 — ICP support posts
- AI Marketing for Restaurants — published
- AI Marketing for Gyms — published
- AI Marketing for Dentists — published
- AI Marketing for SaaS Startups — published 2026-06-23
- AI Marketing for Fashion Brands — planned 2026-06-30

## Internal Linking Rules
Every post should include 2-3 internal links to:
- `https://www.adessa.ai/pricing`
- `https://www.adessa.ai/for`
- Relevant `/for/[use-case]` page once public
- Relevant category education posts
- Relevant `/compare/[competitor]` page only when naming competitors is explicitly approved

## Editorial Guardrails
- Avoid fake review/rating schema.
- Avoid fake claims, fake benchmarks, invented case studies, and unsupported ROI promises.
- Avoid competitor-critical content without Jonathan approval.
- Prefer category education, buyer criteria, practical workflows, and honest limitations over generic AI fluff.
- Keep Adessa positioning broad: "AI marketing on autopilot," not only "for small businesses."
