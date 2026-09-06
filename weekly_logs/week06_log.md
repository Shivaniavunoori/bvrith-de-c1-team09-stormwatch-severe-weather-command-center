# Week 06 Log — Data Quality Checks

**Week:** 6  
**Date range:** September 1–7, 2026  
**Team:** Team 09  
**Project:** StormWatch – Storm Event Monitoring and Analytics

---

## 1. Sprint Goal

The goal for Week 6 was to implement and execute data quality checks on the StormWatch Silver Candidate data.

The checks cover required event fields, chronology and timestamp validation, reference integrity, geographic validity, injury/fatality reconciliation, damage and magnitude validation, and duplicate detection.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|---|---|---|---|
| Implemented storm event required-field checks | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented chronology and UTC timestamp checks | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented reference integrity checks | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented geographic validation checks | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented injury and fatality validation and reconciliation | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented property and crop damage validation | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented magnitude validation against event-type mapping | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Implemented duplicate and join-safety checks | Team 09 | Done | `notebooks/04_data_quality_checks.ipynb` |
| Routed failed records to StormWatch quarantine tables | Team 09 | Done | DQ notebook outputs |
| Validated trusted and quarantine record reconciliation | Team 09 | Done | DQ notebook outputs |
| Captured failed record examples | Team 09 | Done | DQ notebook outputs |

---

## 3. Key Decisions

- Data quality rules were implemented according to the approved StormWatch Week 6 DQ rulebook.
- DQ checks were evaluated before records were routed to Trusted or Quarantine.
- Failed records were retained in quarantine with DQ status and failure information instead of being silently removed.
- Reference checks use trusted upstream reference data for event types and geography.
- Physical quarantine reconciliation is based on distinct source records, while a single record may have multiple rule-level failures.
- Gold metrics are generated only from Trusted Silver data.
- Manual correction of quarantined records is not performed as part of the Week 6 batch process.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|---|---|---|
| No major blocker currently identified | No major impact on the Week 6 DQ implementation | None |

---

## 5. Evidence Added to GitHub

- `notebooks/04_data_quality_checks.ipynb`
- `src/data_quality_rules.py`
- `docs/data_quality_summary.md`
- `weekly_logs/week06_log.md`
- `screenshots/week06_dq_results.png`
- `screenshots/week06_failed_records_sample.png`

---

## 6. AI Transparency Note

| Question | Response |
|---|---|
| Where AI helped | AI was used to help structure the StormWatch data quality notebook and explain suitable DQ checks for the StormWatch Silver Candidate tables. |
| What we changed after AI suggestion | The suggested checks and transformations were adapted to the approved StormWatch DQ rules, actual table names, and available column names in Databricks. |
| What we verified manually | The StormWatch catalog and schema, Silver Candidate tables, column names, reference tables, joins, DQ rule IDs, and routing logic were verified manually in Databricks. |
| What we can explain without AI | We can explain why each DQ rule is required, what type of StormWatch data failure it detects, how failed records are quarantined, and how poor-quality records can affect storm-event analytics and reporting. |

---

## 7. Next Week Preparation

- Review the Week 6 DQ results and quarantined records.
- Review failed DQ rules and identify the earliest upstream cause for any required correction.
- Prepare the Trusted Silver data for the next stage of StormWatch analytics.
- Preserve the DQ and quarantine history for future replay and correction.


