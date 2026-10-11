# StormWatch — Storm Event Analytics and Risk Dashboard

> **Student note:** Start with `00_START_HERE.md` and `00_TEMPLATE_INDEX.md`. The placeholder files inside this repository are the templates.

**Program:** ZENAIZ x BVRIT Hyderabad Data Engineering Internship Program  
**Track:** Data Engineering  
**Duration:** 12 Weeks  
**Team:** Team 09  
**Students:** ANUSHA, SHIVANI, NIRMALA  
**AI Teammate:** Used responsibly for explanation, debugging, review, dashboard design guidance, and documentation support, with manual verification.

---

## 1. Project Summary

- **Domain:** Weather, severe storms, and natural hazard analytics.
- **Core engineering problem:** Transform raw storm-event data into standardized, validated, and trustworthy analytical datasets that support the analysis of storm frequency, fatalities, injuries, and reported damage.
- **Main pipeline:** Raw Sources → Bronze → Silver → Data Quality → Gold → Power BI → Streaming Simulation.
- **Data Engineering:** Use Databricks and Spark SQL/PySpark to ingest, standardize, validate, and aggregate storm-event data.
- **Data Quality:** Apply validation checks to improve data consistency, identify missing or invalid values, and verify the reliability of analytical outputs.
- **Gold Analytics:** Create curated Gold tables and summary metrics for storm events, event types, hazard groups, fatalities, injuries, and damage severity.
- **Power BI:** Build interactive dashboards with KPI cards, trend charts, event distribution visuals, impact analysis, tables, and filters for year, state, and hazard group.
- **Final outcome:** A documented GitHub repository containing Databricks notebooks, Gold outputs, Power BI dashboards, data-quality evidence, a streaming simulation, weekly logs, and final presentation materials.

---

## 2. Tools Used

| Tool | Purpose |
|---|---|
| Databricks Free Edition | Spark SQL, Python/PySpark, data ingestion, Bronze/Silver/Gold processing, data quality checks, and streaming simulation |
| GitHub | Source control, project documentation, weekly logs, screenshots, and implementation evidence |
| Power BI Desktop | Interactive dashboards built from curated Gold outputs |
| Python / PySpark | Data transformation, standardization, validation, and reusable processing logic |
| Spark SQL | Data exploration, aggregation, reconciliation, and analytical metric creation |
| AI Assistant | Explanation, debugging, code review, Power BI guidance, and documentation support, followed by manual verification |

---

## 3. Repository Navigation

| Folder / File | Purpose |
|---|---|
| `00_START_HERE.md` | Initial project instructions and onboarding |
| `00_TEMPLATE_INDEX.md` | Index of repository templates |
| `README.md` | Project overview, architecture, setup, and navigation |
| `docs/` | Project documentation, data dictionary, data-quality summary, Gold metric definitions, and references |
| `src/` | Data generation scripts and reusable data-quality helper functions |
| `notebooks/` | Databricks notebooks for exploration, Bronze ingestion, Silver standardization, data quality, Gold processing, export, and streaming |
| `data_sample/` | Small sample datasets and approved Gold exports for demonstration and Power BI development |
| `dashboard/` | Power BI `.pbix` file, dashboard screenshots or notes, and usage instructions |
| `streaming/` | Streaming architecture, JSON event schema, simulation design, and implementation notes |
| `screenshots/` | Weekly evidence, notebook outputs, data-quality results, and dashboard screenshots |
| `weekly_logs/` | Weekly execution logs, progress records, and AI transparency notes |
| `final_submission/` | Final report, demonstration script, team contribution statement, and submission checklist |

---

## 4. 12-Week Execution Map

