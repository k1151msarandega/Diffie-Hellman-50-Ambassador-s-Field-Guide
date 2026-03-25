# Dynamic Knowledge Repository — Ambassador's Field Guide

This repository is organized as a multi-volume GitHub Pages site with chronological navigation from **Volume 1 → Volume 2 → Volume 3**.

## Repository tree (chronological)

```text
.
├── index.html                                  # Root landing page listing Volumes 1, 2, 3
├── volume-1/
│   └── index.html                              # Volume 1 — Coming Soon
├── volume-2/
│   └── index.html                              # Volume 2 — Coming Soon
└── volume-3/
    ├── index.html                              # Volume 3 landing page
    ├── module-0-welcome.html                   # Optional prelude: Orientation
    ├── module-a-foundations.html               # Module A — Foundations
    ├── module-b1-post-quantum.html             # Module B1 — Post-Quantum Transition
    ├── module-b2-ai-governance.html            # Module B2 — AI Governance & Verifiable Trust
    ├── module-b3-digital-sovereignty.html      # Module B3 — Digital Sovereignty & DPI Models
    ├── module-b4-digital-inclusion.html        # Module B4 — Digital Inclusion & the Trust Gap
    ├── module-b5-your-own-track.html           # Module B5 — Your Own Track
    ├── module-c-going-public.html              # Module C — Going Public
    └── module-d-log-global-connector.html      # Module D — Ambassador Log & Global Connector
```

## Volume 3 module sequence

On `volume-3/index.html`, modules are ordered as requested:

1. **Module A — Foundations**
2. **Module B — Scenario Tracks** (expandable parent with nested **B1–B5**)
3. **Module C — Going Public**
4. **Module D — Ambassador Log & Global Connector**

`Module 0 — Orientation` is preserved as an optional prelude link at the top of the page.

## Run locally

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.


## GitHub Pages 404 troubleshooting

If you see a GitHub Pages 404 when opening a module URL, it is usually one of these issues:

- The URL path doesn't match the file path exactly (including lowercase/uppercase).
- You used an outdated URL after files were reorganized.
- Pages is still deploying and the latest commit is not live yet.
- You opened `/volume-3` (no trailing slash) instead of `/volume-3/` or `/volume-3/index.html`.

Canonical module locations are under `volume-3/`. Use those paths directly.

## GitHub Pages setup

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** default branch (for example `main`), folder `/ (root)`
4. Save and wait for deployment.

### Expected URLs after deploy

- Project root: `https://<username>.github.io/<repo>/`
- Volume 3 landing: `https://<username>.github.io/<repo>/volume-3/`
- Example module: `https://<username>.github.io/<repo>/volume-3/module-a-foundations.html`

## How ambassadors can fork and contribute

1. Fork the repository.
2. Create a branch:

   ```bash
   git checkout -b my-ambassador-updates
   ```

3. Update module pages, add references/exercises, or extend Volume 1/2 stubs.
4. Run locally and verify links.
5. Commit and open a pull request.
