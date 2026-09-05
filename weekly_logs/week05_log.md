# Week 05 Log — Silver Transformations

**Week:** 5
**Date range:** 7-13
**Team:** 9
**Project:** ShipTrack: Supply Chain Visibility Hub

---

## 1. Sprint Goal

Standardize and transform the Bronze-layer data into clean and structured Silver tables.
Create six Silver tables for carriers, exceptions, hubs, routes, scan events, and shipments with appropriate data types, standardized fields, and duplicate handling.

---

## 2. Work Completed

| Task                                         | Owner        | Status | Evidence                          |
| -------------------------------------------- | ------------ | ------ | --------------------------------- |
| Silver transformation for Scan Events        | Nirmala Devi | Done   | `03_silver_transformations.ipynb` |
| Silver transformation for Shipments          | Nirmala Devi | Done   | `03_silver_transformations.ipynb` |
| Silver transformation for Carriers           | Shivani A    | Done   | `03_silver_transformations.ipynb` |
| Silver transformation for Routes             | Shivani A    | Done   | `03_silver_transformations.ipynb` |
| Silver transformation for Hubs               | Anusha       | Done   | `03_silver_transformations.ipynb` |
| Silver transformation for Exceptions         | Anusha       | Done   | `03_silver_transformations.ipynb` |
| Silver table validation and row-count checks | Anusha       | Done   | Databricks screenshots            |

---

## 3. Key Decisions

* Created one Silver table corresponding to each Bronze table.
* Standardized columns and converted fields into appropriate data types.
* Standardized shipment status values for consistency.
* Removed duplicate records during Silver transformations where applicable.
* Stored the transformed datasets as managed Silver tables.

---

## 4. Blockers / Risks

| Blocker                                                                                             | Impact                                                                   | Help Needed                                                                      |
| --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------------------------- |
| Generic Silver template contained columns that were not present in the actual ShipTrack Bronze data | Required modification of the template to match the actual Bronze schemas | Verified Bronze schemas and modified transformations accordingly                 |
| Initial validation query referenced fields that were not available in the project data              | SQL validation query failed                                              | Replaced the query with validation queries based on the actual available columns |

---

## 5. Evidence Added to GitHub

* `03_silver_transformations.ipynb`
* Silver transformation screenshots
* Silver schema screenshots
* Silver row-count screenshots
* SQL validation results

---

## 6. AI Transparency Note

| Question                            | Response                                                                                                                                                      |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Where AI helped                     | AI helped adapt the generic Silver transformation template to the actual ShipTrack Bronze table schemas and suggested suitable validation queries.            |
| What we changed after AI suggestion | We modified the generic transformation code to use the actual columns available in the ShipTrack Bronze tables.                                               |
| What we verified manually           | Bronze table names, column names, schemas, Silver table creation, duplicate handling, row counts, and SQL query results were manually verified in Databricks. |
| What we can explain without AI      | We can explain the Bronze-to-Silver transformation process, schema standardization, duplicate handling, Silver table creation, and validation process.        |

---

## 7. Next Week Preparation

* Review and validate all Silver tables.
* Prepare the Silver data for Gold-layer transformations.
* Identify relationships between shipments, scan events, routes, hubs, carriers, and exceptions.
* Begin designing analytics-ready Gold tables and KPIs.



