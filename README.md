# Office Services Operations Dashboard

Static proof-of-concept dashboard for the seven regional facilities. The current app is a self-contained `index.html` with sample data and the visible `SAMPLE - for PoC only` watermark.

## Local preview

Open `index.html` in a modern browser. No build step or package installation is required.

## Publish with GitHub Pages

1. Create a GitHub repository and push this project to its `main` branch.
2. In the repository, open **Settings → Pages** and select **GitHub Actions** as the build and deployment source.
3. Each push to `main` will publish the static site. The workflow is in `.github/workflows/pages.yml`.

## Data and privacy

This is a sample-only, static proof of concept. Dashboard figures are illustrative. Do not enter or commit real employee identity numbers, email addresses, meal selections, or operational records. The current meal screen does not provide secure durable storage or send email; those require a protected server-side service. Git history retains committed content even after a file is later changed.

GitHub Pages serves files to visitors and should not be treated as a private database. For production use, keep the source repository private where appropriate and use an authenticated server-side API and access-controlled data store for live records. Never put a GitHub token in browser code or commit secrets.
