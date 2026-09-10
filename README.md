# Wonderland

A curated guide to beginner-friendly surf spots along the Agadir coast, Morocco.

**Live site:** https://adek1252ai.github.io/Wonderland/

## What it is

Wonderland gathers the surf breaks within driving distance of Agadir and filters them down to the ones that make sense for someone standing on a board for the first time. Every spot is rated for beginner suitability, with notes on bottom type, crowd levels, best season, and where to find a surf school.

Currently **12 spots** covered, from Agadir city beach north to Taghazout and south toward Tiznit.

## The spots

1. **Agadir Beach** — city beach, 0 km
2. **Anza** — 5–10 km north
3. **Cross** — harbour point, Agadir city
4. **Cherry Cherry Beach** — Inezgane, south of Agadir
5. **Crocro Beach** — 14 km north, Tamraght
6. **Banana Point (Aourir)** — 25 km north, Tamraght
7. **Banana Beach (Tamraght)** — 15 km north, safest beginner beach
8. **Panoramas** — 20–24 km north, Taghazout first-lesson spot
9. **Hash Point** — Taghazout village, walk-to break
10. **Devil's Rock (inside whitewater)** — 15 km north, protected teaching wave
11. **Tifnit** — ~60 min south, uncrowded
12. **Aglou Beach** — ~90 min south near Tiznit, underrated

## Stack

- Single `index.html` + `css/style.css` + `img/favicon.svg`
- Hand-written HTML, CSS, and vanilla JS — no frameworks, no build step
- Google Fonts (DM Sans + Playfair Display)
- Deployed via GitHub Pages

## Developing

Open `index.html` in a browser, or serve locally:

```bash
cd Wonderland
python3 -m http.server 8000
# → localhost:8000
```

## Data

Spot content lives in the `<script>` block at the bottom of `index.html` as a `spots` array. Each entry:

```js
{
  emoji, name, tag, distance, description,
  details: { waveType, typicalSize, bestSeason, bottom },
  difficulty, diffClass, notes
}
```

Add or edit entries there. Research sources:

- `agadir-beginner-surf-spots.json` — first research batch
- `morocco-beginner-surf-spots.json` — second research batch

## Deploying

The site is published on GitHub Pages from the `main` branch. Pushing to `main` triggers a rebuild:

```bash
git add -A
git commit -m "Update spots"
git push origin main
```

## License

Public domain — ride free.
