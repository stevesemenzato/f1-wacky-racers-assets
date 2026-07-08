# f1-wacky-racers-assets

Public CDN source for the **processed visual hero assets** used by the F1 Wacky
Racers fantasy companion app. This repo intentionally contains **only images** —
no application code, spreadsheet data, tokens, or player data live here.

## Layout
```
assets/
  gp-hero/       # per-Grand-Prix opening hero photos, keyed by circuit
  sprint-hero/   # sprint-weekend hero variants (staged)
```

Files are named by the app's circuit key (e.g. `monza.jpg`, `madrid.jpg`,
`las-vegas.jpg`), downscaled to ≤1600px and JPEG-compressed. The app references
them via jsDelivr:

```
https://cdn.jsdelivr.net/gh/stevesemenzato/f1-wacky-racers-assets@main/assets/gp-hero/<key>.jpg
```

Any key with no file falls back gracefully to the app's generated gradient hero.

## Note on imagery
These are Formula 1 race photographs used for a private, non-commercial fantasy
league companion. Rights remain with their respective photographers/rights
holders. Replace any asset with a licensed/original image as needed.
