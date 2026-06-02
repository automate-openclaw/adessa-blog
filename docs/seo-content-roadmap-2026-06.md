# Adessa SEO Content Roadmap — June 2026

## Goal
Build durable organic visibility around AI marketing, AI advertising, automated social media, and high-intent operator use cases while keeping Adessa positioned broadly as "AI marketing on autopilot."

## Status snapshot — 2026-06-01
- Production crawlability is healthy by curl. `/`, `/blog`, latest blog posts, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, and `/for` returned `200` with zero redirects and no `noindex` detected.
- Latest posts checked live:
  - `/blog/ai-social-media-tools-vs-ai-marketing-platforms` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
  - `/blog/what-is-acos-amazon` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
- `robots.txt` allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- `sitemap.xml` includes the current blog posts, `/compare`, compare detail URLs, `/for`, use-case URLs, and `/tools/acos-calculator`.
- Google Search Console data could not be checked. The Google OAuth token refresh succeeded, but Search Console API calls return `403 PERMISSION_DENIED` / `Request had insufficient authentication scopes`; the current token does not include Search Console/Webmasters scopes.
- Bing Webmaster data is still unavailable locally. No Bing/Webmaster config path, environment hint, or CLI was found.
- App-code SEO notes for a separate approved pass:
  - Homepage did not emit a canonical tag in the live HTML while `/blog`, blog posts, `/compare`, and `/for` did.
  - `llms.txt` still says "AI-powered advertising platform for small businesses." Broaden this to match the current positioning preference: "AI marketing on autopilot" without limiting the product to small businesses.

## Content shipped last week
- 2026-05-26 — **What Is ACOS? A Plain-English Guide for Amazon Sellers**
  - Intent: beginner-to-commercial Amazon PPC education.
  - Internal links: `/tools/acos-calculator`, `/for/amazon-sellers`, `/blog/how-to-lower-acos-on-amazon`.
- 2026-05-31 — **AI Social Media Tools vs AI Marketing Platforms**
  - Intent: commercial category education without naming competitors.
  - Internal links: `/blog/automated-social-media-marketing`, `/blog/ai-marketing-platform`, `/pricing`.

## Content shipped this week
- 2026-06-02 — **AI Marketing for Restaurants: What to Automate First**
  - Intent: high-intent local business use-case education.
  - Internal links: `/for`, `/pricing`, `/blog/automated-social-media-marketing`.

## This week's publisher plan
- Tuesday 2026-06-02 — **AI Marketing for Restaurants: What to Automate First**
  - Status: published 2026-06-02.
  - Target keyword: `AI marketing for restaurants`
  - Intent: high-intent local business use-case education.
  - Angle: a practical restaurant workflow for offers, local social posts, paid campaigns, menu/event promotion, review loops, and weekly performance review without fake case studies or unsupported performance claims.
  - Internal links: `/for`, `/pricing`, `/blog/automated-social-media-marketing`.
- Thursday 2026-06-04 — **AI Marketing for Gyms: How to Fill Classes Without Living on Social Media**
  - Target keyword: `AI marketing for gyms`
  - Intent: high-intent local business use-case education.
  - Angle: turn class schedules, promotions, transformations, retention nudges, and paid/social campaigns into a repeatable weekly marketing loop.
  - Internal links: `/for`, `/pricing`, `/blog/ai-marketing-platform`, and `/blog/automated-social-media-marketing`.

## Priority clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — published
- AI Social Media Tools vs AI Marketing Platforms — published
- Marketing Automation for Lean Teams: A Practical Buyer's Guide

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — published
- What Is ACOS? A Plain-English Guide for Amazon Sellers — published
- Sponsored Products vs Sponsored Brands
- Best Amazon PPC Software for Small Sellers in 2026 — hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 — ICP support posts
- AI Marketing for Restaurants — published
- AI Marketing for Gyms — planned 2026-06-04
- AI Marketing for Dentists
- AI Marketing for SaaS Startups
- AI Marketing for Fashion Brands

## Internal linking rules
Every post should include 2-3 internal links to:
- https://www.adessa.ai/pricing
- https://www.adessa.ai/for
- Relevant `/for/[use-case]` page once public
- Relevant category education posts
- Relevant `/compare/[competitor]` page only when naming competitors is explicitly approved

## Editorial guardrails
- Avoid fake review/rating schema.
- Avoid fake claims, fake benchmarks, invented case studies, and unsupported ROI promises.
- Avoid competitor-critical content without Jonathan approval.
- Prefer category education, buyer criteria, practical workflows, and honest limitations over generic AI fluff.
- Keep Adessa positioning broad: "AI marketing on autopilot," not only "for small businesses."
