# SplitsPDF

A browser-based tool that splits a large-format PDF page (A0/A2) into a grid of
A4 tiles, ready for printing. Everything runs client-side — your file is never
uploaded anywhere.

## Live site

Once GitHub Pages is enabled, the app is available at:

> https://pepijnreyn.github.io/SplitsPDF/

## Usage

1. Open the site (or open [index.html](index.html) locally in a browser).
2. Choose or drop an A0-size PDF.
3. Pick the grid (4×4, 3×3, or 2×2) and optional overlap for gluing.
4. Click **Split & Download PDF**.

## Development

This is a single static file ([index.html](index.html)) with no build step.
Just open it in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Pushing to `main` triggers the
[deploy workflow](.github/workflows/deploy-pages.yml), which publishes the site
to GitHub Pages automatically.

**One-time setup:** in the repository, go to **Settings → Pages → Build and
deployment** and set the **Source** to **GitHub Actions**.
