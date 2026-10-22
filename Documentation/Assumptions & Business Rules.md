**Assumption 1**: Region from Customer_Master is treated as the single source of truth. The Region_Recorded field in the transactions table is ignored for reporting.
**Assumption 2**: Exact duplicate Order_ID rows in the Sales Transactions table were removed. Only one record per Order_ID is retained.
**Assumption 3**: Orders with Order_Status = "Cancelled" are excluded from all revenue, cost, and profit calculations.
**Assumption 4**: Orders with Quantity ≤ 0 are also excluded from revenue metrics.
**Assumption 5**: Only valid orders (Order_Status ≠ Cancelled and Quantity > 0) are considered for Net Sales, Profit, Valid Orders, and related KPIs.
**Assumption 6**: Order Status values were standardized (e.g., “canceled”, “Cancelled”, “CANCELLED” → “Cancelled”).
**Assumption 7**: Channel values were cleaned and grouped into standard categories (Online, Retail, Partner, Unknown).
**Assumption 8**: Blank/null values in Channel and Customer Segment were replaced with “Unknown”.
**Assumption 9**: Returns are analyzed separately from regular sales. Return Rate and Return Value are calculated independently and used for Adjusted Sales after Returns.
**Assumption 10**: Monthly Targets are linked via Salesperson and Region. Target Achievement % is calculated as Net Sales ÷ Revenue Target.
**Assumption 11**: A Calendar table was created and marked as the official Date table for all time-based analysis (YTD, YoY, Monthly trends, etc.).
**Assumption 12**: All monetary values are treated in the same currency unit as provided in the source data (no currency conversion applied).