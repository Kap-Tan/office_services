# Office Services Operations Dashboard

Static proof-of-concept dashboard for the seven regional facilities. The current app is a self-contained `index.html` with the visible `SAMPLE - for PoC only` watermark.

## Local preview

Open `index.html` in a modern browser. No build step or package installation is required.

## Publish with GitHub Pages

1. Push this project to the repository's `main` branch.
2. In **Settings → Pages**, select **Deploy from a branch**, choose `main` and the root (`/`) folder.
3. GitHub Pages publishes the dashboard. Data files under `data/` are committed to the same public repository and are publicly readable.

## Saving demo data to GitHub

The dashboard writes service records, reusable meal menus, and demo meal selections to `data/service-records.json`, `data/meal-menus.json`, and `data/meal-selections.json` through the GitHub Contents API. On first load, the app reads those files. To save, choose **Connect GitHub to save** and enter a fine-grained personal access token limited to `Kap-Tan/office_services` with **Contents: Read and write** permission. The token is kept only in the current browser tab's memory; closing or refreshing the tab clears it. Each save creates a commit on `main`, which can trigger a GitHub Pages refresh.

This is a public proof of concept. Anyone can read the data files and the Git history retains committed values, including after a later edit or deletion. Enter fake demo identities and email addresses only. The app does not send confirmation emails. Do not use this token-based browser flow for production or sensitive information; a production service needs an authenticated server-side API and access-controlled database.
