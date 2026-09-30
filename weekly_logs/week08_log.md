# Week 08 Log — Gold Hand-off and Power BI Dashboard Development

**Week:** 8  
**Date range:** 21st September 2026 - 27th September 2026  
**Team:** Team 09  
**Project:** StormWatch — Storm Event Analytics and Risk Dashboard

---

## 1. Sprint Goal

Build the Power BI dashboard using validated Gold-layer outputs and create an interactive analytical view of storm events, fatalities, injuries and event impacts.

Complete the Overview, Event Analysis, and Fatality & Injury Analysis pages with appropriate KPIs, charts, tables and slicers, while validating the dashboard results against the Gold data.

---

## 2. Work Completed

| Task | Owner | Status | Evidence |
|---|---|---|---|
| Identify approved Gold tables required for Power BI | Team | Done | Gold table mapping / Power BI model |
| Review Gold table schemas, fields and grain | Team | Done | Gold table schema review |
| Load required Gold tables into Power BI | Team | Done | Power BI data model |
| Establish relationships between dimension and fact tables | Team | Done | Power BI Model view screenshot |
| Build Overview dashboard page | Team | Done | Power BI Overview screenshot |
| Create KPI cards for total storm events, fatalities, injuries and damage | Team | Done | Overview dashboard |
| Add Year, State and Hazard Group slicers | Team | Done | Overview dashboard |
| Create Monthly Storm Risk Trend line chart | Team | Done | Overview dashboard |
| Create Damage Severity / Impact Band donut chart | Team | Done | Overview dashboard |
| Build Event Analysis dashboard page | Team | Done | Event Analysis screenshot |
| Create Events by Event Type visual | Team | Done | Event Analysis dashboard |
| Create Events by Hazard Group visual | Team | Done | Event Analysis dashboard |
| Create Storm Events Over Time visual | Team | Done | Event Analysis dashboard |
| Create Events by Impact Band visual | Team | Done | Event Analysis dashboard |
| Create Event Type Details table | Team | Done | Event Analysis dashboard |
| Build Fatality & Injury Analysis page | Team | Done | Fatality & Injury Analysis screenshot |
| Create Fatalities by Event Type visual | Team | Done | Fatality & Injury Analysis dashboard |
| Create Injuries by Event Type visual | Team | Done | Fatality & Injury Analysis dashboard |
| Create Fatalities & Injuries Over Time visual | Team | Done | Fatality & Injury Analysis dashboard |
| Create Fatalities & Injuries by Impact Band visual | Team | Done | Fatality & Injury Analysis dashboard |
| Create Fatality & Injury Details table | Team | Done | Fatality & Injury Analysis dashboard |
| Format dashboard visuals, cards, slicers and tables consistently | Team | Done | Power BI dashboard screenshots |
| Validate selected dashboard measures against Gold data | Team | Done | Gold reconciliation checks |

---

## 3. Key Decisions

- Use only validated Gold-layer outputs as the source for Power BI dashboard development.
- Keep the Power BI model based on the approved fact and dimension tables and their defined relationships.
- Use Year, State Name and Hazard Group as common dashboard slicers where applicable.
- Use distinct count of event IDs for event-count KPIs and event distribution visuals.
- Use aggregated fatality and injury measures for the corresponding analysis visuals.
- Use the Overview page for high-level KPIs and summary information.
- Use the Event Analysis page to analyze event frequency, hazard distribution, impact bands and event details.
- Use the Fatality & Injury Analysis page to analyze fatalities and injuries by event type, impact band and time.
- Maintain a consistent visual design across all dashboard pages, including card styling, slicers, chart formatting, spacing and alignment.
- Keep the dashboard focused on evidence from the available Gold data and avoid adding unsupported metrics or conclusions.

---

## 4. Blockers / Risks

| Blocker | Impact | Help Needed |
|---|---|---|
| No major blocking issue remained after Power BI model and visual validation | No significant impact on Week 08 completion | None |
| Some Power BI visuals required formatting and alignment adjustments | Minor additional dashboard design effort | Team review |
| Different measures use different aggregation methods such as distinct count and sum | Incorrect aggregation could affect dashboard values | Manual measure validation |

---

## 5. Evidence Added to GitHub

- Power BI dashboard file updated with the completed dashboard pages.
- Overview dashboard screenshot/evidence added.
- Event Analysis dashboard screenshot/evidence added.
- Fatality & Injury Analysis dashboard screenshot/evidence added.
- Gold table and field mapping documented for Power BI usage.
- Power BI model/relationship evidence captured.
- KPI and visual validation evidence captured.
- Dashboard formatting and slicer implementation evidence added.
- Relevant Power BI development notebooks/documentation updated.

---

## 6. AI Transparency Note

| Question | Response |
|---|---|
| Where AI helped | AI was used to assist with Power BI dashboard planning, Gold-table-to-visual mapping, selection of suitable fields for KPI cards and charts, dashboard layout suggestions, formatting guidance, troubleshooting and documentation wording. |
| What we changed after AI suggestion | The team reviewed the AI suggestions and adapted the dashboard layout, visual selection, field mappings, slicers, titles, formatting and table designs according to the actual StormWatch Gold data and project requirements. |
| What we verified manually | Gold table availability, field names, relationships, aggregation methods, KPI values, slicer behaviour, chart outputs, table contents, dashboard alignment and selected values were manually checked in Power BI against the available data. |
| What we can explain without AI | The team can explain the Gold-to-Power BI data flow, selected Gold tables, fact and dimension relationships, KPI calculations, slicers, dashboard visuals, event analysis, fatality and injury analysis, and the validation process used for the dashboard. |

---

## 7. Next Week Preparation

- Complete remaining StormWatch dashboard pages and analytical requirements, if applicable.
- Perform final validation of KPIs, filters, charts and tables against Gold-layer data.
- Review dashboard consistency, alignment, readability and user interaction.
- Document evidence-backed insights from the completed dashboard.
- Capture final screenshots and supporting evidence for GitHub.
- Update the project README and dashboard documentation with the final Power BI implementation.
