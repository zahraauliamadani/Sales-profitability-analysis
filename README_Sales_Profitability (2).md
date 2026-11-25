
# Sales Profitability & Loss Analysis

### Interactive Excel Dashboard | Data Analytics Portfolio Project

An interactive Microsoft Excel dashboard designed to analyze sales performance, profitability, cost of goods sold (COGS), and business performance across products, segments, countries, and discount categories.

**Tools:** Microsoft Excel, PivotTables, PivotCharts, Slicers, Power Pivot, DAX

**Dataset:** Microsoft Financial Sample (sample dataset)

**Data Source:** [Microsoft Financial Sample](https://learn.microsoft.com/en-us/power-bi/create-reports/sample-financial-download)

---

## Dashboard Preview

![Sales Profitability Dashboard](dashboard.png)

## View Interactive Dashboard

**[Open Interactive Excel Dashboard](https://1drv.ms/x/c/cbd0a3b974291310/IQDwkfjD8MPkTLRoKNwObov4Af6NKLLqYN1Y7p-LX-BU8oc?e=Uoc0Bc&nav=MTVfezU5NTQwQzgxLUQ0MkMtNDRGNy1BQzUzLTFEODNDQzNBOTdCMn0)**

Explore the dashboard online using Microsoft Excel for the Web. Use the available filters to examine sales, profits, product performance, business segments, and geographic profitability.

For full Power Pivot functionality, download the Excel workbook and open it in Microsoft Excel Desktop.

---

## Business Problem

High sales do not always result in high profitability. A business may generate substantial revenue while certain products, customer segments, or discount categories contribute relatively low margins or financial losses.

This project investigates profitability patterns to identify areas requiring further business analysis and potential improvement.

## Project Objectives

1. Analyze overall sales, profit, COGS, and profit margin.
2. Explore monthly sales and profit trends.
3. Compare profitability across products and business segments.
4. Identify segments generating financial losses.
5. Evaluate profitability across countries and discount categories.
6. Develop interactive visualizations and data-driven business recommendations.

## Dataset Overview

The project uses the Microsoft Financial Sample dataset containing 700 transaction records and 16 original columns.

Key fields include:

- Segment
- Country
- Product
- Discount Band
- Units Sold
- Sales
- COGS
- Profit
- Discounts
- Date

The dataset is provided for educational and analytical purposes and does not represent a company's audited financial statements.

## Data Analysis Workflow

### 1. Data Preparation

- Reviewed dataset structure and column formats.
- Checked financial and categorical variables.
- Prepared the data for analysis using Microsoft Excel.

### 2. Data Aggregation

Created PivotTables to summarize:

- Monthly Sales and Profit
- Profit by Product
- Profit by Business Segment
- Profit by Country
- Profit by Discount Band

### 3. Profitability Calculation

Calculated profit margin using the ratio of total profit to total sales.

**Profit Margin (%) = Total Profit / Total Sales × 100**

Created a DAX measure in Power Pivot:

```dax
Profit Margin % =
DIVIDE(
    SUM(financials[Profit]),
    SUM(financials[Sales])
)
```

This measure calculates profit margin using the current filter context rather than summing transaction-level percentages.

### 4. Dashboard Development

Developed an Excel dashboard containing:

- KPI Cards
- Line Charts
- Bar and Column Charts
- PivotCharts
- Interactive Slicers
- Profit Margin Analysis

## Key Performance Indicators

The following approximate figures describe the overall, unfiltered dataset.

| KPI | Value |
|---|---:|
| Total Sales | $118.73M |
| Total Profit | $16.89M |
| Total COGS | $101.83M |
| Overall Profit Margin | 14.23% |

## Dashboard Visualizations

| Visualization | Purpose |
|---|---|
| Monthly Sales vs Profit | Track sales and profitability trends over time |
| Profit by Product | Identify the most profitable products |
| Profit by Business Segment | Compare profitability across customer segments |
| Profit by Country | Evaluate geographic profit contributions |
| Profit by Discount Band | Compare total profit across discount categories |
| Profit Margin by Discount Band | Compare profit efficiency across discount levels |

## Key Findings

### 1. Overall Business Profitability

The dataset recorded approximately $118.73M in sales and $16.89M in profit, representing an overall profit margin of approximately 14.23%.

### 2. Government Is the Largest Profit Contributor

The Government segment generated approximately $11.39M in profit, the highest among the business segments.

### 3. Enterprise Segment Recorded a Loss

The Enterprise segment recorded a negative profit of approximately $0.61M.

This highlights an area that requires further investigation into product-level profitability, cost structure, and pricing.

### 4. Paseo Is the Most Profitable Product

Paseo generated approximately $4.80M in total profit, making it the highest profit-contributing product in the reviewed dashboard.

### 5. Profit Margins Differ Across Discount Categories

The No Discount category recorded a profit margin of approximately 22%, while the High Discount category recorded approximately 9%.

This indicates differences in profitability across discount categories. However, the observed association does not establish that discounts alone caused the margin differences.

## Business Recommendations

### 1. Investigate Loss-Making Segments

Conduct further analysis of the Enterprise segment by product, sales, COGS, and discount category to identify possible contributors to negative profitability.

### 2. Monitor Profit Margins by Discount Category

Evaluate profit margins alongside total sales and profit when reviewing discount practices. Consider product mix, customer segments, and transaction volumes before proposing pricing changes.

### 3. Monitor Product-Level Profitability

Use product-level profit and margin comparisons to identify strong performers and areas for further operational or commercial investigation.

### 4. Establish Regular Profitability Reviews

Use the dashboard for periodic monitoring of sales, profitability, product performance, and segment-level financial results.

These recommendations are proposed analytical actions, not interventions tested on a real business.

## Project Files

| File | Description |
|---|---|
| [Financial Sample.xlsx](Financial%20Sample.xlsx) | Excel workbook containing data, analysis, and dashboard |
| [dashboard.png](dashboard.png) | Screenshot of the completed dashboard |

## Limitations

- The project uses an educational sample dataset provided by Microsoft.
- The financial measures do not constitute a complete audited income statement.
- Findings are descriptive and do not demonstrate causation.
- Interactive features may have limitations in Excel for the Web. Microsoft Excel Desktop is recommended for full workbook functionality.
- Business recommendations have not been implemented or tested.

## Author

**Personal Data Analytics Portfolio Project**

Industrial Engineering Student | Data Analytics & Business Intelligence

**Focus:** Excel Data Analysis, Business Performance, Profitability Analysis, Data Visualization, and Reporting.
  
