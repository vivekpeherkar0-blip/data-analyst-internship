# Superstore Sales Analysis (Data Analyst Internship - Beginner Level)

## Dataset
- Name: Superstore Sales dataset (Kaggle: vivek468/superstore-dataset-final)
- Link: https://www.kaggle.com/datasets/vivek468/superstore-dataset-final
- File: Sample_Superstore.csv (9,994 order lines, Jan 2014 to Dec 2017, USD)
- Columns used: Order ID, Order Date, Customer, Segment, State, Region, Category, Sub-Category, Product Name, Sales, Quantity, Discount, Profit

## Files
- Superstore_Sales_Dashboard.xlsx : full workbook
  - Dashboard : KPIs and 8 charts
  - Insights : observations and recommendations
  - Analysis : summary tables (all formulas)
  - Clean_Data : cleaned dataset (9,993 rows)
  - Raw_Data : original dataset
  - Cleaning_Log : cleaning steps
- Sample_Superstore.csv : original data
- Video_Script.md : notes for the explanation video

## Data Cleaning
- Order Date was text, converted to date
- 1 duplicate row removed (9,994 -> 9,993 rows)
- No missing values found
- 16 product names had extra spaces, trimmed
- Dropped columns not needed (Row ID, Ship Date, Country, Postal Code, Product ID)
- Added Year, Month, New Order flag (to count orders correctly, because 1 order has many lines)

## Metrics
- Total Sales: $2,296,919
- Total Profit: $286,409
- Orders: 5,009
- Avg Order Value: $459
- Profit Margin: 12.5%

## Key Insights
- Overall: Total sales $2,296,919, profit $286,409 (margin 12.5%) from 5,009 orders. Average order value $459.
- Growth: Sales grew from $483,966 (2014) to $733,215 (2017). 2015 dipped 2.8%, then 2016 grew 29.5% and 2017 grew 20.4%. Profit also rose every year after 2014.
- Seasonality: Strongest months are Nov, Dec and Sep. Sep-Dec together give 51.6% of all sales, so demand is year-end heavy. Jan and Feb are the weakest.
- Category: Technology earns the best margin (17.4%), Office Supplies is close (17.0%), but Furniture has only 2.5% margin even with sales of $741,718.
- Products: Best sellers by sales: Phones, Chairs, Storage. Loss-making sub-categories: Tables, Bookcases, Supplies. Tables alone lost $17,725.
- Region: West has the highest sales ($725,458) and best margin (14.9%). Central has the lowest margin (7.9%) of all four regions, even though its sales ($501,240) are higher than South.
- Segment: Consumer gives 50.6% of sales, Corporate 30.7%, Home Office 18.7%.
- Discount: Orders with discount above 40% have a margin of -77.4% (loss of $99,559), while orders without discount earn 29.5%. Heavy discounting is the main reason for losses.
- States: Top states: California ($457,688), New York ($310,876), Texas ($170,188).

## Recommendations
- Cap discounts at around 20-30% and stop deep discounts (above 40%), mainly on Furniture and Machines.
- Review pricing and supplier cost of Tables, Bookcases, Supplies, which lose money.
- Plan stock and marketing before Sep-Dec, because that is when most sales happen.
- Run bundle or festive offers in Jan-Feb to lift the weak months.
- Push Technology and Office Supplies, which give higher margin; investigate why Central region margin is lower.

## Tools
Microsoft Excel (SUMIFS, COUNTIFS, RANK, charts)
