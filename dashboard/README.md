# Power BI Dashboard Folder

# StormWatch: Severe Weather Intelligence Hub

> **Student note:** Start with `00_START_HERE.md` and `00_TEMPLATE_INDEX.md`. The placeholder files inside this repo are the templates.

**Program:** ZENAIZ x BVRIT Hyderabad Data Engineering Internship Program  
**Track:** Data Engineering  
**Duration:** 12 Weeks  
**Team:** 10  
**Students:** A. Shivani, Nirmala Devi Patel, G. Anusha  
**AI Teammate:** Used responsibly for explanation, debugging, review, and documentation support.

---

## 1. Project Summary

**Domain:** Weather Analytics & Disaster Management.  

**Core engineering problem:** Convert raw weather data from weather stations, satellites, rainfall sensors, temperature records, humidity readings, wind speed measurements, and severe weather alerts into clean, reliable, and real-time insights for monitoring and predicting extreme weather conditions.

**Main pipeline:** Raw Weather Data Sources → Bronze (raw ingestion) → Silver (cleaned & transformed data) → Data Quality Validation → Gold (business-ready weather datasets) → Power BI Dashboard → Streaming Simulation for live severe weather alerts.

**Technologies:** Databricks, Apache Spark, Delta Lake, Power BI, GitHub, and streaming tools.

**Final outcome:** An end-to-end data engineering solution with a GitHub repository, Databricks notebooks, Bronze/Silver/Gold data layers, validated Gold outputs, interactive Power BI dashboards, a streaming simulation of severe weather events, and a final project demonstration.

---

## 2. Tools Used

| Tool | Purpose |
|---|---|
| Databricks Free Edition | Spark SQL notebooks, Python/PySpark, Bronze/Silver/Gold tables, streaming simulation |
| GitHub | Repository, weekly evidence, documentation, screenshots, commits |
| Power BI Desktop | Dashboard from Gold weather datasets |
| AI Assistant | Explanation, debugging, review, documentation support with manual verification |

---

## 3. Repository Navigation

| Folder / File | Purpose |
|---|---|
| `docs/` | Project documentation, weather data dictionary, DQ summary, Gold metric definitions |
| `src/` | Weather data generation and reusable helper scripts |
| `notebooks/` | Databricks notebooks for exploration, Bronze, Silver, DQ, Gold, export, streaming |
| `data_sample/` | Small sample weather datasets only; do not store large files |
| `dashboard/` | Power BI `.pbix` file and dashboard documentation |
| `streaming/` | Streaming design, JSON weather event schema, real-time weather alert simulation |
| `screenshots/` | Weekly evidence screenshots |
| `weekly_logs/` | Weekly execution logs and AI transparency notes |
| `final_submission/` | Final report, demo script, team contribution, checklist |

---

## 4. 12-Week Execution Map

| Week | Focus | Main Evidence |
|---:|---|---|
| 1 | Project framing + GitHub | README, Problem Charter, Week 1 Log |
| 2 | Weather dataset design | Data dictionary, assumptions, sample weather data |
| 3 | Databricks exploration | Exploration notebook, schema/count screenshots |
| 4 | Bronze ingestion | Bronze notebook, raw-to-Bronze reconciliation |
| 5 | Silver standardization | Silver notebook, cleaned weather datasets |
| 6 | Data quality | DQ rules, DQ notebook, DQ summary |
| 7 | Gold metrics | Gold weather tables and metric definitions |
| 8 | Power BI draft | Gold export and first weather dashboard |
| 9 | Dashboard refinement | Final dashboard screenshots and weather insights |
| 10 | Streaming simulation | Structured Streaming notebook and live weather alerts |
| 11 | Integration | Pipeline walkthrough, cleaned README, final evidence |
| 12 | Final demo | Final report, demo script, contribution note |

---

## 5. Important Rules

- Do not connect Power BI directly to raw CSV files. Power BI must use Gold outputs.
- Do not submit copied internet GitHub repositories as your own project.
- External references must be listed in `docs/references.md`.
- AI-generated code or content must be verified and explainable.
- Every week must have a GitHub commit and weekly log.
- Keep sample data small in GitHub. Large generated weather data should be recreated using scripts or uploaded to Databricks separately.

---

## 6. Final Project Proof

By Week 12, this repository should prove:

- We designed weather source datasets.
- We processed batch weather data in Databricks.
- We created Bronze tables.
- We standardized Silver tables.
- We implemented data quality checks.
- We created Gold weather metric tables.
- We built Power BI dashboards from Gold outputs.
- We simulated live weather events using Structured Streaming.
- We documented weekly evidence in GitHub.
- We can explain and defend the complete data engineering pipeline.
