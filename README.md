# Institute of Sports Science Seminar Pages

Static website for the seminar series at the **Institute of Sports Science, Saarland University**, built as a plain HTML + CSS site with no build step.

## Structure

```
.
├── index.html                # Reading Group
├── open-colloquium.html      # Open Colloquium
├── insights.html             # Redirect to new seminar structure
├── publications.html         # Redirect to new seminar structure
├── presentations.html        # Redirect to new seminar structure
├── gatherings.html           # Redirect to new seminar structure
├── members.html              # Redirect to new seminar structure
├── css/style.css             # Shared styles
└── assets/                   # Icons and optional media
```

## Local preview

Open `index.html` directly in a browser, or run any static server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Pages

- `index.html`: Reading Group
- `open-colloquium.html`: Open Colloquium
- Legacy paths redirect to the new two-page seminar structure

## Deploy to GitHub Pages

1. Push to the `main` branch of your GitHub repository.
2. In the repo settings → **Pages**, set:
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
3. The site will be served at `https://<org-or-user>.github.io/<repo-name>/`.

If you want to host at the root domain, rename the repository to `<username>.github.io` instead.

## Updating content

Each page is plain HTML. Edit `index.html` for the Reading Group, `open-colloquium.html` for the Open Colloquium, and `css/style.css` for shared styling.
