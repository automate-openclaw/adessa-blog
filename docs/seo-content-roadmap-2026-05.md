# Adessa SEO Content Roadmap — May 2026

## Goal
Build topical authority for Adessa around AI marketing, AI advertising, automated social media, marketing automation, and high-intent buyer use cases.

## Status snapshot — 2026-05-18
- Production crawlability remains healthy: `/`, `/blog`, latest blog posts, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, and `/for/amazon-sellers` all returned `200` with no redirect-to-login and no `noindex` detected by curl.
- Sitemap includes the latest posts plus `/compare`, `/for`, tools, legal, and support URLs. `robots.txt` allows public crawl paths and points to `https://www.adessa.ai/sitemap.xml`.
- Google Search Console data could not be checked from Jarvis yet. The Google OAuth refresh succeeded, but the token still lacks Search Console scopes; the API returned `403 ACCESS_TOKEN_SCOPE_INSUFFICIENT` for both `google.searchconsole.v1.SitesService.List` and `google.searchconsole.v1.searchanalytics.SearchAnalyticsService.Query`.
- Bing Webmaster data is not configured locally yet; no Bing/Webmaster config files, environment hints, or CLI were found.
- Web search spot-check could not be used this week because the configured Gemini search path returned `429 RESOURCE_EXHAUSTED`. Do not infer index coverage from that failed check.

## Published so far
- 2026-04-10 — Welcome to the Adessa Blog
- 2026-05-07 — What an AI Marketing Platform Should Actually Do
- 2026-05-07 — Automated Social Media Marketing: What to Automate and What Not To
- 2026-05-14 — How to Lower ACOS on Amazon in 30 Days
- 2026-05-14 — AI Advertising Platform: What to Look For Before You Buy

## This week's publisher plan
- Tuesday 2026-05-12 — **AI Advertising Platform: What to Look For Before You Buy** — published
  - Intent: commercial/category evaluation.
  - Angle: buyer criteria for platforms that create, launch, measure, and improve campaigns — not a competitor teardown.
  - Internal links: `/pricing`, `/blog/ai-marketing-platform`, `/for`.
- Thursday 2026-05-14 — **How to Lower ACOS on Amazon in 30 Days** — published
  - Intent: practical Amazon seller pain point with high commercial adjacency.
  - Angle: budget allocation, query cleanup, creative testing, landing-page lift, and off-Amazon support; no fake claims or invented case studies.
  - Internal links: `/for/amazon-sellers`, `/tools/acos-calculator`, `/blog/ai-marketing-platform`.

## Next publisher plan
- Tuesday 2026-05-19 — **What Is ACOS? A Plain-English Guide for Amazon Sellers**
  - Intent: beginner-to-commercial Amazon PPC education.
  - Angle: define ACOS, break-even ACOS, TACOS, campaign goals, and what actions to take when ACOS is too high or misleading.
  - Internal links: `/tools/acos-calculator`, `/for/amazon-sellers`, `/blog/how-to-lower-acos-on-amazon`.
- Thursday 2026-05-21 — **AI Social Media Tools vs AI Marketing Platforms**
  - Intent: commercial comparison/category education without naming competitors.
  - Angle: explain when standalone scheduling/content tools are enough and when a business needs campaign creation, publishing, measurement, and learning loops in one platform.
  - Internal links: `/blog/automated-social-media-marketing`, `/blog/ai-marketing-platform`, `/for`, `/pricing`.

## Priority clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — published
- AI Social Media Tools vs AI Marketing Platforms — planned 2026-05-21
- Marketing Automation for Lean Teams: A Practical Buyer’s Guide

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — published
- What Is ACOS? A Plain-English Guide for Amazon Sellers — planned 2026-05-19
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
