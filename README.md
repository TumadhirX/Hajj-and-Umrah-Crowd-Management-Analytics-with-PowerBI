# Hajj and Umrah Crowd Management Analytics with PowerBI

An interactive **Power BI** project combining pilgrimage statistics and crowd-management data to explore Hajj and Umrah trends, congestion, and pilgrim behavior. Developed for **DS322: Business Intelligence** at Princess Nourah bint Abdulrahman University.

## Project overview

The dashboard supports analysis of pilgrim distribution, waiting times, crowd density, perceived safety, satisfaction, stress, and health conditions. Power Query transformations, a dimensional data model, DAX measures, slicers, and page navigation bring the analysis together.

## Dashboard pages

The report describes three dashboard pages. The supplied PBIX stores them as `Page 1`, `Page 2`, and `Page 3`.

| Analysis area | What it covers |
| --- | --- |
| Hajj and Umrah Pilgrims Overview | Pilgrim totals, male/female counts, arrival categories, yearly trends, and gender distribution |
| Crowd Analysis | Queue times, activities, crowd density, transport modes, incidents, satisfaction, and safety |
| Pilgrim Behavior and Health Analysis | Activity duration, stress levels, crowd conditions, and health distribution |

The dashboard uses KPI cards, gauge, bar and column charts, donut charts, scatter plots, and a decomposition tree. Available slicers vary by page; navigation buttons support moving between analyses.

## Repository contents

| File | Description |
| --- | --- |
| [Hajj_and_Umrah_Analytics.pbix](dashboard/Hajj_and_Umrah_Analytics.pbix) | Original Power BI dashboard, with a standardized filename |
| [Business_Intelligence_Report.pdf](docs/Business_Intelligence_Report.pdf) | Project report, methodology, dashboard screenshots, and references |
| [Dashboard_User_Guide.pdf](docs/Dashboard_User_Guide.pdf) | Original dashboard usage guide |
| [Report_Reading_Guide.pdf](docs/Report_Reading_Guide.pdf) | Original guide to the report structure |

## Open and explore

1. Install the current [Microsoft Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494) on a supported Windows computer.
2. Download this repository as a ZIP and extract it, or clone it:

   ```bash
   git clone https://github.com/TumadhirX/Hajj-and-Umrah-Crowd-Management-Analytics-with-PowerBI.git
   ```

3. Open `dashboard/Hajj_and_Umrah_Analytics.pbix` in Power BI Desktop.
4. Explore the pages, slicers, and chart selections. Use Ctrl+click for navigation buttons when required in Desktop edit mode.
5. Read `docs/Business_Intelligence_Report.pdf` alongside the dashboard for the data model and visual explanations. All supplied documentation is PDF and can be opened with a PDF viewer.

Power BI Desktop is required to interact with the report; GitHub does not render PBIX dashboards. No Python dependencies are needed. Publishing to Power BI Service is optional and requires your own account and any applicable license.

## Data sources and preparation

The report cites:

- [General Authority for Statistics, Saudi Arabia](https://www.stats.gov.sa): official Hajj and Umrah statistics.
- [Hajj and Umrah Crowd Management Dataset](https://www.kaggle.com/datasets/ziya07/hajj-and-umrah-crowd-managementdataset), by Z. Ziya on Kaggle.

Documented preparation includes removing non-data rows, renaming columns, assigning data types, filtering incomplete records, combining annual Hajj and quarterly Umrah tables, deriving year/quarter fields, and creating supporting Year and Quarter dimension tables.

Documented measures include average queue time, time spent at a location converted to hours, and crowd-observation counts.

Raw source datasets were not included in the uploaded files. The PBIX contains an embedded data-model component, but refreshing its queries may require the original source files, updated paths, or source access. If refresh fails, inspect **Transform data → Data source settings** and reconnect the appropriate sources. Do not assume refresh is necessary simply to view saved content.

## Scope and limitations

This project analyzes pre-collected data. The report identifies real-time feeds and advanced forecasting as future improvements; a live monitoring service or independently validated predictive model has not been verified here. Historical coverage and annual/quarterly aggregation limit detailed time-based analysis, and some behavioral indicators may be estimates.

The PBIX archive integrity and report layout were checked: **three pages and 44 visual containers**. Interactive rendering, DAX execution, model loading, and data refresh were not tested because Power BI Desktop is unavailable in the Linux workspace. Dashboard screenshots are included in the project report.

## Contributors

Jood Ahmed Bagazi, Mashael Mohammed Algazla, Reem Alotaibi, Tumadhir Alyahya, and Raghad Alqassimi.

The report credits Tumadhir Alyahya with dashboard design, user interaction, and implementation.

## Usage rights

No project license has been specified. Refer to the original sources for dataset usage terms.