| Week | Focus | Main Evidence |
|---:|---|---|
| 1 | Project framing and GitHub setup | README, problem charter, Week 1 log |
| 2 | Dataset design and source planning | Data dictionary, assumptions, sample data plan |
| 3 | Databricks exploration | Exploration notebook, schema and record-count screenshots |
| 4 | Bronze ingestion | Bronze notebook, raw-to-Bronze reconciliation |
| 5 | Silver standardization | Silver notebook, canonical field mapping, transformation evidence |
| 6 | Data quality | Data-quality rules, validation notebook, DQ summary |
| 7 | Gold metrics | Gold tables, metric definitions, aggregation validation |
| 8 | Power BI draft | Gold exports, Power BI data model, initial dashboard pages |
| 9 | Dashboard refinement | Refined dashboard pages, final screenshots, analytical insights |
| 10 | Streaming simulation | Streaming notebook, JSON event schema, streaming metric evidence |
| 11 | Integration | Pipeline walkthrough, README updates, consolidated evidence |
| 12 | Final demonstration | Final report, demo script, contribution statement, submission checklist |

---

## 5. Important Rules

- Power BI must use approved, validated Gold outputs rather than connecting directly to raw CSV files or bypassing the Bronze/Silver/Gold pipeline.
- Do not submit copied internet repositories as original team work.
- Record external references in `docs/references.md`.
- AI-generated code, explanations, and documentation must be reviewed, tested, and explainable by the team.
- Maintain a GitHub commit and weekly log for each project week.
- Keep sample data small in GitHub. Recreate large datasets using scripts or store them in the approved data environment.
- Document the grain, schema, aggregation logic, and intended use of each Gold table.
- Validate KPI calculations and dashboard totals against the corresponding Gold data.
- Protect credentials and other sensitive information; do not commit secrets or private access tokens.
- Keep implementation status and evidence accurate. Mark work as completed only when the corresponding artifact or validation result exists.

---

## 6. Final Project Proof

By Week 12, this repository should demonstrate that the team has:

- Designed and documented the storm-event data sources and assumptions.
- Explored the dataset using Databricks.
- Ingested raw data into Bronze tables.
- Standardized and transformed data into Silver tables.
- Implemented data-quality checks and documented their results.
- Created curated Gold tables and analytical metric definitions.
- Built Power BI dashboards using Gold outputs.
- Implemented storm-event analysis, fatality and injury analysis, and damage/impact analysis where supported by the available data.
- Simulated streaming JSON events and documented the streaming workflow.
- Reconciled selected dashboard KPIs against Gold outputs.
- Maintained weekly GitHub logs, commits, screenshots, and supporting evidence.
- Documented individual contributions and responsible AI use.
- Prepared a final report and demonstration that explain the complete data pipeline, design decisions, validation process, and analytical outcomes.

---

## 7. Power BI Dashboard Scope

The Power BI dashboard is intended to provide an interactive view of storm-event activity and impacts.

| Dashboard page | Purpose | Example visuals |
|---|---|---|
| Overview | Present high-level storm activity and impact indicators | KPI cards, monthly trend, damage severity distribution, state and hazard filters |
| Event Analysis | Examine event frequency and hazard distribution | Events by event type, events by hazard group, time trend, impact-band chart, event details table |
| Fatality & Injury Analysis | Compare human impacts across storm events | Fatalities by event type, injuries by event type, impact-band comparison, time trend, details table |
| Additional analysis pages | Extend the analysis if required by project scope and available Gold tables | State comparisons, damage analysis, or other validated analytical views |

**Data integrity note:** KPI definitions, units, aggregation methods, relationships, and filter behaviour should be documented and verified against the actual Gold tables before the dashboard is presented as final.

---

## 8. Team and AI Transparency

**Team:** Team 09  
**Members:** ANUSHA, SHIVANI, NIRMALA

The team is responsible for understanding, reviewing, testing, and explaining the project's implementation. AI assistance may support learning, debugging, dashboard planning, and documentation, but it does not replace manual validation or team ownership of the submitted work.

Each team member's specific responsibilities and contributions should be recorded in the weekly logs and final submission materials.
