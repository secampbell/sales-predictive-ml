# Sales Predictive ML  
Forecasting & Quota-Attainment Classification  

![pipeline](assets/overview_banner.png)

---

## 1 • Project Overview
This repo contains an Azure ML Studio notebook that walks through a **three-part predictive workflow** for a fictional B2B sales organization:

| Task | Goal | Technique |
|------|------|-----------|
| 1. **2025 Full-Year Revenue** | Estimate full-year revenue from half-year YTD figures | ElasticNet & Random Forest regression |
| 2. **2026 Revenue Projection** | Predict next-year revenue using multi-year history & activity features | Random Forest regression |
| 3. **Quota Attainment 2026** | Binary classification → will a rep/territory hit 2026 quota? | Random Forest classifier (ROC ≈ 1.0 on demo data) |

*All numbers are synthetic and “shaped” for demo purposes; focus is on process competence.*

---

## 2 • Dataset
`sales_territories-f.csv` ( ≈ 60 rows × 21 columns )

| Column groups | Examples |
|---------------|----------|
| IDs / hierarchy | `territory_id`, `territory_name`, `region_manager_name` |
| Activity | `active_customers`, `Avg_Deal_Size` |
| Financial history | `sales_2022`-`sales_2025_YTD`, `total_sales` |
| Target flags | `sales_2025_full_year` (engineered), `sales_2026` (predicted), `quota_hit_2026` (engineered binary) |

---

## 3 • Key Notebooks & Scripts

