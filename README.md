# Sujeet Gaikwad — Portfolio

Personal portfolio site. Single self-contained `index.html`: no build step, no npm install,
no framework. Open it in a browser and it works.

**Live:** https://sujgaik2003.github.io/Portfolio-suj/

---

## Push this to GitHub

From the folder containing these files:

```bash
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/Sujgaik2003/Portfolio-suj.git
git push -u origin main
```

If the repo already has commits, use `git push -u origin main --force` (this overwrites it).

## Turn on GitHub Pages

Repo → **Settings** → **Pages** → Source: **Deploy from a branch** → Branch: `main` → Folder: `/ (root)` → **Save**.

Live in ~60 seconds at `https://sujgaik2003.github.io/Portfolio-suj/`.

---

## What's here

| File | Purpose |
| --- | --- |
| `index.html` | The entire site — HTML, CSS, JS, icons and your photo, all inline |
| `assets/sujeet.jpg` | Your portrait, cropped to 4:5 (the same image is already embedded in `index.html`) |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Design system

| | |
| --- | --- |
| **Palette** | Void black `#08090B` + a single amber signal `#FFB627`. Warm amber on black instead of the usual AI blue/purple — it's the colour of an instrument panel, a warning lamp, and EY's own brand yellow. |
| **Type** | `Archivo` (expanded, industrial) for display · `IBM Plex Sans` for body · `IBM Plex Mono` for all data, dates and IDs. Plex because you hold three IBM certifications and it's the native typeface of enterprise technical docs. |
| **Signature** | **Fig. 1** in the hero — a self-drawing PPO episode-reward curve: noisy and unstable early, converging late. It's the shape of your DRDO humanoid-walking work, used as the page's thesis. |
| **Structure** | Projects that produced a formal artifact carry a link marker to it (`Political_News → Patent 2025/05214`, `Stock-Market → IEEE 10503557`). The markers encode something true, not decoration. |

## Things you should change

1. **Verify the certificate links.** You gave four Coursera IDs without saying which is which. They're currently mapped in the order you listed them:

   | Card | Certificate | Coursera ID |
   | --- | --- | --- |
   | C-01 | Continuous Integration and Continuous Delivery (CI/CD) — IBM | `SAZLJGF93JWF` |
   | C-02 | Generative AI with Large Language Models — DeepLearning.AI | `04VRBVHNHUZC` |
   | C-03 | Application Security for Developers and DevOps — IBM | `OWMAQ0L9KIF9` |
   | C-04 | Python for Data Science, AI & Development — IBM | `8QB7LKQ73H31` |

   Click each one. If a link opens the wrong certificate, swap the IDs in the `#certs` section.
   (The first cert's full title was cut off in your screenshot — confirm it's the CI/CD one.)

2. **Read the About copy.** It's written in your voice but it's my draft, not your words. Change anything that doesn't sound like you.

3. **Fig. 1 is a representative curve, not your logged data** — and the caption says so. To use your real run, replace the `RAW` array in the `FIG.1` block of the script with your actual reward values (any length; it normalises to 0–1).

4. **Company logos are typographic monograms** (`EY`, `HTS`, `DRDO`, `VIIT`, `APS`, `IBM`), not real brand marks — you asked for no images beyond your photo, and reproducing employer logos is a trademark question you don't need. To use real logos, replace the `.job__logo` contents with an `<img>`.

5. **Swap your photo** by replacing `assets/sujeet.jpg` and changing the `<img src="data:image/jpeg;base64,...">` in `index.html` back to `src="assets/sujeet.jpg"`.

## Built to a quality floor

- Responsive from 320px to ultrawide
- `prefers-reduced-motion` fully respected — every animation drops out
- Visible keyboard focus on every interactive element
- No `localStorage`, no cookies, no trackers, no analytics
- Fonts from Google Fonts; everything else is inline. One HTTP request for the page.

---

© Sujeet Gaikwad
