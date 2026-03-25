# Dynamic Knowledge Repository — Ambassador's Field Guide

This repository is structured as a multi-volume GitHub Pages site for ambassador learning journeys, scenario analysis, and public contribution.

## Site structure

```text
.
├── index.html                                  # Volume 3 landing page
├── module-0-welcome.html                       # Module 0 — Orientation
├── module-a-foundations.html                   # Module A — Foundations
├── module-b1-post-quantum.html                 # Module B1 — Post-Quantum Transition
├── module-b2-ai-governance.html                # Module B2 — AI Governance & Verifiable Trust
├── module-b3-digital-sovereignty.html          # Module B3 — Digital Sovereignty & DPI Models
├── module-b4-digital-inclusion.html            # Module B4 — Digital Inclusion & the Trust Gap
├── module-b5-your-own-track.html               # Module B5 — Your Own Track
├── module-c-going-public.html                  # Module C — Going Public
├── module-d-log-global-connector.html          # Module D — Ambassador Log & Global Connector
├── volume-1/
│   └── index.html                              # Volume 1 stub
└── volume-2/
    └── index.html                              # Volume 2 stub
```

## How to run locally

1. Clone the repository.
2. Open `index.html` directly in a browser, **or** run a lightweight local server:

   ```bash
   python -m http.server 8000
   ```

3. Navigate to `http://localhost:8000`.

## GitHub Pages setup

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, select:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (or your default branch), `/ (root)`
4. Save and wait for deployment.

## How ambassadors can fork and contribute

1. **Fork** this repository to your GitHub account.
2. **Create a branch** for your contribution:

   ```bash
   git checkout -b add-module-content
   ```

3. Add or update module content pages (for example, adding new prompts, activities, logs, or references).
4. Test locally in browser to ensure links and layout still work.
5. Commit your changes:

   ```bash
   git add .
   git commit -m "Add module content updates"
   ```

6. Push your branch and open a pull request to your fork or upstream project.

### Contribution ideas

- Add guided exercises and region-specific case studies.
- Add reading lists or source references per module.
- Add multilingual variants of module pages.
- Extend Volume 1 and Volume 2 beyond their current stubs.

## Design notes

- A shared visual style is used across the landing page, module pages, and volume stubs.
- Volume 3 uses cards for top-level modules.
- Module B is expandable and reveals B1–B5 sub-cards.
