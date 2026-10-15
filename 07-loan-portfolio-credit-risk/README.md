# Loan Portfolio & Credit Risk Dashboard (Power BI)

Risk-committee dashboard for a Saudi consumer-finance company: portfolio size, NPL / PAR30, risk drivers, vintage curves, roll rates, collections and simplified IFRS 9 ECL.

> **Note:** simulated data for a realistic business scenario (portfolio case study). Client name withheld/fictional.

| Pages | Model | Measures |
|---|---|---|
| Portfolio Overview · Credit Risk Drivers · Vintage & Roll Rates · Collections & IFRS 9 | Star/snowflake: monthly `Performance` snapshots (162K rows from 36 files) → Loans → Customers / Products / Branches; Date, Bucket, Prev Bucket, Stages | 27 DAX measures in display folders |

**Techniques:** folder ingestion, record-based mapping tables, previous-month bucket via self-merge (roll rates), **semi-additive balance measures**, `TREATAS` virtual relationship for originations, `KEEPFILTERS`, IFRS 9 staging.

## Findings
* NPL rose from **2.5% to 4.9%** in 2025 (PAR30 7.6%) on a SAR 740M book.
* The **H2-2024 growth-campaign vintage** reached 13.7% 30+ DPD at month 12 vs 9.4% for the previous vintage.
* **Broker** loans: 13.6% NPL vs 0.5% via the mobile app. Score < 600: 27.1%. DBR > 45%: 7.7%.
* Early delinquency spikes after Eid (April).

Every measure was validated against an independent Python calculation (DAX queries on the model).
See also: [Logistic-regression driver analysis on the same data](https://github.com/ahmedsalamsali/python-data-analysis/tree/main/03-credit-default-drivers).

## How to open
1. Install a recent **Power BI Desktop** and open `LoanPortfolio.pbip`. The project is saved in the Power BI Project format (TMDL model + PBIR report), so it's readable in Git.
2. Click **Refresh now** (or Home → Refresh → *Schema and data*). If you moved the folder: Transform data → Edit parameters → `DataFolder`.
3. Screenshots of every page are in [`screenshots/`](screenshots).

