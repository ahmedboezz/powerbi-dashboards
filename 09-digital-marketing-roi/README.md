# Digital Marketing ROI Dashboard (Power BI)

> **Note:** simulated data for a realistic business scenario (portfolio case study). Client name withheld/fictional.

| Pages | Key measures |
|---|---|
| Marketing Overview · Channel Efficiency · Website Funnel · Budget & What-if | Spend, ROAS, CAC, CTR, CPC, CPM, CVR, budget pacing, funnel rates, what-if projections |

**Techniques:** one rename map + `MissingField.Ignore` to combine Google / Meta / other ad exports with different schemas, unpivoted funnel, channel-relative spend bands (diminishing returns) and a **what-if parameter**.

## Findings
* Total spend SAR 26.3M at **ROAS 3.40x**. Google Search 5.33x vs Display 1.64x.
* Diminishing returns: ROAS 4.12x on low-spend days vs 2.39x when daily spend doubles.
* Snapchat overspent its November budget by 38%, and November ROAS fell to 2.75x.
* An August sales dip came from **checkout completion falling to 47%**, a payment problem rather than a marketing one.

## How to open
1. Install a recent **Power BI Desktop** and open `MarketingROI.pbip`. The project is saved in the Power BI Project format (TMDL model + PBIR report), so it's readable in Git.
2. Click **Refresh now** (or Home → Refresh → *Schema and data*). If you moved the folder: Transform data → Edit parameters → `DataFolder`.
3. Screenshots of every page are in [`screenshots/`](screenshots).
