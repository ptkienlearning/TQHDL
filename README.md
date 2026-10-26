# Urban Retail Intelligence — HCMC 2025

A static, interactive data visualization website for the Midterm Project.

## Files
- `index.html` — webpage structure
- `style.css` — responsive layout and visual design
- `app.js` — filters, charts, KPIs, table, and CSV export
- `data.js` — embedded transaction dataset (240 rows)

## Run locally
Open `index.html` in a modern browser. Internet access is required for Chart.js and Google Fonts CDN resources. The transaction data is bundled locally in `data.js`; no backend or build step is required.

## Deploy to GitHub Pages
1. Rename this folder/repository to the required name: `<YOUR_MSHV>_DataViz_Midterm` (replace the placeholder with your actual student ID).
2. Create a GitHub repository with that name.
3. Upload `index.html`, `style.css`, `app.js`, `data.js`, and `README.md` to the repository root.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main`, folder `/ (root)`, and click **Save**.
7. Wait for the Pages deployment to finish. The URL will look like:
   `https://YOUR-USERNAME.github.io/YOUR_MSHV_DataViz_Midterm/`
8. Open the published URL in a private/incognito window and verify filters, charts, table, and CSV export.

## Data and interpretation notes
- Currency values are displayed in the dataset's original units. The CSV does not independently establish a currency label, so the dashboard does not assert one.
- Missing customer ratings and delivery times are not treated as zero.
- The findings describe this 240-transaction dataset and are not causal claims.
- Charts and KPI cards update with store, category, customer type, month, and transaction search filters.
- The website uses Chart.js via CDN. For a fully offline copy, download Chart.js and reference the local file instead.

## Submission checklist
The assignment asks for the webpage/project name `<MSHV>_DataViz_Midterm` and a PDF named `<MSHV>.pdf` containing student name, MSHV, and the deployed URL.
