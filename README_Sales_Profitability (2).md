# Sales Profitability & Loss Analysis

**Tools:** Microsoft Excel, PivotTables, PivotCharts, Slicers, Power Pivot / DAX  
**Dataset:** Microsoft Financial Sample (sample data; not a real company's financial statements)  
**Source:** https://learn.microsoft.com/en-us/power-bi/create-reports/sample-financial-download

![Sales Profitability Dashboard](images/dashboard.png)

> **Dashboard image:** Save your final Excel dashboard screenshot as `images/dashboard.png` before publishing. The image path above will work once uploaded to GitHub.

## Business problem

Sales growth does not necessarily mean higher profitability. This project explores which products, customer segments, countries, and discount categories contribute most to sales and profit, and identifies potential loss-making areas for further investigation.

## Objectives

- Track total sales, profit, cost of goods sold (COGS), and profit margin.
- Compare sales and profit over time.
- Identify the most and least profitable products and business segments.
- Compare profitability across discount bands and countries.
- Summarize potential improvement opportunities grounded in the results.

## Workflow

1. Reviewed and prepared the Financial Sample dataset in Excel.
2. Created PivotTables to aggregate sales, profit, and COGS by month, product, segment, country, and discount band.
3. Calculated profit margin as **SUM(Profit) / SUM(Sales)** using a DAX measure so that it responds correctly to filter context.
4. Built a dashboard with KPI cards, PivotCharts, and slicers.
5. Reviewed patterns and formulated business recommendations.

## Dashboard metrics

The following figures were observed in the unfiltered dashboard screenshots and **should be rechecked against the final workbook before publication**:

| Metric | Approximate value |
| --- | ---: |
| Total Sales | $118.73M |
| Total Profit | $16.89M |
| Total COGS | $101.83M |
| Overall Profit Margin | 14.23% |

## Preliminary findings

- **Government** had the highest total profit among business segments (approximately **$11.39M**).
- **Enterprise** recorded a negative total profit (approximately **-$0.61M**), making it a priority for further product-level cost investigation.
- **Paseo** had the highest total product profit in the reviewed dashboard (approximately **$4.80M**).
- The **No Discount** group showed a profit margin of roughly **22%**, compared with around **9%** for the **High Discount** group. This is an association in the sample, **not proof that discounts caused lower profit**.

## Recommendations to investigate

- Examine Enterprise profitability by product, COGS, and discount category before changing prices.
- Review margin alongside absolute profit and sales volume when comparing discount groups.
- Monitor profitability by segment and product rather than sales alone.

## Files

- `Sales_Profitability_Dashboard.xlsx` — final Excel workbook, including data, analysis, and dashboard (upload your final version).
- `images/dashboard.png` — screenshot of the finished dashboard (upload your final version).

## Notes and limitations

- The dataset is a Microsoft teaching/sample dataset; it should not be presented as real business experience.
- In this dataset, `Profit` represents the provided sample's profit measure and should not be treated as a complete audited net-income statement.
- Findings are descriptive; they do not establish causal relationships.
- PivotChart and slicer interactivity is available in Excel, not directly inside the GitHub README screenshot. Download the workbook to explore it.

## Author

Portfolio project by an Industrial Engineering student, focused on Excel-based data analysis and business reporting.
