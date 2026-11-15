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

Edit `index.html` — all copy, styling, and the show countdown live in that one file.
Commit, push to `main`, and Vercel does the rest.

## Still to add

- [x] Photos of Ken's actual pieces — added Nov 15, 2026 (camper trailer, motorcycle trike, tractors, workbench group shot, show poster; web copies are resized with location/EXIF data stripped)
- [ ] Ken's contact info and/or Etsy link, when he's ready to share them
- [ ] Specific farmers market dates and locations
