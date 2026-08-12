# Adessa SEO Content Roadmap - August 2026

## Goal
Rebuild the publishing cadence around durable organic visibility for AI marketing on autopilot, practical operator workflows, and Amazon seller education while avoiding fake claims, fake review schema, and competitor-critical content without Jonathan approval.

## Status Snapshot - 2026-08-11
- Production crawlability is healthy by curl for the core public SEO surfaces. `/`, `/blog`, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, and `/for` all returned `200` with zero redirects.
- `robots.txt` is accessible, allows public crawl paths, blocks authenticated app surfaces, and points to `https://www.adessa.ai/sitemap.xml`.
- `sitemap.xml` returned `200`, contains 49 URLs, includes `/compare`, `/for`, use-case URLs, and the 14 real blog URLs currently present in this repo.
- Real recent article pages such as `/blog/ai-campaign-launch-checklist`, `/blog/ai-marketing-for-saas-startups`, and `/blog/weekly-marketing-plan-with-ai` return `200`, emit canonical tags, have no `noindex`, and include `BlogPosting` schema.
- Planned-but-unpublished slugs `/blog/ai-marketing-for-fashion-brands` and `/blog/sponsored-products-vs-sponsored-brands` still return `200` with a noindexed blog shell, no canonical tag, no `BlogPosting` schema, and no sitemap entry. Treat these as not shipped.
- Homepage still does not emit a live canonical tag. `/blog`, real blog posts, `/compare`, and `/for` do emit canonical markup.
- `llms.txt` is accessible, but still says "AI-powered advertising platform for small businesses." Broaden this in a separate approved app-code/content pass to match the positioning preference: "AI marketing on autopilot."

## Search Console / Bing Data
- Google Search Console data was not checked because the current Google OAuth token does not include Search Console/Webmasters scope. Token refresh works and returns Gmail, Drive, Calendar, Docs, Sheets, YouTube, profile, and related workspace scopes, but no Search Console scope. `GET https://www.googleapis.com/webmasters/v3/sites` returned `403 PERMISSION_DENIED` with `ACCESS_TOKEN_SCOPE_INSUFFICIENT` for `google.searchconsole.v1.SitesService.List`. No GSC top query/page, impression, click, CTR, indexing, or crawl data was read.
- Bing Webmaster data was not checked. Local checks found no Bing/Webmaster config files, no relevant Bing/Webmaster environment variable names, and no `bing` or `gcloud` CLI available.

## Content Shipped Last Week
- No new blog posts landed between 2026-08-04 and 2026-08-10.
- The latest real published blog post in `automate-openclaw/adessa-blog` remains `AI Campaign Launch Checklist for Platform-Ready Ads`, published 2026-06-25.
- The previously planned fashion-brand and Amazon ad-type posts did not land as real repo posts and are not in the live sitemap.

## This Week's Publisher Plan
- Tuesday 2026-08-11 - **AI Marketing for Fashion Brands: Turn Drops, Content, and Retargeting Into a Weekly Loop**
  - Status: carry-forward because it still has not published.
  - Target keyword: `AI marketing for fashion brands`
  - Intent: high-intent ICP/use-case education for operators with product launches, seasonal drops, creator assets, and repeat purchase loops.
  - Angle: show how fashion brands can turn product drops, offer windows, creator content, email/social promotion, paid creative, retargeting, and weekly review into one repeatable campaign rhythm without fake performance claims.
  - Internal links: `/for`, `/pricing`, `/blog/ai-campaign-launch-checklist`, `/blog/automated-social-media-marketing`, and `/blog/marketing-automation-for-lean-teams`.
- Thursday 2026-08-13 - **Sponsored Products vs Sponsored Brands: Which Amazon Ad Type Should You Use First?**
  - Status: carry-forward because it still has not published.
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
- Sponsored Products vs Sponsored Brands - planned 2026-08-13
- Best Amazon PPC Software for Small Sellers in 2026 - hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 - ICP Support Posts
- AI Marketing for Restaurants - published
- AI Marketing for Gyms - published
- AI Marketing for Dentists - published
- AI Marketing for SaaS Startups - published
- AI Marketing for Fashion Brands - planned 2026-08-11

## Separate App-Code Brief
- Make unknown blog slugs return a real 404, or at least a clearly non-indexable 404 status, instead of a `200` noindexed blog shell.
- Add a homepage canonical tag.
- Broaden `llms.txt` positioning from "for small businesses" toward "AI marketing on autopilot" while keeping pricing/audience details factual.
- Add Search Console OAuth scope to Jarvis Google auth before the next weekly review if we want query/page/CTR/index coverage.

## Editorial Guardrails
- No fake claims, fake benchmarks, invented case studies, or unsupported ROI promises.
- No fake review/rating schema.
- No competitor-critical content without Jonathan approval.
- Prefer category education, practical workflows, buyer criteria, and honest limitations over generic AI content.
- Keep Adessa positioned broadly as "AI marketing on autopilot," not only "for small businesses."
