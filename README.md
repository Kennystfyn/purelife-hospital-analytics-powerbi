# Pure Life Hospital Analytics Project

**Type:** Power BI Portfolio Case Study
**Focus:** Operational • Clinical • Financial Performance Analysis
**Tool:** Power BI (data modeling, DAX measures, date table, drill-through, slicers)

## Executive summary
Pure Life Hospital needed a clearer way to connect patient activity, clinical outcomes, and financial performance. This project turns the hospital dataset into an interactive Power BI reporting solution across three linked views: **Executive/Operations**, **Clinical**, and **Patient**.

The dashboard covers **5,000 patient visits** and **$294.03M in total revenue**. Insurance covers $201.84M (a 68.65% coverage ratio). Admission rate is 30.48%, average length of stay is 3.56 days, average severity score is 5.84, and mortality rate is 2.22%.

The standout finding: only **35% ($102M)** of billed revenue is Paid, while **33% ($97M) is Pending** and **32% ($95M) is Rejected** — meaning roughly **65% of billed revenue ("Revenue at Risk")** needs active claims and collections follow-up.

## Business problem
Despite high patient volume and substantial billed revenue, the hospital lacked a centralized way to monitor the intersection of clinical outcomes and financial performance — specifically: revenue cycle visibility, resource allocation across departments, clinical quality tracking, and consolidated patient history.

## What I did
- Structured the dataset (patient, visit, clinical, and financial fields) and built a dedicated date table for chronological analysis
- Built the data model and relationships, then created DAX measures for total visits, revenue, insurance coverage ratio, admission rate, ALOS, average severity score, and mortality rate
- Designed three interactive report pages with slicers for insurance provider, department, and patient ID
- Added a Revenue at Risk % KPI, upgraded the severity visual to compare outcome composition by severity score, and configured the Patient page for drill-through investigation

## Dashboard pages
1. **Executive/Operations** — headline KPIs, monthly revenue trend, department workload, payment-status breakdown, with Date/Insurance Provider/Department slicers
2. **Clinical** — severity distribution, visit type, primary diagnosis, and outcome status, including severity-vs-outcome comparison
3. **Patient** — record-level detail by Patient ID, usable as a drill-through destination with a Back button for navigation

## Key metrics
- **Total patient visits:** 5,000 · **Total revenue:** $294.03M · **Insurance covered:** $201.84M (68.65%)
- **Admission rate:** 30.48% · **Avg. length of stay:** 3.56 days · **Avg. severity score:** 5.84 · **Mortality rate:** 2.22%
- **Payment status:** Paid $102M (35%) · Pending $97M (33%) · Rejected $95M (32%) → **Revenue at Risk: 65%**

## Key findings
- **Department workload:** Dermatology (1,201) and General Practice (1,027) together account for ~44.6% of all visits; Oncology has the lowest volume (161)
- **Visit type:** Outpatient (~2.5K) is the largest visit category, ahead of Inpatient (~1.5K) and Emergency (~1.0K)
- **Clinical severity:** Severity score 9 has the highest frequency (846 visits); notable volume at scores 9–10 warrants closer monitoring
- **Diagnoses:** Digestive System Disorder is the leading diagnosis (873), followed by Infectious/Parasitic Diseases (692) and Cardiovascular Disease (554)
- **Outcomes:** ~84.5% of visits end in Discharged status; mortality rate is 2.22%
- **Revenue:** Monthly revenue ranges from ~$21.9M (February) to ~$27.0M (June); insurance-covered amounts range from ~$14.6M (April) to ~$18.8M (November)

## Recommendations
- Prioritize review of Pending and Rejected claims — track rejection reasons, resubmission time, and recovery rate by insurance provider
- Review staffing/capacity in Dermatology and General Practice given their patient load
- Examine outpatient registration, consultation, and discharge flow for avoidable waiting time
- Build a severity-vs-outcome view and monitor mortality by department/diagnosis to separate case complexity from potential quality concerns
- Introduce a focused view for severity scores 9–10
- Use the Patient drill-through page to consolidate repeat-visit history
- Add rejection rate, pending claim value, and collection rate KPIs for a fuller revenue-cycle picture

## Business impact
Faster visibility into department workload and demand, improved monitoring of clinical severity and outcomes, clearer identification of revenue at risk, a consolidated patient-level view, and a shared reporting layer across operations, clinical, and finance teams.

## Limitations & future improvements
Severity-outcome and claims findings currently show association, not causation — deeper patient-risk, treatment, and claims-aging data would be needed to confirm root causes. Targets/benchmarks for ALOS, admission rate, mortality, and rejection rate are still needed to judge performance against expectations rather than raw numbers alone.

## Files
- [Pure_Life_Hospital_Portfolio_Report_Final.docx](./Pure_Life_Hospital_Portfolio_Report_Final.docx) — full written case study
- [Purelife_Hospital_DataSet_Final.pbix](./Purelife_Hospital_DataSet_Final.pbix) — the Power BI file (all 3 report pages)
- [Pure_Life_Executive_Operations_Dashboard.png](./Pure_Life_Executive_Operations_Dashboard.png) — Executive/Operations view
- [Pure_Life_Clinical_Dashboard.png](./Pure_Life_Clinical_Dashboard.png) — Clinical view
- [Pure_Life_Patient_Dashboard.png](./Pure_Life_Patient_Dashboard.png) — Patient view
