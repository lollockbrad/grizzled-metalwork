# Grizzled Metalworks

One-of-a-kind metal and reclaimed wood art by **Ken Steelman**.
Built from what gets thrown away — no two pieces alike, nothing made in bulk.

**Repo:** `lollockbrad/grizzled-metalwork`
**Site:** three static pages sharing `styles.css` — no build step, no framework.

## The pages

- **Home** (`index.html`) — hero ("Built from what gets thrown away"), featured work,
  About the Maker, how a piece is made (find it → see it → build it → sell it in person),
  Next Show (XMAS Extreme Metal Art Show, **Saturday, December 5, 2026, 1:00–5:00 PM**,
  So Metal Global Headquarters, 76296 Industrial Park Way, Oakridge, OR — live countdown,
  Add to Calendar, directions, and the show poster), and How to Buy
- **Gallery** (`gallery.html`) — Ken's actual work, grouped: Metal Camper Trailer,
  Motorcycle Trike, Scrap Tractors, and On the Workbench. Tap a photo for full size.
- **Contact Us** (`contact.html`) — meet Ken at the Dec 5 show, farmers markets,
  and how buying a one-of-a-kind piece works. Ready for Ken's email / Etsy link
  the moment he shares one — no contact info is published yet because none has been given.

## Deployment — Vercel auto-deploys from GitHub

This repo is connected to Vercel. **Every push to the `main` branch auto-builds and auto-deploys:**

1. Push a change to `main` on GitHub (or merge a pull request into `main`)
2. Vercel detects the push, builds the site, and deploys it automatically
3. The live site updates on its own — no manual deploy step

Pull requests get their own preview deployment from Vercel, so a change can be
checked on a preview link before it merges to `main` and goes live.

### Vercel settings for this site

| Setting | Value |
|---|---|
| Framework preset | Other (static) |
| Build command | None — leave empty |
| Output directory | Root of the repo (leave default / empty) |
| Install command | None — leave default |

`vercel.json` in the repo root turns on clean URLs. That's the only config.

## Making changes

Copy lives in the page files (`index.html`, `gallery.html`, `contact.html`);
shared styling lives in `styles.css`. Edit, commit, push to `main`, and Vercel does the rest.
You can also edit any file right on GitHub: open the file, click the pencil icon,
change the text, and commit — that's a push, so the live site updates on its own.

## SEO — where everything lives

There's no SEO plugin here; the SEO fields are lines in each page's `<head>`,
near the top of the file. Same fields Yoast gives you, just typed instead of form-filled:

| SEO element | Where it is |
|---|---|
| SEO title | The `<title>` line in each page's `<head>` |
| Meta description | The `<meta name="description" ...>` line under it |
| H1 / headings | The `<h1>`, `<h2>`, `<h3>` tags in the page body — one H1 per page |
| Image alt text | The `alt="..."` inside each `<img>` tag |
| Clean URLs | `vercel.json` (`cleanUrls`) — pages serve as `/gallery`, not `/gallery.html` |
| Crawl access | `robots.txt` — currently allows everything |

Page targets (one intent per page, no overlap):
Home = Grizzled Metalworks / Ken Steelman brand · Gallery = his pieces ·
Contact = how to reach / buy from Ken.

Still to add once the live URL is confirmed: `sitemap.xml`, the sitemap line in
`robots.txt`, Open Graph share tags, and Google Search Console verification.

## Still to add

- [x] Photos of Ken's actual pieces — added Nov 15, 2026 (camper trailer, motorcycle trike, tractors, workbench group shot, show poster; web copies are resized with location/EXIF data stripped)
- [ ] Ken's contact info and/or Etsy link, when he's ready to share them
- [ ] Specific farmers market dates and locations
