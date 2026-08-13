# Power-BI-Food-Junction

# Food Junction --- Power BI Business Analysis Dashboard

## 📊 Project Overview

This project presents an interactive **Power BI business analysis
dashboard** for *Food Junction*, a fictional Pakistani restaurant chain.

The purpose of the project is to demonstrate how business data can be
transformed into meaningful insights for management --- from high-level
revenue and growth analysis to branch-level performance and operational
opportunities.

Rather than focusing only on creating attractive visuals, the dashboard
was built around practical business questions:

-   Is the business growing?
-   Which menu categories generate the most revenue and profit?
-   Which branches are performing strongly or weakly?
-   Are differences in branch revenue driven by order volume or customer
    spending?
-   Which weekdays are the weakest for individual branches?
-   Where should management investigate or consider targeted actions?

------------------------------------------------------------------------

## 🛠️ Tools & Technologies

-   **Power BI**
-   **DAX**
-   **Power Query**
-   **Excel / CSV data**
-   Data modeling and relationships
-   Interactive slicers and dashboard visuals

------------------------------------------------------------------------

## 📁 Dataset

The project uses a fictional restaurant dataset covering **January 2024
through December 2025**.

The dataset contains information relating to:

-   Branches
-   Employees
-   Customers
-   Menu items
-   Orders
-   Order details
-   Customer reviews

The restaurant offers several menu categories:

-   Pakistani
-   Pizza
-   BBQ
-   Chinese
-   Burgers
-   Coffee & Beverages
-   Desserts

The data was designed to resemble a realistic business dataset,
including enough variation to support exploratory analysis and business
decision-making.

------------------------------------------------------------------------

# 📌 Dashboard Structure

The dashboard currently contains two main pages.

## Page 1 --- Executive Overview

The Executive Overview provides management with a high-level view of
business performance.

### KPIs

-   **Total Revenue:** Rs 99.12M
-   **Total Orders:** 20K
-   **Unique Customers:** 5K
-   **Average Order Value:** Rs 4.96K
-   **YoY Revenue Growth:** +50.31%

### Main Visuals

#### Revenue by Month

A comparison of monthly revenue between 2024 and 2025.

This allows management to identify periods of stronger or weaker
performance and understand how revenue growth developed throughout the
year.

#### Revenue, Profits & COGS by Category

Revenue, realized sales profit, and cost of goods sold are compared
across menu categories.

This provides a more complete picture than revenue alone and helps
distinguish between categories that generate sales and categories that
contribute strongly to profit.

#### Revenue by Branch

Branch-level revenue is compared to identify the strongest and weakest
contributors.

#### Revenue by Weekday

Revenue is compared across the days of the week to identify recurring
demand patterns.

#### Interactive Filters

The dashboard includes:

-   **Year slicer**
-   **Branch slicer**

These allow management to investigate individual branches and compare
performance across years.

------------------------------------------------------------------------

# 📌 Page 2 --- Branch Performance Matrix

The second page focuses on branch-level operational performance without
unnecessarily duplicating the visuals from the Executive Overview.

The matrix compares:

  Metric                Business Meaning
  --------------------- ---------------------------------------
  Total Orders          Order volume / customer activity
  Average Order Value   Average customer spending per order
  Total Revenue         Overall branch contribution
  Weakest Revenue Day   Lowest-revenue weekday for the branch

Conditional formatting highlights the highest and lowest values in the
numerical columns, allowing important differences to be identified
quickly.

------------------------------------------------------------------------

# 🔎 Key Business Findings

### 1. Strong overall revenue growth

Food Junction generated approximately **50.31% more revenue in 2025 than
in 2024**.

The monthly comparison shows that 2025 started relatively slowly but
subsequently exceeded 2024 during much of the middle portion of the
year.

------------------------------------------------------------------------

### 2. Pakistani cuisine is the largest revenue category

The Pakistani menu category generates the highest revenue, followed by
Pizza.

