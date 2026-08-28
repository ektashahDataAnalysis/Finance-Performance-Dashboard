# Finance-Performance-Dashboard
Modern Power BI Finance Performance Dashboard featuring DAX, KPI analysis, Actual vs Target reporting, interactive slicers, sparklines, data bars, and executive-focused data storytelling.
# Business & Reporting Requirements

## 1. Project Overview

### Project Name

**Finance Performance Dashboard**

### Business Area

Finance / Sales Performance

### Primary Users

* Finance Managers
* Sales Managers
* Business Leaders
* Executives
* Management

### Purpose

The purpose of this project is to provide a centralized Power BI dashboard for monitoring financial and sales performance against established targets.

The dashboard should allow business users to quickly understand overall performance, identify variances, and investigate salesperson-level results.

---

# 2. Business Problem

The business needs a simple way to answer:

* How much sales have we achieved?
* What was the expected target?
* Are we above or below target?
* What is the variance?
* How is performance changing over time?
* Which salespeople are performing well?
* Which teams require attention?
* How consistently are targets being achieved?

Previously, answering these questions may require reviewing multiple tables or manually comparing actuals and targets.

The Power BI solution brings these metrics together into one interactive report.

---

# 3. Business Requirements

## BR-01 — Executive Performance Overview

The report must provide an executive-level summary of financial performance.

Users should be able to see:

* Actual Sales
* Sales Target
* Sales Variance
* Variance %
* Target Achievement / Status
* Number of periods meeting target

---

## BR-02 — Actual vs Target Analysis

Users must be able to compare actual sales against sales targets over time.

The analysis should make it easy to identify:

* Periods above target
* Periods below target
* Performance trends
* Changes in performance over time

---

## BR-03 — Variance Analysis

The dashboard must calculate the difference between actual sales and target sales.

### Variance

**Actual Sales − Target Sales**

Users should be able to determine whether performance is favorable or unfavorable.

---

## BR-04 — Variance Percentage

The report should provide a percentage-based view of performance.

### Variance %

**(Actual Sales − Target Sales) ÷ Target Sales**

This allows users to compare performance regardless of the size of the underlying sales value.

---

## BR-05 — Salesperson Analysis

Users must be able to evaluate performance at the salesperson level.

The report should provide:

* Salesperson
* Actual Sales
* Target
* Variance
* Variance %
* Performance trend

---

## BR-06 — Team Filtering

Users must be able to filter the report by team.

Filtering the team should update the relevant report visuals and KPIs.

---



# . User Experience Requirements

## UX-01 — Executive-Friendly Design

The report should communicate the most important information immediately.

Important KPIs should appear prominently at the top of the report.

---

## UX-02 — Minimal Visual Clutter

The dashboard should avoid unnecessary visuals.

Each visual should have a clear analytical purpose.

---

## UX-03 — Consistent Design

The report should use:

* Consistent typography
* Consistent spacing
* Consistent visual hierarchy
* Consistent formatting
* Consistent theme

---

## UX-04 — Interactive Filtering

Users should be able to filter the report without navigating away from the primary dashboard.

---

## UX-05 — Easy Performance Comparison

The design should allow users to recognize strong and weak performance quickly.

Conditional formatting, data bars, and embedded trends should be used where appropriate.

---

# 5. Technical Requirements

## TR-01 — Data Model

The solution should use a structured Power BI data model rather than relying on manually calculated values.

The model should support:

* Date analysis
* Salesperson analysis
* Team analysis
* Actual vs Target calculations

---

## TR-02 — DAX Measures

Business calculations should be implemented using DAX measures.

Core measures include:

* Total Actual Sales
* Total Target Sales
* Sales Variance
* Sales Variance %
* Target Status
* Months Target Reached

---

## TR-03 — Dynamic Filtering

All relevant measures and visuals should respond appropriately to report filters.

---

## TR-04 — Conditional Formatting

The report should visually distinguish performance where appropriate.

Examples include:

* Positive/negative variance
* High/low sales performance
* Actual vs target comparison

---

# 6. Visualization Requirements

The report should include a combination of:

### KPI Cards

For high-level financial metrics.

### Trend Visual

For Actual vs Target over time.

### Performance Table

For salesperson-level analysis.

### Sparklines

For compact trend analysis inside the detailed table.

### Data Bars

For quick comparison of sales values.

### Interactive Slicer

For team-level filtering.

### Shapes / Containers

For visual grouping and section hierarchy.

---

# 7. Non-Functional Requirements

### Performance

The dashboard should remain responsive when users interact with filters and visuals.

### Readability

Numbers should use appropriate financial formatting.

### Maintainability

Measures should be clearly named and organized.

### Scalability

The model should be structured so additional dimensions and KPIs can be added later.

### Professional Presentation

The report should be suitable for presentation to management and inclusion in a professional Power BI portfolio.

---



---

# 9. Success Criteria

The project will be considered successful when a business user can open the dashboard and quickly answer:

> **How are we performing against target, what is driving the variance, and which salespeople or teams require attention?**

The dashboard should provide those answers with minimal interaction while maintaining a clean and professional user experience.


