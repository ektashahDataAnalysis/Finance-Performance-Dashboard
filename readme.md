# Finance Performance Dashboard

## Overview

This project is a **Finance Performance Dashboard built in Microsoft Power BI**.

I created this report to give finance and sales teams a clear view of actual sales performance against targets. It brings key financial metrics, sales trends, and salesperson performance together in one interactive report.

The focus was on creating a dashboard that is easy to understand, practical for business users, and clean enough for management reporting.

---

## What I Built

### 1. Executive KPI Section

The top section provides a quick view of the main financial metrics:

* Actual Sales
* Sales Target
* Sales Variance
* Variance %
* Target Performance
* Periods Where Target Was Reached

The KPIs are placed at the top so users can understand the overall performance before moving into the detailed analysis.

### 2. Actual vs Target Analysis

I created a trend view comparing actual sales with the sales target over time.

This helps users identify:

* Periods where sales exceeded the target
* Periods where sales were below target
* Changes in performance over time
* Overall sales trends

### 3. Salesperson Performance

The report includes a detailed salesperson performance table with:

* Salesperson
* Actual Sales
* Target
* Variance
* Variance %
* Performance Trend

Conditional formatting, data bars, and sparklines are used to make the table easier to read and compare.

---

## Power BI Features Used

### Sparklines(In table Visual)

Sparklines are included in the salesperson table to show individual sales trends over time without requiring a separate chart for each salesperson.

### Data Bars
###Data bars(IN table Visual too)

Data bars make differences in sales values easier to compare directly within the table.

### Interactive Team Slicer

A team-level slicer allows users to focus the report on a specific team. The relevant KPIs, trends, and salesperson details update based on the selection.

### KPI Cards

KPI cards provide a quick summary of the main financial measures.

### Shapes and Layered Design

Shapes and layered elements are used to organize the report into clear sections and create visual hierarchy.

### Custom Styling

I applied consistent spacing, typography, number formatting, alignment, and theme settings instead of relying on Power BI's default formatting.

---

## How I Built the Report

### Step 1 — Prepare the Data

I brought the required finance and sales data into Power BI.

The data supports:

* Actual sales
* Sales targets
* Dates
* Salespeople
* Teams

I reviewed the available fields before building the report to make sure the data could support the required analysis.

### Step 2 — Build the Data Model

I created a structured Power BI model to support the report.

The model includes supporting tables such as:

* Calendar
* People / Salesperson
* Measures

The Calendar table supports time-based analysis, while salesperson and team information supports the detailed performance analysis.

### Step 3 — Create the DAX Measures

I created reusable DAX measures for the main calculations.

#### Actual Sales

Calculates total sales based on the current filter context.

#### Target Sales

Calculates the sales target for the selected period and filter context.

#### Sales Variance

```DAX
Sales Variance =
[Actual Sales] - [Target Sales]
```

This shows the difference between actual sales and the target.

#### Variance %

```DAX
Variance % =
DIVIDE(
    [Sales Variance],
    [Target Sales]
)
```

`DIVIDE()` helps handle situations where the target is zero or blank.

#### Target Status

Determines whether actual performance is meeting the expected target.

#### Months Target Reached

Shows how consistently the target was achieved during the reporting period.

---

## Report Layout

I organized the page around the way a business user would consume the information.

The report follows this flow:

**KPI Summary → Trend Analysis → Detailed Performance → Filtering**

This allows users to move from the overall result into the trend and then into salesperson-level details.

---

## Visual Design

After the calculations and visuals were working, I focused on the presentation of the report.

The design includes:

* Consistent spacing
* Alignment
* Font sizing
* Number formatting
* Section hierarchy
* Visual balance
* Background treatment
* Consistent theme

The goal was to keep the dashboard clean and easy to scan while still providing enough information for analysis.

---

## Testing & Interactivity

I tested the report using the available filters to make sure the visuals responded correctly.

For example, selecting a team updates the relevant:

* KPI values
* Trend analysis
* Salesperson details

This helped ensure that the dashboard was both visually polished and functional.

---

## Design Decisions

### Why not use more charts?

Adding more charts would make the page more crowded without necessarily adding more useful information.

Tables, data bars, and sparklines allow more information to be presented without overcrowding the report.

### Why put KPIs at the top?

The most important numbers should be visible first. Users can quickly understand overall performance before moving into the detailed analysis.

### Why use sparklines?

A separate chart for every salesperson would take up too much space. Sparklines provide a compact way to show individual performance trends.

### Why use data bars?

Data bars make numerical differences easier to recognize while scanning the table.

---

## Tools & Technologies

* Microsoft Power BI Desktop
* DAX
* Power BI Data Modeling
* Power BI Visualizations
* Conditional Formatting
* Sparklines
* Interactive Slicers
* Custom Report Styling

---

## Skills Demonstrated

This project demonstrates the complete Power BI reporting process:

**Data → Data Model → DAX → Visual Design → Interactivity → Dashboard**

Key skills demonstrated include:

* Power BI report development
* DAX measures
* Data modeling
* Financial KPI development
* Actual vs Target analysis
* Variance analysis
* Time-based analysis
* Interactive filtering
* Conditional formatting
* Sparklines
* Data bars
* Dashboard design
* Data storytelling
* Executive reporting

---

## Future Improvements

Potential enhancements for a future production version include:

* Regional analysis
* Product/category analysis
* Profitability and margin analysis
* MTD and YTD metrics
* Drill-through pages
* Custom tooltip pages
* Dynamic metric selection
* Additional executive KPIs
* Power BI Service deployment
* Scheduled data refresh

These are future enhancements and are not part of the current dashboard.

---

## Repository Structure

```text
PowerBI-Finance-Performance-Dashboard/
│
├── README.md
├── REQUIREMENTS.md
├── Finance data git.pbix
│
├── screenshots/
│   └── finance-dashboard.png
│
└── documentation/
    └── dax-measures.md
```

---

## Project Takeaway

I built this dashboard to demonstrate how Power BI can turn finance and sales data into a report that is easy to understand and explore.

The project combines **DAX, data modeling, interactive filtering, conditional formatting, sparklines, and dashboard design** to provide both a high-level view and detailed salesperson analysis.

The main focus was to create a practical business report rather than simply a collection of Power BI visuals.

---

## Portfolio Project

**Technology:** Microsoft Power BI
**Focus:** Finance & Sales Performance
**Primary Skills:** DAX, Data Modeling, Dashboard Design, Data Visualization, Business Reporting