However, the analysis also considers **sales profit and COGS**, rather
than assuming that the category with the highest revenue is
automatically the most profitable.

------------------------------------------------------------------------

### 3. Branch performance differs

**Clifton** is the strongest branch by both total orders and total
revenue.

**F-7** has the lowest total orders and lowest total revenue among the
branches.

------------------------------------------------------------------------

### 4. F-7's lower revenue is primarily an order-volume issue

Comparing F-7 with stronger branches showed that its Average Order Value
is broadly comparable with other branches.

For example:

-   **F-7 Revenue:** Rs 11.35M
-   **F-7 Orders:** 2,311
-   **F-7 AOV:** Rs 4,912

Compared with Clifton:

-   **Clifton Revenue:** Rs 13.60M
-   **Clifton Orders:** 2,736
-   **Clifton AOV:** Rs 4,972

This suggests that increasing **order volume**, rather than simply
increasing spending per order, may be the more relevant area for
investigation at F-7.

------------------------------------------------------------------------

### 5. Weak weekdays differ by branch

The weakest revenue day is not the same across all branches.

Examples from the analysis include:

-   DHA → Friday
-   Satellite Town → Thursday
-   Clifton → Wednesday
-   F-7 → Thursday
-   Civil Lines → Saturday

This suggests that promotional strategies could potentially be
**targeted according to individual branch demand patterns**, rather than
applying the same promotion across every branch.

These observations should be treated as opportunities for further
investigation and testing rather than guaranteed causes or outcomes.

------------------------------------------------------------------------

### 6. High AOV does not necessarily mean high revenue

Satellite Town provides an interesting example.

It has a relatively high Average Order Value but relatively low order
volume.

This demonstrates why management should consider both:

> **Order Volume × Average Order Value**

rather than relying on revenue or AOV alone.

------------------------------------------------------------------------

# 🧠 Analytical Approach

The project follows a business-question-driven approach:

**Business Question → Data Investigation → DAX / Calculation →
Visualization → Business Insight**

Examples of DAX concepts used in the project include:

-   `CALCULATE`
-   `SUMX`
-   `RELATED`
-   `FILTER`
-   `ALL`
-   `DIVIDE`
-   `AVERAGE`
-   `DISTINCTCOUNT`
-   Time-intelligence calculations
-   Variables (`VAR`)
-   Iterator functions such as `MINX`

The project also demonstrates the importance of **data modeling and
filter context**.

During development, a category-based order calculation initially
returned the total number of orders for every category. Investigation
showed that the issue was related to **filter propagation through the
data model**, rather than incorrect DAX syntax.

This was an important part of the analysis because a correct DAX
expression still depends on an appropriately structured Power BI model.

------------------------------------------------------------------------

# 💡 Business Recommendations

Based on the analysis, management could consider:

1.  **Investigating F-7's low order volume**, particularly because its
    AOV is broadly comparable with other branches.
2.  **Testing targeted promotions on branch-specific weak weekdays**
    rather than using one company-wide promotion strategy.
3.  Investigating why some branches have high AOV but comparatively low
    order volume.
4.  Monitoring category-level profit alongside revenue when making menu
    or promotional decisions.
5.  Using the dashboard interactively to investigate branch and
    year-specific performance before making operational decisions.

These recommendations are intended as **data-informed hypotheses for
further investigation and testing**, rather than definitive causal
conclusions.

------------------------------------------------------------------------

# 📷 Dashboard Preview

### Executive Overview
![Dashboard Page 1](Food%20junction%20PBI%201.PNG)

### Branch Performance
![Dashboard Page 2](Food%20junction%20PBI%202.PNG)


------------------------------------------------------------------------

# 🎯 Project Objective

This project was created as a portfolio demonstration of practical
**Data Analyst / BI Analyst** skills.

The main objective was not simply to build a Power BI dashboard, but to
demonstrate the complete analytical process:

> **Understand the business question → analyze the data → build the
> appropriate calculations → visualize the result → communicate an
> actionable insight.**

