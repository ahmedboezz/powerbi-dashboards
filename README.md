# Power BI Dashboards

Eleven Power BI reports built on star-schema models with DAX measures. They are saved as **Power BI Projects (.pbip)**, so the model (TMDL) and the report (PBIR) can be read and diffed in Git. Open any `.pbip` file in Power BI Desktop.

| # | Project | Sector |
|---|---|---|
| 1 | [**E-Commerce Sales Performance**](01-ecommerce-sales) | E-commerce / Retail |
| 2 | [**HR Workforce & Attrition Analysis**](02-hr-attrition) | Human Resources |
| 3 | [**Hospital Inpatient & ER Performance**](03-hospital-performance) | Healthcare |
| 4 | [**Logistics & Carrier Performance**](04-logistics-carriers) | Supply Chain / Logistics |
| 5 | [**Bank Loan Applications & Approvals**](05-bank-loan-applications) | Banking / Finance |
| 6 | [**Restaurant Chain Sales & Operations**](06-restaurant-chain-sales) | Food & Beverage / Hospitality |
| 7 | [**Loan Portfolio & Credit Risk Dashboard**](07-loan-portfolio-credit-risk) | Banking / Credit risk |
| 8 | [**Contact Centre Performance & Customer Experience**](08-contact-center-cx) | Contact centre / CX |
| 9 | [**Digital Marketing ROI Dashboard**](09-digital-marketing-roi) | Digital marketing |
| 10 | [**Fleet Operations & Maintenance Dashboard**](10-fleet-maintenance) | Fleet / Operations |
| 11 | [**Construction Portfolio Control with Earned Value Management**](11-construction-evm) | Construction / Projects |

**Highlights**
- **Loan portfolio & credit risk:** NPL / PAR30, vintage curves, roll-rate matrix, IFRS 9 ECL, semi-additive measures. NPL doubled, and I traced it to a growth-campaign vintage and the broker channel.
- **Contact centre & CX:** SL 80/20, AHT, FCR from 7-day repeat contacts, NPS. Service level drops to 63% on Sundays and 43% in Ramadan.
- **Digital marketing ROI:** merges ad exports from several platforms, with a funnel, budget pacing and a what-if parameter.
- **Fleet maintenance:** cost per km, availability, preventive share. Older vehicles cost 2.3x more per km.
- **Construction EVM:** S-curve, CPI / SPI, project-level EAC, and a SAR 290M forecast overrun after a material price shock.

**Skills:** Power Query (parameters, folder imports, date tables) · star schema and relationships · DAX (CALCULATE, time intelligence, RANKX, iterators, semi-additive measures, what-if) · RLS · report themes and conditional formatting.

> **About the data:** all datasets are simulated to mirror real business systems and include realistic data-quality issues. Company names are fictional. My client work can't be published, so these projects rebuild the same kind of business problems with data I can share.

More projects: [Excel](https://github.com/ahmedsalamsali/excel-dashboards) · [SQL](https://github.com/ahmedsalamsali/sql-projects) · [Python](https://github.com/ahmedsalamsali/python-data-analysis)

---
**Ahmed Abdulsalam** · Data Analyst · Jeddah, Saudi Arabia · a@ezzprx.com · [LinkedIn](https://linkedin.com/in/ahmedboezz)
