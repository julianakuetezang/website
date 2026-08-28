# Juliana Kuetezang — Personal Website

A single-page, fully static site (no build step) ready for **GitHub Pages**.

```
.
├── index.html                 ← the whole site
├── assets/
│   ├── img/                    ← portraits + video poster frames
│   ├── vid/                    ← introduction.mp4, forgeforth-demo.mp4 (web-compressed)
│   └── doc/Juliana-Kuetezang-CV.pdf
└── README.md
```

## Deploy to GitHub Pages (5 minutes)

**Option A — user site (`juliana.github.io`)**
1. Create a repo named exactly **`<your-username>.github.io`**.
2. Upload every file here, keeping the folder structure (`index.html` at the repo root).
3. **Settings → Pages → Deploy from a branch → `main` / `root`**, Save.
4. Live in ~1 minute at `https://<your-username>.github.io`.

**Option B — project site (`<username>.github.io/<repo>`)**
1. Create any repo, upload these files.
2. **Settings → Pages → Deploy from a branch → `main` / `root`**.

### Command line
```bash
git init && git add . && git commit -m "Launch personal website"
git branch -M main
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main
```

## About the videos
- Both videos were re-encoded for the web. The original `Introduction_video.mp4` was 178 MB — **over GitHub's 100 MB per-file limit** — and is now 6.5 MB; the product demo is 4.1 MB. They load on demand (`preload="none"`), so the page stays fast.
- To swap a video, replace the file in `assets/vid/` (keep the filename) and update its poster in `assets/img/`.

## Adding more photos
Only two photos were supplied directly, so the site uses them prominently. The Google Drive links you shared (Clothe-our-community and Forgeforth) couldn't be pulled in automatically — Drive folders need sign-in. To add a photo gallery later:
1. Drop web-sized JPGs (long edge ~1200 px) into `assets/img/`.
2. Tell me which section (e.g. a "Life of Purpose in action" gallery) and I'll wire them in — or copy the gallery pattern from the sister site.

## Editing
- All copy lives in `index.html` — search a phrase and edit in place.
- Colours/fonts are CSS variables at the top of `<style>` (`--ink`, `--coral`, `--gold` …).
- Section numbering uses an accounting motif ("Note 01, Note 02 …") — keep it sequential if you add sections.

## Notes
- Name shown as **Juliana Kuetezang** (matches KPMG, LinkedIn, and email); the fuller "Ngongni Kuetezang" can be added if preferred.
- Phone number and home address were intentionally **left off** the public page for privacy — email + LinkedIn only. Add them in the contact block if wanted.
- Custom domain: add a `CNAME` file with the domain and configure DNS per GitHub's docs.
