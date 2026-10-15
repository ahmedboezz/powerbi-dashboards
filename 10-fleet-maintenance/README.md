# Fleet Operations & Maintenance Dashboard (Power BI)

> **Note:** simulated data for a realistic business scenario (portfolio case study). Client name withheld/fictional.

| Pages | Key measures |
|---|---|
| Fleet Overview · Maintenance · Fuel & Drivers · Replacement Planning | Utilization, availability, cost per km, maintenance cost per km, preventive share, km between breakdowns, L/100 km, idle % |

**Techniques:** telematics cleaning (duplicates, negative odometer deltas), chained merges for fuel cost, period-aware denominators (`COUNTROWS('Date')`), ranked replacement list.

## Findings
* Vehicles 7+ years old cost **1.04 SAR/km** to maintain vs 0.45 for 0-3 years.
* The branch with a **45% preventive share** (vs ~65% elsewhere) has the lowest availability.
* AC failures nearly double in summer (49 work orders in Jun-Aug vs 28 in the other 9 months).
* 12 drivers idle ~3x longer than peers (26.4 vs 21.9 L/100 km).

## How to open
1. Install a recent **Power BI Desktop** and open `FleetOps.pbip`. The project is saved in the Power BI Project format (TMDL model + PBIR report), so it's readable in Git.
2. Click **Refresh now** (or Home → Refresh → *Schema and data*). If you moved the folder: Transform data → Edit parameters → `DataFolder`.
3. Screenshots of every page are in [`screenshots/`](screenshots).
