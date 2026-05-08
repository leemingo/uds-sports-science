# KAISports Homepage

Static website for **KAISports — Korea AI Research Society for Sports** (한국스포츠인공지능연구회), built as a GitHub Pages–ready static site (HTML + CSS, no build step).

## Structure

```
.
├── index.html           # Home
├── publications.html    # Publications (2021–2026)
├── presentations.html   # Talks, conference & invited presentations
├── gatherings.html      # Offline gatherings
├── members.html         # Coordinators & members
├── css/style.css        # Shared styles
└── assets/              # (optional) member photos, logos, etc.
```

## Local preview

Open `index.html` directly in a browser, or run any static server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy to GitHub Pages

1. Push to the `main` branch of `github.com/KAISport/homepage`.
2. In the repo settings → **Pages**, set:
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
3. The site will be served at `https://kaisport.github.io/homepage/`.

If you want to host at the root domain `https://kaisport.github.io/`, rename the repository to `kaisport.github.io` instead.

## Adding member photos

Member cards currently use initial-based avatars. To use real photos:

1. Add image files under `assets/members/` (e.g. `assets/members/sang-ki-ko.jpg`).
2. In `members.html`, replace the `<div class="avatar initials">SK</div>` element with:
   ```html
   <div class="avatar" style="background-image: url('assets/members/sang-ki-ko.jpg');"></div>
   ```

## Updating content

Each page is plain HTML — edit the relevant file directly. Publications are grouped by year inside `publications.html`; add a new `<li class="pub-item">…</li>` block to the appropriate year section.

## Contact

thedatadribblers [at] gmail.com
