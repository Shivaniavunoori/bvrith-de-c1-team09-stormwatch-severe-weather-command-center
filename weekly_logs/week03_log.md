# Week 03 Log — StormWatch Data Exploration

**Week:** 3  
**Date range:** 25 July 2026  
**Team:** Team 9  
**Project:** StormWatch: Severe Weather Command Center  

**Team Members:**  
- A. Shivani
- Nirmala Devi Patel
- Anusha

---

## 1. Sprint Goal

The goal of Week 3 was to explore and understand the assigned StormWatch source data in Databricks. We loaded the approved source files from the Databricks Volume, inspected their schemas and grains, profiled row counts and key distributions, and checked relationships, missing values, timestamp anomalies, and impossible values.

We also created one Week-3 Bronze demonstration table and one downstream lineage demonstration view while keeping the complete Bronze implementation reserved for Week 4.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|---|---|---|---|
| Inspected the assigned Databricks Volume | Team 9 | Done | `screenshots/week03_databricks_data_loaded.png` |
| Loaded the approved StormWatch source files | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Created DataFrames for the Week-3 sources | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Displayed source DataFrames and inspected schemas | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Created temporary SQL views | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Profiled physical rows and distinct business keys | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Checked missing and impossible values | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Performed parent-child and reference relationship checks | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Demonstrated join multiplication risk | Team 9 | Done | `notebooks/01_data_exploration.ipynb` |
| Created one Week-3 Bronze demonstration table | Team 9 | Done | Databricks table and notebook |
| Created one downstream lineage demonstration view | Team 9 | Done | `screenshots/week03_databricks_lineage_demo.png` |
| Updated the Week-3 evidence log | Team 9 | Done | `weekly_logs/week03_log.md` |

---

## 3. Key Decisions

- Used the assigned Databricks Volume path as the source location authority.
- Preserved the documented source grains instead of treating all source files as event-grain data.
- Used Spark SQL as the primary language for data exploration.
- Used physical row counts and distinct business-key counts separately because they answer different questions.
- Used anti-join checks to identify possible orphan records and unresolved references.
- Aggregated child sources independently before joining them to event-level data to avoid measure multiplication.
- Created exactly one Week-3 Bronze demonstration table.
- Created exactly one downstream lineage demonstration view.
- Did not implement the complete Bronze layer or other Week-4 functionality.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|---|---|---|
| Actual execution results must be recorded from Databricks | Counts and data-quality findings cannot be fabricated | Team review of executed notebook results |
| Exact project repository structure and evidence naming must be maintained | Incorrect paths could make evidence difficult to verify | Team confirmation before final commit |

---

## 5. Evidence Added to GitHub

- `notebooks/01_data_exploration.ipynb`
- `screenshots/week03_databricks_volume_config.png`
- `screenshots/week03_databricks_data_loaded.png`
- `screenshots/week03_databricks_lineage_demo.png`
- `weekly_logs/week03_log.md`

---

## 6. AI Transparency Note

| Question | Response |
|---|---|
| Where AI helped | AI helped convert the Week-3 learning notebook structure into a project-specific StormWatch exploration notebook and helped organize the Week-3 evidence log. |
| What we changed after AI suggestion | We verified and updated the project-specific Volume path and checked that the source files visible in Databricks matched the assigned project source pack. |
| What we verified manually | We manually verified the Databricks Volume listing, the source filenames, the project configuration, notebook execution, and the displayed exploration outputs. |
| What we can explain without AI | We can explain the source grains, physical versus distinct key counts, temporary SQL views, missing-value checks, anti-joins, parent-child relationships, join multiplication risk, and the Week-3 versus Week-4 boundary. |

---

## 7. Next Week Preparation

- Review the Week-3 profiling findings and confirm the source-to-business-grain relationships.
- Prepare the Week-4 Bronze implementation using the approved source files and repository structure.
- Define the official raw-preserving Bronze table design for each approved source.
- Prepare the Week-4 ingestion and reconciliation approach without modifying source values.
