# Adessa SEO Content Roadmap — June 2026

## Goal
Build durable organic visibility around AI marketing, AI advertising, automated social media, and high-intent operator use cases while keeping Adessa positioned broadly as "AI marketing on autopilot."

## Status Snapshot — 2026-06-08
- Production crawlability is healthy by curl. `/`, `/blog`, latest blog posts, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, and `/for/amazon-sellers` returned `200` with zero redirects and no `noindex` detected.
- Latest posts checked live:
  - `/blog/marketing-automation-for-lean-teams` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
  - `/blog/ai-marketing-for-restaurants` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
- `robots.txt` allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- `sitemap.xml` includes the current blog posts, `/compare`, compare detail URLs, `/for`, use-case URLs, and `/tools/acos-calculator`.
- Google Search Console data could not be checked. Google OAuth refresh succeeded, but Search Console API calls returned `403 PERMISSION_DENIED` / `ACCESS_TOKEN_SCOPE_INSUFFICIENT` for `SitesService.List` and `SearchAnalyticsService.Query`; the current token does not include Search Console/Webmasters scopes.
- Bing Webmaster data is still unavailable locally. No Bing/Webmaster config path, environment hint, or CLI was found.
- Web search spot-check found the Adessa homepage cited for `site:adessa.ai Adessa AI`. Exact post index spot-checks could not be used because the configured Gemini search path returned malformed JSON responses, so no page-level index coverage claim is made here.
- App-code SEO notes for a separate approved pass:
  - Homepage still did not emit a canonical tag in the live HTML while `/blog`, blog posts, `/compare`, and `/for` did.
  - `llms.txt` still says "AI-powered advertising platform for small businesses" and lists small-business-specific audience bullets. Broaden this to match the current positioning preference: "AI marketing on autopilot" without limiting the product to small businesses.

## Content Shipped Last Week
- 2026-06-02 — **AI Marketing for Restaurants: What to Automate First**
  - Intent: high-intent local business use-case education.
  - Internal links: `/for`, `/pricing`, `/blog/automated-social-media-marketing`.
- 2026-06-04 — **Marketing Automation for Lean Teams: A Practical Buyer's Guide**
  - Intent: broad commercial category education for lean operators evaluating automation.
  - Internal links: `/blog/ai-marketing-platform`, `/pricing`, `/for`.
- Missed/carry-forward: **AI Marketing for Gyms: How to Fill Classes Without Living on Social Media** was planned for 2026-06-04 but was not present in the repo or sitemap on 2026-06-08.

## This Week's Publisher Plan
- Tuesday 2026-06-09 — **AI Marketing for Gyms: How to Fill Classes Without Living on Social Media**
  - Status: published 2026-06-09.
  - Target keyword: `AI marketing for gyms`
  - Intent: high-intent local business use-case education.
  - Angle: turn class schedules, seasonal offers, transformation stories, retention nudges, and paid/social campaigns into a repeatable weekly marketing loop.
  - Internal links: `/for`, `/for/gyms`, `/pricing`, `/blog/ai-marketing-platform`, and `/blog/automated-social-media-marketing`.
- Thursday 2026-06-11 — **AI Marketing for Dentists: What to Automate Before You Buy More Ads**
  - Status: published 2026-06-16.
  - Target keyword: `AI marketing for dentists`
  - Intent: high-intent local business use-case education.
  - Angle: practical dental marketing workflow for new-patient offers, recall/reactivation, local service-line campaigns, review mining, ad creative, and weekly performance review without clinical claims or fake patient outcomes.
  - Internal links: `/for/dentists`, `/pricing`, and `/blog/ai-advertising-platform`.

## Priority Clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — published
- AI Social Media Tools vs AI Marketing Platforms — published
- Marketing Automation for Lean Teams: A Practical Buyer's Guide — published
- Weekly Marketing Plan with AI: What to Decide, Draft, Launch, and Review — next broad-category candidate

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — published
- What Is ACOS? A Plain-English Guide for Amazon Sellers — published
- Sponsored Products vs Sponsored Brands
- Best Amazon PPC Software for Small Sellers in 2026 — hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 — ICP support posts
- AI Marketing for Restaurants — published
- AI Marketing for Gyms — published
- AI Marketing for Dentists — published
- AI Marketing for SaaS Startups
- AI Marketing for Fashion Brands

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
