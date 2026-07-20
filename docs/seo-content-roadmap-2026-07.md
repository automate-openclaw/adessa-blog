# Adessa SEO Content Roadmap - July 2026

## Goal
Keep compounding durable organic visibility around AI marketing on autopilot, high-intent operator workflows, and Amazon seller education while avoiding fake claims, fake review schema, and competitor-critical content without Jonathan approval.

## Status Snapshot - 2026-07-20
- Production crawlability is mostly healthy by curl. `/`, `/blog`, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, `/for/amazon-sellers`, `/blog/ai-campaign-launch-checklist`, `/blog/ai-marketing-for-saas-startups`, and `/blog/weekly-marketing-plan-with-ai` returned `200` with zero redirects.
- Confirmed indexable article pages:
  - `/blog/ai-campaign-launch-checklist` returned `200`, emitted canonical markup, had no `noindex`, and included `BlogPosting` schema.
  - `/blog/ai-marketing-for-saas-startups` returned `200`, emitted canonical markup, had no `noindex`, and included `BlogPosting` schema.
  - `/blog/weekly-marketing-plan-with-ai` returned `200`, emitted canonical markup, had no `noindex`, and included `BlogPosting` schema.
- `robots.txt` is accessible, allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- `sitemap.xml` returned `200` and currently includes 49 URLs, including `/compare`, `/for`, use-case URLs, and all 14 real blog URLs.
- Missing blog slug behavior still needs a separate app-code pass: `/blog/ai-marketing-for-fashion-brands` and `/blog/sponsored-products-vs-sponsored-brands` return `200` with the blog listing shell, `noindex`, no canonical tag, and no `BlogPosting` schema. This prevents indexing but creates soft-404 ambiguity and can make planned-but-unpublished topics look shipped unless the body/schema/canonical are checked.
- Homepage still does not emit a live canonical tag. `/blog`, real blog posts, `/compare`, and `/for` do emit canonical markup.
- `llms.txt` is accessible, but still narrows positioning to "AI-powered advertising platform for small businesses." Broaden this in a separate approved app-code/content pass to match the current positioning preference: "AI marketing on autopilot."
- The `Adessa SEO Blog Publisher` cron is currently disabled, with no `nextRunAtMs`. The weekly review cron remains enabled. Re-enabling the publisher should be an explicit owner/guardrail decision because it commits and publishes external content.

## Search Console / Bing Data
- Google Search Console data was not checked because the current Google OAuth token does not include Search Console/Webmasters scope. Token refresh works and returns workspace scopes such as Gmail, Drive, Calendar, Docs, Sheets, YouTube, and profile, but no Search Console scope. `GET https://www.googleapis.com/webmasters/v3/sites` returned `403 PERMISSION_DENIED` with `ACCESS_TOKEN_SCOPE_INSUFFICIENT` for `google.searchconsole.v1.SitesService.List`. No GSC top query/page, impression, click, CTR, indexing, or crawl data was read.
- Bing Webmaster data was not checked. Local checks found no Bing/Webmaster config files, no relevant Bing/Webmaster environment variable names, and no `bing`, `bingsiteauth`, or `gcloud` CLI available.

## Content Shipped Last Week
- No new blog posts landed between 2026-07-13 and 2026-07-19.
- The planned 2026-07-14 and 2026-07-16 topics did not land as real posts in `automate-openclaw/adessa-blog` or the live sitemap.
- The live URLs `/blog/ai-marketing-for-fashion-brands` and `/blog/sponsored-products-vs-sponsored-brands` return `200`, but they are the noindexed blog shell with no canonical and no `BlogPosting` schema, so they should not be counted as shipped content.

## This Week's Publisher Plan
- Tuesday 2026-07-21 - **AI Marketing for Fashion Brands: Turn Drops, Content, and Retargeting Into a Weekly Loop**
  - Status: carry-forward again because it still has not published; requires publisher cron re-enable or a manual approved publisher run.
  - Target keyword: `AI marketing for fashion brands`
  - Intent: high-intent ICP/use-case education for operators with product launches, seasonal drops, creator assets, and repeat purchase loops.
  - Angle: show how fashion brands can turn product drops, offer windows, creator content, email/social promotion, paid creative, retargeting, and weekly review into one repeatable campaign rhythm without fake performance claims.
  - Internal links: `/for`, `/pricing`, `/blog/ai-campaign-launch-checklist`, `/blog/automated-social-media-marketing`, and `/blog/marketing-automation-for-lean-teams`.
- Thursday 2026-07-23 - **Sponsored Products vs Sponsored Brands: Which Amazon Ad Type Should You Use First?**
  - Status: carry-forward again because it still has not published; requires publisher cron re-enable or a manual approved publisher run.
  - Target keyword: `Sponsored Products vs Sponsored Brands`
  - Intent: Amazon PPC education with commercial adjacency for sellers deciding what to launch or clean up first.
  - Angle: explain when each ad type fits, how budget, product readiness, branded search, creative assets, and ACOS/TACOS should influence the decision; no fake benchmarks, fake vendor comparisons, or invented performance claims.
  - Internal links: `/for/amazon-sellers`, `/tools/acos-calculator`, `/blog/what-is-acos-amazon`, and `/blog/how-to-lower-acos-on-amazon`.

## Priority Clusters

### Cluster 1 - Broad Category / Workflow Posts
- What an AI Marketing Platform Should Actually Do - published
- Automated Social Media Marketing: What to Automate and What Not To - published
- AI Advertising Platform: What to Look For Before You Buy - published
- AI Social Media Tools vs AI Marketing Platforms - published
- Marketing Automation for Lean Teams: A Practical Buyer's Guide - published
- Weekly Marketing Plan with AI: What to Decide, Draft, Launch, and Review - published
- AI Campaign Launch Checklist for Platform-Ready Ads - published

### Cluster 2 - Amazon / High-Intent Posts
- How to Lower ACOS on Amazon in 30 Days - published
- What Is ACOS? A Plain-English Guide for Amazon Sellers - published
- Sponsored Products vs Sponsored Brands - planned 2026-07-23
- Best Amazon PPC Software for Small Sellers in 2026 - hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 - ICP Support Posts
- AI Marketing for Restaurants - published
- AI Marketing for Gyms - published
- AI Marketing for Dentists - published
- AI Marketing for SaaS Startups - published
- AI Marketing for Fashion Brands - planned 2026-07-21

## Separate App-Code Brief
- Keep monitoring sitemap completeness, but the 2026-07-20 production check showed all 14 real blog URLs present.
- Make unknown blog slugs return a real 404, or at least a clearly non-indexable 404 status, instead of a `200` noindexed blog shell.
- Add a homepage canonical tag.
- Broaden `llms.txt` positioning from "for small businesses" toward "AI marketing on autopilot" while keeping pricing/audience details factual.

## Editorial Guardrails
- No fake claims, fake benchmarks, invented case studies, or unsupported ROI promises.
- No fake review/rating schema.
- No competitor-critical content without Jonathan approval.
- Prefer category education, practical workflows, buyer criteria, and honest limitations over generic AI content.
- Keep Adessa positioned broadly as "AI marketing on autopilot," not only "for small businesses."
