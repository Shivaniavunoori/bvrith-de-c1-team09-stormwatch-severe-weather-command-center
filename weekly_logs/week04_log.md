# Week 04 Log — StormWatch Bronze Layer Implementation

**Week:** 4  
**Date range:** 31 July 2026 – 06 August 2026  
**Team:** Team 9  
**Project:** StormWatch: Severe Weather Command Center  

**Team Members:**
- A. Shivani
- Nirmala Devi Patel
- Anusha

---

## 1. Sprint Goal

The goal of Week 4 was to implement the initial Bronze layer for the StormWatch project using Databricks. We focused on creating raw Bronze tables from the assigned source files while preserving the original data without applying business transformations or cleaning.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|------|-------|--------|----------|
| Reviewed Week-3 data exploration results | Team 9 | Done | `weekly_logs/week03_log.md` |
| Read approved StormWatch source files from Databricks Volume | Team 9 | Done | `notebooks/02_bronze_ingestion.ipynb` |
| Created Bronze tables for the assigned sources | Team 9 | Done | Databricks Bronze Tables |
| Verified source-to-Bronze row counts | Team 9 | Done | Notebook output |
| Executed DESCRIBE DETAIL and DESCRIBE HISTORY | Team 9 | Done | Notebook output |
| Validated successful Bronze data loading | Team 9 | Done | Databricks results |
| Captured Week-4 evidence screenshots | Team 9 | Done | `screenshots/week04_bronze_counts.png` |
| Updated GitHub repository | Team 9 | Done | GitHub Commit |

---

## 3. Key Decisions

- Preserved all raw source data without modification.
- Used Databricks Delta tables for Bronze storage.
- Maintained one Bronze table for each approved source file.
- Verified row-count consistency between source files and Bronze tables.
- Deferred data cleaning, standardization, and business transformations to later weeks.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|----------|--------|-------------|
| Large source files increased execution time | Notebook execution was slower | Optimize cluster resources if required |
| Row-count validation required careful verification | Needed manual comparison of source and Bronze counts | Team review before final submission |

---

## 5. Evidence Added to GitHub

- `notebooks/02_bronze_ingestion.ipynb`
- `screenshots/week-4_source-to bronze ingestion.png`
- `screenshots/week-4_sql-outputs.png`
- `weekly_logs/week04_log.md`

---

## 6. AI Transparency Note

| Question | Response |
|----------|----------|
| Where AI helped | AI assisted in creating the Week-4 Bronze notebook structure, documentation, and SQL examples. |
| What we changed after AI suggestion | We updated file paths, table names, and project-specific details according to the assigned StormWatch project. |
| What we verified manually | We manually verified notebook execution, Bronze table creation, row counts, and Databricks outputs. |
| What we can explain without AI | We can explain the Bronze layer architecture, Delta tables, row-count validation, source-to-Bronze ingestion process, and Databricks implementation steps. |

---

## 7. Next Week Preparation

- Begin implementing Candidate/Silver layer transformations.
- Define data-quality rules and validation checks for Week 5.
- Review data types and standardization requirements.
- Prepare cleaned datasets for downstream processing.
