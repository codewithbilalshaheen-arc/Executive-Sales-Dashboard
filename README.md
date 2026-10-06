# Executive Sales Dashboard (Power BI)

An interactive Power BI dashboard that gives sales leadership a single, live view of revenue, pipeline health, and sales rep performance, replacing scattered weekly spreadsheet reports that had to be compiled by hand.

## Business Problem

Sales directors receive separate spreadsheets from different reps and regions. Compiling them delays decisions and risks inconsistent numbers. This dashboard centralizes the data so leadership can see overall performance at a glance and drill down to a region or rep without requesting a new report.

## Key Features

- **Overview:** Total revenue (MTD), revenue vs. target, total pipeline value, deals closed this month, 12-month revenue trend with target line, and regional breakdown
- **Pipeline:** Deal funnel (Prospecting → Qualified → Negotiation → Closed Won/Lost), stage-to-stage conversion rates, and a deal-level table
- **Rep Leaderboard:** Revenue closed, quota attainment, and deals in progress per rep, with drill-through to individual deals
- **Filters:** Date range, region, product line, and sales rep
- **Row-level security:** Regional managers see only their own region
- **Scheduled refresh** through Power BI Service

## Tech Stack

Power BI Desktop · Power Query (M) · DAX · Star-schema data model · Power BI Service

## Data Model

`Fact_Deals` linked to `Dim_Reps`, `Dim_Regions`, `Dim_Products`, and `Dim_Dates`.

## Status

🚧 In development. Documentation, screenshots, KPI definitions, and validation notes will be added as each phase is completed.

## Out of Scope (v1)

Predictive forecasting, native mobile app, and commission calculations.
