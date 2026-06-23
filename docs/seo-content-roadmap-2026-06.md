# Adessa SEO Content Roadmap — June 2026

## Goal
Build durable organic visibility around AI marketing, AI advertising, automated social media, and high-intent operator use cases while keeping Adessa positioned broadly as "AI marketing on autopilot."

## Status Snapshot — 2026-06-22
- Production crawlability is healthy by curl. `/`, `/blog`, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, and `/for` returned `200` with zero redirects and no `noindex` detected.
- Latest posts checked live:
  - `/blog/weekly-marketing-plan-with-ai` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
  - `/blog/ai-marketing-for-dentists` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
  - `/blog/ai-marketing-for-gyms` returned `200`, emitted canonical markup, and included `BlogPosting` schema.
- `robots.txt` allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- `sitemap.xml` currently includes 47 URLs, including all 12 live blog posts, `/compare`, compare detail URLs, `/for`, use-case URLs, and `/tools/acos-calculator`.
- Google Search Console data could not be checked. The local Google OAuth refresh now returns `invalid_grant` / `Token has been expired or revoked`, and API calls to Search Console and Google userinfo return `401 UNAUTHENTICATED`. This needs owner reauthorization with Search Console/Webmasters scope before query/page/indexing data can be trusted.
- Bing Webmaster data is still unavailable locally. No Bing/Webmaster config path, environment hint, or CLI was found.
- App-code SEO notes for a separate approved pass:
  - Homepage still does not emit a canonical tag in the live HTML while `/blog`, blog posts, `/compare`, and `/for` do.
  - `llms.txt` still says "AI-powered advertising platform for small businesses" and lists small-business-specific audience bullets. Broaden this to match the current positioning preference: "AI marketing on autopilot" without limiting the product to small businesses.

## Content Shipped Last Week
- 2026-06-16 — **AI Marketing for Dentists: What to Automate Before You Buy More Ads**
  - Intent: high-intent local business use-case education.
  - Internal links: `/blog/ai-advertising-platform`, `/for/dentists`, `/pricing`.
- 2026-06-18 — **Weekly Marketing Plan with AI: What to Decide, Draft, Launch, and Review**
  - Intent: broad workflow education for operators who need repeatable marketing execution.
  - Internal links: `/blog/marketing-automation-for-lean-teams`, `/blog/automated-social-media-marketing`, `/for`, `/pricing`.

## This Week's Publisher Plan
- Tuesday 2026-06-23 — **AI Marketing for SaaS Startups: Build a Demand Loop Before You Hire a Team**
  - Status: published 2026-06-23.
  - Target keyword: `AI marketing for SaaS startups`
  - Intent: high-intent ICP support for lean founders evaluating marketing automation.
  - Angle: turn positioning, launch assets, lifecycle content, paid experiments, and weekly review into a small-team demand loop without implying fake traction or guaranteed growth.
  - Internal links: `/blog/weekly-marketing-plan-with-ai`, `/pricing`, and `/for/saas`.
- Thursday 2026-06-25 — **AI Campaign Launch Checklist: From Business URL to Platform-Ready Ads**
  - Status: planned.
  - Target keyword: `AI campaign launch checklist`
  - Intent: practical workflow content aligned with Adessa's "website in -> campaigns out" proof loop.
  - Angle: show the concrete launch sequence: website/offer intake, audience and message thesis, format coverage, creative quality gates, approval, publishing, tracking, and the first weekly report.
  - Internal links: `/for`, `/pricing`, `/blog/ai-advertising-platform`, `/blog/automated-social-media-marketing`, and `/blog/weekly-marketing-plan-with-ai`.

## Priority Clusters

### Cluster 1 — Broad category pages/posts
- What an AI Marketing Platform Should Actually Do — published
- Automated Social Media Marketing: What to Automate and What Not To — published
- AI Advertising Platform: What to Look For Before You Buy — published
- AI Social Media Tools vs AI Marketing Platforms — published
- Marketing Automation for Lean Teams: A Practical Buyer's Guide — published
- Weekly Marketing Plan with AI: What to Decide, Draft, Launch, and Review — published 2026-06-18
- AI Campaign Launch Checklist: From Business URL to Platform-Ready Ads — planned 2026-06-25

### Cluster 2 — Amazon/high-intent posts
- How to Lower ACOS on Amazon in 30 Days — published
- What Is ACOS? A Plain-English Guide for Amazon Sellers — published
- Sponsored Products vs Sponsored Brands
- Best Amazon PPC Software for Small Sellers in 2026 — hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 — ICP support posts
- AI Marketing for Restaurants — published
- AI Marketing for Gyms — published
- AI Marketing for Dentists — published
- AI Marketing for SaaS Startups — published 2026-06-23
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
