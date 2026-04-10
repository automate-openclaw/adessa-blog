# Adessa Blog Content

Blog posts for adessa.ai. Managed by Jarvis, published automatically.

## Structure

```
posts/
  post-slug/
    index.md       — post content (markdown + inline HTML/CSS)
    meta.json      — title, excerpt, author, date, tags, reading time
    hero.jpg       — hero/cover image
    *.png/jpg      — any inline images referenced in index.md
assets/
  shared/          — reusable brand images, icons, graphics
```

## How It Works

1. Jarvis creates a new folder under `posts/`
2. Writes `index.md` (content) + `meta.json` (metadata) + images
3. Pushes to this repo
4. Adessa.ai fetches posts from this repo at build time via GitHub API
5. Posts go live automatically via Vercel ISR (revalidates every 60s)

## Content Format

`meta.json`:
```json
{
  "title": "Post Title",
  "subtitle": "Optional subtitle",
  "excerpt": "1-2 sentence summary for blog index and SEO",
  "author": { "name": "Adessa Team", "role": "Marketing" },
  "publishedAt": "2026-04-10",
  "updatedAt": null,
  "readingTimeMin": 7,
  "tags": ["ai-marketing", "social-media"],
  "status": "published",
  "coverImage": "hero.jpg"
}
```

`index.md`: Standard markdown with support for inline HTML/CSS.
Images referenced as relative paths (e.g., `![diagram](./diagram.png)`).
