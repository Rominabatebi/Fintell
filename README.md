# Fintell website

The public website for **Fintell**: an AI financial intelligence platform for CEOs, CFOs and investors.

- **Live site:** `https://YOUR-GITHUB-USERNAME.github.io/fintell-website/` (after step 4 below)
- **Founder:** Romina Golfam Batebi · batebi.golfam@gmail.com

## What's in this folder

```
fintell-website/
├── index.html              The whole website: 10 pages (home, platform, CEOs, CFOs, investors, pricing, data, security, CPI, about)
├── .nojekyll               Tells GitHub Pages to serve the files as they are
├── README.md               This file
└── assets/
    ├── img/                Logo, favicon, video posters, founder photo, link-preview image
    └── video/              The three product walkthroughs (investor, CEO, CFO)
```

## Put it online with GitHub Pages (about 5 minutes, free)

1. **Create a GitHub account** at github.com if you don't have one.
2. **Create a repository:** click **+ → New repository**, name it `fintell-website`, choose **Public**, and click **Create repository**.
   GitHub Pages is free only for public repositories. Don't upload your R source code here.
3. **Upload the files:** on the new repository page, click **uploading an existing file**. Open the unzipped `fintell-website` folder on your computer, select **everything inside it** (`index.html`, `README.md`, the `assets` folder) and drag it into the browser. Click **Commit changes**.
   The `.nojekyll` file is hidden on most computers; the site works without it.
4. **Switch on Pages:** go to **Settings → Pages**. Under **Build and deployment**, choose **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**, and click **Save**.
5. **Wait about a minute**, then refresh the Pages settings. Your link appears at the top:
   `https://YOUR-GITHUB-USERNAME.github.io/fintell-website/`

To update the site later, upload a changed file with the same name. GitHub replaces it and republishes within a minute.

## Live public data (no keys needed)

When the page opens, the visitor's browser calls these free public APIs directly. If one doesn't answer within six seconds, the page keeps the dated snapshot and labels it. The **Data & APIs** page shows the status of every source.

| Data | Provider | API |
|---|---|---|
| ECB deposit and main refinancing rates | European Central Bank | ECB Data Portal (`data-api.ecb.europa.eu`) |
| €STR, euro short-term rate | European Central Bank | ECB Data Portal |
| 10-year euro yield (AAA yield curve) | European Central Bank | ECB Data Portal |
| Inflation, euro area and Austria (HICP) | ECB / Eurostat | ECB Data Portal |
| Real GDP growth, Austria | Eurostat | Eurostat Statistics API |
| Unemployment, euro area | Eurostat | Eurostat Statistics API |
| Euro exchange rates and 12-month history | ECB, via Frankfurter | `api.frankfurter.dev` |
| GDP growth: Austria, Germany, EU, US | World Bank | World Bank Indicators API |

Fixed datasets, updated by hand: EV/Sales multiples (Damodaran Online, January 2026), Euro Stoxx 50 closes (Investing.com), and the industry betas and risk premia from the Fintell prototype.

**Updating the snapshot:** search `index.html` for `const MARKET` and change the numbers and dates. The `SRC` list right below it holds each source's name, link and "as of" date.

## Use your own domain (optional)

Buy a domain (for example `fintell.at`), then in **Settings → Pages → Custom domain** enter it and follow GitHub's instructions for the DNS records.

## Honesty notes shown on the site

- The product is a working prototype. Demo figures are synthetic.
- Prices are proposed pilot prices, not validated offers.
- No security certifications are claimed.
- Nothing on the site is investment advice.
