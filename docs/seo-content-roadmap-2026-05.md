# Adessa SEO Content Roadmap — May 2026

## Goal
Build topical authority for Adessa around AI marketing, AI advertising, automated social media, marketing automation, and high-intent buyer use cases.

## Status snapshot — 2026-05-11
- Production crawlability has improved since the 2026-05-07 review: `/`, `/blog`, current blog posts, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, and `/for/amazon-sellers` all return `200` with no redirect-to-login and no `noindex` detected by curl.
- Sitemap includes the blog posts plus the `/compare`, `/for`, tools, legal, and support URLs.
- Google Search Console data could not be checked from Jarvis yet: current Google OAuth token is missing Search Console scopes and the API returned `403 ACCESS_TOKEN_SCOPE_INSUFFICIENT` for `google.searchconsole.v1.SitesService.List`.
- Bing Webmaster data is not configured locally yet; no Bing/Webmaster config files or environment hints were found.
- Web search spot-check: Google/Gemini search sees the homepage for an Adessa AI query, but no reliable evidence yet that `/for/amazon-sellers` is indexed.

## Published so far
- 2026-04-10 — Welcome to the Adessa Blog
- 2026-05-07 — What an AI Marketing Platform Should Actually Do
- 2026-05-07 — Automated Social Media Marketing: What to Automate and What Not To

## This week's publisher plan
- Tuesday 2026-05-12 — **AI Advertising Platform: What to Look For Before You Buy**
  - Intent: commercial/category evaluation.
  - Angle: buyer criteria for platforms that create, launch, measure, and improve campaigns — not a competitor teardown.
  - Internal links: `/pricing`, `/blog/ai-marketing-platform`, `/for`.
- Thursday 2026-05-14 — **How to Lower ACOS on Amazon in 30 Days**
  - Intent: practical Amazon seller pain point with high commercial adjacency.
  - Angle: budget allocation, query cleanup, creative testing, landing-page lift, and off-Amazon support; no fake claims or invented case studies.
  - Internal links: `/for/amazon-sellers`, `/tools/acos-calculator`, `/blog/ai-marketing-platform`.

## Priority clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — planned for 2026-05-12
- Marketing Automation for Small Businesses: A Practical Buyer’s Guide
- AI Social Media Tools vs AI Marketing Platforms

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — planned for 2026-05-14
- What Is ACOS? A Plain-English Guide for Amazon Sellers
- Sponsored Products vs Sponsored Brands
- Best Amazon PPC Software for Small Sellers in 2026 — hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 — ICP support pages
- AI Marketing for Restaurants
- AI Marketing for Gyms
- AI Marketing for Dentists
- AI Marketing for SaaS Startups
- AI Marketing for Fashion Brands

## Internal linking rules
Every post should include 2-3 internal links to:
- https://www.adessa.ai/pricing
- https://www.adessa.ai/for
- Relevant /for/[use-case] page once public
- Relevant /compare/[competitor] page only when naming competitors is explicitly approved

## Editorial guardrails
- Avoid fake review/rating schema.
- Avoid competitor-critical content without Jonathan approval.
- Prefer category education, buyer criteria, practical workflows, and honest limitations over generic AI fluff.
- Keep Adessa positioning broad: “AI marketing on autopilot,” not only “for small businesses.”
