# Adessa SEO Content Roadmap - October 2026

## Goal
Recover public crawlability, restart the publishing cadence, and keep compounding durable organic visibility around AI marketing on autopilot, practical campaign workflows, Amazon seller education, and AI-search readiness.

## Status Snapshot - 2026-10-06
- Production curl verification is still blocked by Vercel Security Checkpoint. `/`, `/blog`, latest real blog posts, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, `/for`, and `/for/amazon-sellers` all returned `429` with `x-vercel-mitigated: challenge`.
- Retrying key public SEO surfaces with a Googlebot user agent also returned `429` with `x-vercel-mitigated: challenge`.
- Because `/robots.txt` and `/sitemap.xml` are challenged, current crawl/indexability cannot be treated as healthy until the challenge is removed or Search Console live tests prove Googlebot can fetch the assets.
- The blog repo still contains 14 published posts. No new post files landed after `ai-campaign-launch-checklist` on 2026-06-25.
- The planned URLs `/blog/ai-marketing-for-fashion-brands` and `/blog/sponsored-products-vs-sponsored-brands` are still absent from the post folders and should not be counted as shipped content.
- The `Adessa SEO Blog Publisher` automation is still disabled, with no next run shown in `openclaw automations list --all`.

## Search Console / Bing Data
- Google Search Console data was not checked successfully because the current Google OAuth token for `automate.openclaw@gmail.com` does not include Search Console/Webmasters scope. Token refresh is healthy, but `GET https://www.googleapis.com/webmasters/v3/sites` returned `403 PERMISSION_DENIED` with `ACCESS_TOKEN_SCOPE_INSUFFICIENT` for `google.searchconsole.v1.SitesService.List`.
- `POST https://searchconsole.googleapis.com/webmasters/v3/sites/sc-domain:adessa.ai/searchAnalytics/query` returned the same `403 PERMISSION_DENIED` / `ACCESS_TOKEN_SCOPE_INSUFFICIENT` blocker for `google.searchconsole.v1.searchanalytics.SearchAnalyticsService.Query`.
- No GSC top query, page, impression, click, CTR, indexing, or crawl data was read.
- Bing Webmaster data was not checked. Local checks found no Bing/Webmaster config files, no relevant local CLI (`bing`, `bingsiteauth`, or `gcloud`), and no usable local Bing Webmaster integration.

## Content Shipped Last Week
- No new blog posts landed between 2026-09-29 and 2026-10-06.
- No `docs` or `posts` commits landed in `automate-openclaw/adessa-blog` during that window.
- The latest real published blog post remains **AI Campaign Launch Checklist for Platform-Ready Ads**, published 2026-06-25.
- The previously planned fashion-brand and Amazon ad-type posts did not land as real repo posts.

## This Week's Publisher Plan
- Tuesday 2026-10-06 - **AI Marketing for Fashion Brands: Turn Drops, Content, and Retargeting Into a Weekly Loop**
  - Status: carry-forward because it still has not published; requires publisher automation re-enable or a manual approved publisher run.
  - Target keyword: `AI marketing for fashion brands`
  - Intent: high-intent ICP/use-case education for operators with product launches, seasonal drops, creator assets, and repeat purchase loops.
  - Angle: show how fashion brands can turn product drops, offer windows, creator content, email/social promotion, paid creative, retargeting, and weekly review into one repeatable campaign rhythm without fake performance claims.
  - Internal links: `/for`, `/pricing`, `/blog/ai-campaign-launch-checklist`, `/blog/automated-social-media-marketing`, and `/blog/marketing-automation-for-lean-teams`.
- Thursday 2026-10-08 - **Sponsored Products vs Sponsored Brands: Which Amazon Ad Type Should You Use First?**
  - Status: carry-forward because it still has not published; requires publisher automation re-enable or a manual approved publisher run.
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
- AI Search Visibility Checklist for Lean Marketing Teams - planned backlog; keep claims unverified and avoid promising rankings.

### Cluster 2 - Amazon / High-Intent Posts
- How to Lower ACOS on Amazon in 30 Days - published
- What Is ACOS? A Plain-English Guide for Amazon Sellers - published
- Sponsored Products vs Sponsored Brands - planned 2026-10-08
- Best Amazon PPC Software for Small Sellers in 2026 - hold unless Jonathan approves a non-critical category/listicle approach

### Cluster 3 - ICP Support Posts
- AI Marketing for Restaurants - published
- AI Marketing for Gyms - published
- AI Marketing for Dentists - published
- AI Marketing for SaaS Startups - published
- AI Marketing for Fashion Brands - planned 2026-10-06

## Separate App-Code / Deployment Brief
- Material: public SEO routes remain behind Vercel Security Checkpoint for curl and Googlebot-style requests. Remove the challenge from public SEO surfaces or explicitly allow known crawlers and public assets including `/`, `/blog`, `/blog/*`, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/compare`, and `/for/*`.
- After the challenge is removed, rerun curl verification and use Search Console URL Inspection or Live Test once Search Console scope is available.
- Add Search Console/Webmasters OAuth scope to Jarvis Google auth before the next weekly review if query/page/CTR/index coverage is required.
- Carry-forward app-code checks from prior roadmaps still need a separate approved pass after production is reachable: unknown blog slugs should return a real 404/non-indexable 404 status, homepage should emit a canonical tag, and `llms.txt` should broaden positioning from "for small businesses" toward "AI marketing on autopilot" while staying factual.

## Editorial Guardrails
- No fake claims, fake benchmarks, invented case studies, or unsupported ROI promises.
- No fake review/rating schema.
- No competitor-critical content without Jonathan approval.
- Prefer category education, practical workflows, buyer criteria, and honest limitations over generic AI content.
- Keep Adessa positioned broadly as "AI marketing on autopilot," not only "for small businesses."
