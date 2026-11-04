# Bright-Coffee-Case-Study-


**From sales transactions to actionable business insights**  
**Author:** Nompumelelo Deanah Mkolo  
**Analysis period:** 1 JanuaryΓÇô30 June 2023

## Project Overview

This case study analyses Bright Coffee Shop's sales performance across three locations: **Astoria, HellΓÇÖs Kitchen and Lower Manhattan**. It brings together project planning, data preparation, sales analysis and dashboard development to support management decisions about revenue growth, product availability, staffing and promotions.

The project addresses four business questions:

- Which products and categories generate the most revenue?
- How does sales performance compare across stores?
- How do sales vary by month, day and trading period?
- Which improvements should management prioritise and test?

The supporting materials include Excel dashboards, a Power BI report, a CEO presentation, a Miro project layout and dashboard plan, and a Gantt chart.

## Process

The Gantt chart organises the work into seven overlapping activities across four weeks.

| Stage | Activity | Purpose |
| --- | --- | --- |
| 1 | Project initiation and planning | Define business objectives, scope, deliverables and the project schedule. |
| 2 | Data acquisition and understanding | Review sales fields, reporting dates, store locations and product classifications. |
| 3 | ETL development | Prepare data types, check missing values and duplicates, and standardise fields for analysis. |
| 4 | Databricks data storage | Structure the planned lakehouse into Bronze (raw), Silver (cleaned) and Gold (reporting) layers. |
| 5 | SQL analysis | Aggregate revenue, transactions and units sold by product, store and time period. |
| 6 | Dashboard development | Present KPIs and sales patterns through Excel and Power BI dashboards. |
| 7 | Testing and validation | Reconcile totals, review calculations and labels, and check dashboard consistency. |

**Workflow:** Sales data ΓåÆ data preparation ΓåÆ planned Databricks lakehouse ΓåÆ analysis ΓåÆ dashboards ΓåÆ management recommendations.

The presentation describes a SQL and Databricks workflow; executable SQL scripts and Databricks notebooks were not included in the supplied project files.

### KPI definitions

| Metric | Calculation |
| --- | --- |
| Revenue | Sum of unit price ├ù quantity at transaction level; sum of `revenue` in the supplied aggregated data. |
| Transactions | Sum of `number_of_sales` in the supplied aggregated data. |
| Units sold | Sum of `units_sold`. |
| Average transaction value | Total revenue ├╖ total transactions. |
| Store revenue share | Store revenue ├╖ total revenue ├ù 100. |

The worksheet named `Raw Data` contains aggregated records. Its row count should not be treated as the transaction count, and distinct-product or distinct-store counts should not be summed across groups.

## Summary

The supplied Excel data reconciles to the following six-month results:

| KPI | Result |
| --- | ---: |
| Total revenue | 698,812.33 |
| Total transactions | 149,116 |
| Total units sold | 214,470 |
| Average transaction value | 4.69 |
| Average units per transaction | 1.44 |
| Store locations | 3 |

The CEO presentation reports that HellΓÇÖs Kitchen contributes approximately **34.8%** of revenue, followed by Astoria at **34.1%** and Lower Manhattan at **31.1%**. Monthly transaction volume rises from approximately **17,300 in January to 35,400 in June**. Brewed Chai tea is the highest-revenue product type among those highlighted in the presentation.

Recommended actions are to maintain availability of strong sellers, test coffee-and-pastry bundles, compare successful selling practices across stores, and automate validated KPI reporting. These are proposed improvements; the materials do not establish a measured uplift from implementation.

**Reporting limitations:** The presentation uses dollar symbols while the executive Excel dashboard labels revenue in rand. Confirm the source currency before publishing financial figures. Exact peak 30-minute intervals still need validation. Cost, margin, labour, waste and customer-level data are needed to assess profitability and retention.

## Tools Used

| Tool | Role in the project |
| --- | --- |
| Microsoft Excel | Data review, KPI reconciliation, pivot summaries and interactive dashboards. |
| Microsoft Power BI | Sales visualisation and business intelligence reporting in the supplied `.pbix` file. |
| SQL | Querying and aggregation described in the project workflow; scripts are not supplied. |
| Databricks | Lakehouse storage and processing described in the project plan; notebooks are not supplied. |
| Miro | Project layout, analysis workflow and dashboard planning, provided as a PDF export. |
| Microsoft PowerPoint | CEO presentation of findings, recommendations and implementation priorities. |
| Gantt chart | Scheduling project activities and tracking their overlap across four weeks. |




