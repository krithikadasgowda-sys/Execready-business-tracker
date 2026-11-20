# ExecReady – Executive Request Management and Business Reporting

An Excel-based executive reporting solution designed to track ad hoc business requests, monitor workload distribution, identify overdue deliverables, and evaluate turnaround performance through an interactive management dashboard.

![ExecReady Dashboard](images/dashboard.png)

## Project Overview

Executive teams frequently handle ad hoc requests, including presentations, business reports, data pulls, analytical assignments, and dashboard updates. Managing these requests effectively requires visibility into ownership, priorities, deadlines, and delivery performance.

**ExecReady** addresses this challenge through a centralized Excel-based request management and reporting system. It transforms raw request data into actionable management insights, helping decision-makers identify bottlenecks, monitor team workload, and improve delivery accountability.

## Project Highlights

The following results are based on simulated request data, with a reporting date of 19 November 2026.

| Performance Metric | Result |
|---|---:|
| Total Requests Tracked | 60 |
| Departments Covered | 5 |
| Assigned Request Owners | 4 |
| Confirmed Request Types | 5 |
| Completed Requests | 47 (78%) |
| Open Requests | 13 |
| On-Time Delivery Rate | 54% (25 of 46 valid completions) |
| Late Completions | 21 of 46 valid completions |
| Average Turnaround Time | 4.5 days |
| Records Flagged by Data Quality Checks | 4 |

**Key observation:** Although 78% of requests have been completed, the on-time delivery rate is only 54%. This highlights the importance of measuring delivery timeliness separately from overall completion.

## Key Business Findings and Recommendations

**1. Completion Rate vs. Delivery Performance**

A 78% completion rate initially suggests strong progress. However, the on-time delivery rate of 54% indicates potential issues with deadline management.

*Recommendation:* Track completion and on-time delivery as separate performance indicators.

**2. Overdue Requests Require Immediate Attention**

All 13 open requests are overdue as of the reporting date. Two overdue requests, REQ-023 and REQ-047, carry High priority.

*Recommendation:* Introduce a daily 10-minute request review to prioritize overdue deliverables and resolve pending dependencies.

**3. Uneven Workload Distribution**

One request owner is responsible for 32% of the total request volume, while two requests remain unassigned.

*Recommendation:* Review workload distribution, reallocate requests where necessary, and establish clear ownership for every request.

**4. Deadline Management and Turnaround Targets**

The findings suggest that deadline planning and request prioritization deserve attention alongside turnaround efficiency.

*Recommendation:* Establish realistic turnaround targets based on request type and priority.

**5. Improve Request Intake Controls**

Missing ownership details, an unconfirmed request type, and invalid dates can affect reporting accuracy and accountability.

*Recommendation:* Make request owner, due date, request type, and priority mandatory fields during request submission.

## Workbook Structure

The workbook is organized into five functional sections.

| Worksheet | Purpose |
|---|---|
| Dashboard | Executive overview featuring six KPI cards, a management attention section, and six visualizations. Designed to print on one landscape page. |
| Pivot Tables | Formula-driven summary tables covering status, priority, request type, owner, department, and weekly trends, with reconciliation checks. |
| Requests | Centralized request register with dropdown validation, conditional formatting, and calculated columns. |
| Insights | Six business findings supported by data, explanations, and recommended management actions. |
| Read Me | Project documentation, metric definitions, assumptions, and data quality records. |

## Data Quality and Validation

Data quality checks were incorporated to improve consistency and ensure reliable reporting.

| Issue Identified | Action Taken |
|---|---|
| Duplicate request ID (REQ-008) | The second occurrence was renamed REQ-015 to restore the request sequence. |
| Two missing request owners | Replaced with UNASSIGNED and flagged for review. |
| One missing request type | Replaced with To Confirm and flagged. |
| Invalid completion date (REQ-045) | Retained and flagged because the completion date precedes the request's raised date. Excluded from turnaround and on-time calculations. |

**Impact of data validation:** Including the invalid REQ-045 record would have reduced the reported average turnaround time from 4.5 days to 3.6 days. Excluding it provides a more reliable performance measure.

## Technical Skills and Tools Demonstrated

**Microsoft Excel**
- COUNTIFS and AVERAGEIFS
- INDEX/MATCH
- Formula-driven PivotTable-style summaries
- Data validation and dropdown lists
- Conditional formatting
- KPI calculations and performance tracking
- Interactive charts and dashboard development
- Data reconciliation and quality checks

**Business and Analytical Skills**
- Executive reporting and business analysis
- Workload and priority analysis
- Deadline and turnaround monitoring
- Data quality assessment
- Management insights and recommendations
- Presentation development and documentation

**Additional Tool:** Microsoft PowerPoint

## Repository Structure

```text
ExecReady/
│
├── ExecReady_Dashboard.xlsx
├── README.md
├── .gitignore
│
├── docs/
│   ├── ExecReady_Presentation.pptx
│   ├── ExecReady_Dashboard_Snapshot.pdf
│   └── data_dictionary.md
│
├── data/
│   ├── ExecReady_Sample_Requests_original.csv
│   └── ExecReady_Requests_cleaned.csv
│
└── images/
    └── dashboard.png
```

## Assumptions and Limitations

- All request records and performance figures are simulated and do not represent actual organizational data.
- The reporting date is maintained as a fixed input to ensure consistent and reproducible results.
- Summary tables are formula-driven rather than native Excel PivotTable objects. They update automatically when the underlying data changes.
- The analysis reflects the assumptions and validation rules documented in the workbook.

## Project Deliverables

The repository includes:

- **Excel Workbook:** Centralized request tracker, management dashboard, reporting summaries, and business insights.
- **PowerPoint Presentation:** Eight-slide executive presentation summarizing project findings and recommendations.
- **PDF Dashboard Snapshot:** One-page export of the executive dashboard.
- **Data Dictionary:** Definitions of the dataset fields.
- **Sample Dataset:** Original and cleaned request data for transparency and reproducibility.

## Author

**Krithika Gowda**
