# Adessa SEO Content Roadmap — May 2026

## Goal
Build topical authority for Adessa around AI marketing, AI advertising, automated social media, marketing automation, and high-intent buyer use cases.

## Status snapshot — 2026-05-25
- Production crawlability remains healthy: `/`, `/blog`, latest blog posts, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, and `/for/amazon-sellers` all returned `200` with zero redirects and no `noindex` detected by curl.
- Sitemap includes published blog posts plus `/compare`, `/for`, use-case pages, compare pages, and `/tools/acos-calculator`. `robots.txt` allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- Google Search Console data could not be checked from Jarvis this week. The local Google OAuth token for `automate.openclaw@gmail.com` is revoked/expired; token refresh failed with `400 invalid_grant` and `Token has been expired or revoked.` No GSC top query/page, CTR, indexing, or crawl data was read.
- Bing Webmaster data is still not configured locally; no Bing/Webmaster config files, environment hints, or CLI were found.
- The Thursday 2026-05-21 publisher run did not land new content. The Adessa SEO Blog Publisher cron is enabled but its last run timed out with `cron: job execution timed out (last phase: tool-execution-started)`.

## Published so far
- 2026-04-10 — Welcome to the Adessa Blog
- 2026-05-07 — What an AI Marketing Platform Should Actually Do
- 2026-05-07 — Automated Social Media Marketing: What to Automate and What Not To
- 2026-05-14 — How to Lower ACOS on Amazon in 30 Days
- 2026-05-14 — AI Advertising Platform: What to Look For Before You Buy
- 2026-05-26 — What Is ACOS? A Plain-English Guide for Amazon Sellers
- 2026-05-31 — AI Social Media Tools vs AI Marketing Platforms
- 2026-06-02 — AI Marketing for Restaurants: What to Automate First

## Previous publisher plan
- Tuesday 2026-05-12 — **AI Advertising Platform: What to Look For Before You Buy** — published
  - Intent: commercial/category evaluation.
  - Angle: buyer criteria for platforms that create, launch, measure, and improve campaigns — not a competitor teardown.
  - Internal links: `/pricing`, `/blog/ai-marketing-platform`, `/for`.
- Thursday 2026-05-14 — **How to Lower ACOS on Amazon in 30 Days** — published
  - Intent: practical Amazon seller pain point with high commercial adjacency.
  - Angle: budget allocation, query cleanup, creative testing, landing-page lift, and off-Amazon support; no fake claims or invented case studies.
  - Internal links: `/for/amazon-sellers`, `/tools/acos-calculator`, `/blog/ai-marketing-platform`.

## Missed publisher plan
- Tuesday 2026-05-19 — **What Is ACOS? A Plain-English Guide for Amazon Sellers** — not published
  - Intent: beginner-to-commercial Amazon PPC education.
  - Angle: define ACOS, break-even ACOS, TACOS, campaign goals, and what actions to take when ACOS is too high or misleading.
  - Internal links: `/tools/acos-calculator`, `/for/amazon-sellers`, `/blog/how-to-lower-acos-on-amazon`.
- Thursday 2026-05-21 — **AI Social Media Tools vs AI Marketing Platforms** — not published
  - Intent: commercial comparison/category education without naming competitors.
  - Angle: explain when standalone scheduling/content tools are enough and when a business needs campaign creation, publishing, measurement, and learning loops in one platform.
  - Internal links: `/blog/automated-social-media-marketing`, `/blog/ai-marketing-platform`, `/pricing`.

## This week's publisher plan
- Tuesday 2026-05-26 — **What Is ACOS? A Plain-English Guide for Amazon Sellers** — published
  - Intent: beginner-to-commercial Amazon PPC education.
  - Angle: define ACOS, break-even ACOS, TACOS, campaign goals, and what actions to take when ACOS is too high or misleading.
  - Internal links: `/tools/acos-calculator`, `/for/amazon-sellers`, `/blog/how-to-lower-acos-on-amazon`.
- Thursday 2026-05-28 — **AI Social Media Tools vs AI Marketing Platforms**
  - Status: published 2026-05-31.
  - Intent: commercial comparison/category education without naming competitors.
  - Angle: explain when standalone scheduling/content tools are enough and when a business needs campaign creation, publishing, measurement, and learning loops in one platform.
  - Internal links: `/blog/automated-social-media-marketing`, `/blog/ai-marketing-platform`, `/pricing`.

## Next planned publisher topic
- **AI Marketing for Restaurants: What to Automate First**
  - Status: published 2026-06-02.
  - Intent: high-intent ICP/use-case education.
  - Angle: a practical restaurant marketing workflow around offers, local social, paid campaigns, menus/events, reviews, and weekly performance review without fake case studies.
  - Internal links: `/for`, `/pricing`, and `/blog/automated-social-media-marketing`.

## Next topic candidate
- **Marketing Automation for Lean Teams: A Practical Buyer's Guide**
  - Intent: broad category/commercial evaluation.
  - Angle: explain what lean teams should automate first across planning, creative, publishing, ads, landing pages, and reporting; keep it practical and avoid vendor comparisons unless approved.
  - Internal links: `/pricing`, `/for`, and `/blog/ai-marketing-platform`.

## Priority clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — published
- AI Social Media Tools vs AI Marketing Platforms — published
- Marketing Automation for Lean Teams: A Practical Buyer’s Guide

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — published
- What Is ACOS? A Plain-English Guide for Amazon Sellers — published
- Sponsored Products vs Sponsored Brands
- Best Amazon PPC Software for Small Sellers in 2026 — hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 — ICP support pages
- AI Marketing for Restaurants — published
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
