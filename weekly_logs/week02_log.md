# Week 02 Log — Meet the Data: Contracts, Grains and Checksums

**Week:** 2  
**Date Range:** 21 July 2026 – 27 July 2026  
**Team:** Team 9  
**Project:** StormWatch – Weather Event Analytics Platform

---

# 1. Sprint Goal

The objective for Week 02 was to understand the StormWatch dataset by identifying all raw and reference source files, documenting their schemas, defining primary and foreign keys, understanding the business grain of each dataset, documenting synthetic data assumptions, and preparing sample datasets before implementing the Bronze layer.

---

# 2. Work Completed

| Task | Owner | Status | Evidence |
|------|-------|--------|----------|
| Reviewed StormWatch Project Playbook | Team 9 | ✅ Completed | Project Playbook PDF |
| Explored all source datasets | Team 9 | ✅ Completed | Dataset Pack |
| Identified all raw and reference files | Team 9 | ✅ Completed | docs/data_dictionary.md |
| Documented source file catalog | Team 9 | ✅ Completed | docs/data_dictionary.md |
| Documented field names, data types and descriptions | Team 9 | ✅ Completed | docs/data_dictionary.md |
| Defined Primary Keys and Foreign Keys | Team 9 | ✅ Completed | docs/data_dictionary.md |
| Designed Canonical Silver table mapping | Team 9 | ✅ Completed | docs/data_dictionary.md |
| Documented Streaming Event Schema | Team 9 | ✅ Completed | docs/data_dictionary.md |
| Documented Synthetic Data Assumptions | Team 9 | ✅ Completed | docs/synthetic_data_assumptions.md |
| Prepared raw sample datasets | Team 9 | ✅ Completed | data_sample/raw/ |
| Verified dataset relationships and business grain | Team 9 | ✅ Completed | Project Documentation |
| Updated Week 02 documentation | Team 9 | ✅ Completed | GitHub Repository |

---

# 3. Key Decisions

- Used the official StormWatch dataset.
- Preserved the original business grain for all datasets.
- Documented raw, reference, and streaming datasets before ingestion.
- Defined Primary Keys and Foreign Keys.
- Created a canonical Silver table design.
- Used only synthetic weather data.
- Followed the official project folder structure.

---

# 4. Blockers / Risks

| Blocker | Impact | Resolution |
|----------|--------|------------|
| Understanding relationships between storm events, locations and fatalities | Medium | Studied project documentation |
| Identifying Primary and Foreign Keys | Low | Cross-verified relationships |
| Understanding streaming alert structure | Low | Reviewed project playbook |
| Mapping raw fields to Silver schema | Low | Designed canonical Silver mapping |

---

# 5. Validation Performed

- Verified source files.
- Verified field names and data types.
- Verified primary and foreign keys.
- Verified business grain.
- Reviewed streaming event schema.
- Ensured documentation follows the template.

---

# 6. Evidence Added to GitHub

```text
docs/
├── data_dictionary.md
└── synthetic_data_assumptions.md

weekly_logs/
└── week02_log.md
```

---

# 7. AI Transparency Note

| Question | Response |
|----------|----------|
| Where AI helped | Assisted in preparing documentation and formatting Markdown files. |
| What we changed after AI suggestion | Verified dataset fields and updated project-specific content manually. |
| What we verified manually | Dataset schemas, keys, relationships, and documentation. |
| What we can explain without AI | Dataset structure, workflow, documentation, and project design. |

---

# 8. Next Week Preparation

- Build Bronze layer.
- Load raw datasets.
- Perform schema validation.
- Implement Data Quality checks.
- Begin Silver transformations.
- Commit Bronze implementation.

---

# 9. Team Members

- A. Shivani
- Nirmala Devi
- Goli Anusha

**Team Number:** 9

---

# 10. Week 02 Summary

- Completed documentation of all datasets.
- Documented schemas, keys, and relationships.
- Created Data Dictionary.
- Documented Synthetic Data Assumptions.
- Prepared Week 02 GitHub documentation.

**Week 02 Status:** ✅ Completed Successfully



