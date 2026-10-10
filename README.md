# lauren-mee.com

Static portfolio site for Lauren Mee, hosted on GitHub Pages at lauren-mee.com. No build step.

## Files
- `index.html` — the whole site: one shadowbox per project
- `images/` — the photos for each shadowbox (see below)
- `CNAME` — tells GitHub Pages to serve at www.lauren-mee.com (lauren-mee.com redirects there)
- `.nojekyll` — skips Jekyll processing

## Adding photos
Each shadowbox looks for numbered JPGs in its own folder. Any slot without a photo shows a striped "photo" placeholder, so you can fill them in gradually.

| Shadowbox | Folder | Slots |
|---|---|---|
| Marvel's Wolverine | `images/wolverine/` | 1.jpg – 4.jpg |
| Marvel's Spider-Man 2 | `images/spider-man-2/` | 1.jpg – 4.jpg |
| Ratchet & Clank: Rift Apart | `images/rift-apart/` | 1.jpg – 3.jpg (2.jpg is a portrait slot) |
| The Walking Dead: The Final Season | `images/the-walking-dead/` | 1.jpg – 3.jpg |
| Batman: The Enemy Within | `images/batman/` | 1.jpg – 3.jpg |

Tips:
- Landscape photos work best (4:3). They are cropped to fit, so keep the subject near the center.
- Keep each file around 1200px wide and under ~400 KB so the page loads fast.
- File names are case-sensitive on GitHub: `1.jpg`, not `1.JPG`.
- To add a handwritten caption under a polaroid, add `<figcaption>Your caption</figcaption>` right after its `</div>` inside the `<figure>`.

Moving a photo or sticker: each one has `--x` / `--y` (position, % of the collage), `--w` (width, %) and `--r` (rotation) in its `style`.

## Before publishing
1. Confirm the Batman: The Enemy Within WGA nomination wording.

## Deploy
Upload everything to the root of the repo's `main` branch. GitHub Pages republishes within a minute or two.
