# Monthly Sales Trend – Superstore

**Task 17 – Monthly Sales Trend**
Veda Technology | Data Analytics Track | Level 1, Day 17

## About
I summarized the sales of the Sample Superstore dataset by month (January 2014 to December 2017, 48 months) and visualized the trend in a line chart using Excel.

## Dates: how I handled them
Some of the original `Order Date` values were stored as text, so Excel could not group them by month. I added a helper column, `Order Date Fixed`, that converts every date into a real Excel date. The monthly table uses a real date for each month (1st of the month), so the months sort in the correct chronological order and the chart axis is a proper date axis.

## Monthly table
The table has one row per month with:
- **Total Sales** – `SUMIFS` of Sales between the first and last day of the month
- **Order Lines** – `COUNTIFS` of the transactions in that month

The 48 monthly totals add up to the grand total of 2,297,201 sales and 9,994 order lines.

## Yearly totals
| Year | Total Sales |
|------|-------------|
| 2014 | 484,248 |
| 2015 | 470,533 |
| 2016 | 609,206 |
| 2017 | 733,215 |

## Chart
A line chart of monthly sales from 2014 to 2017, with a date axis, axis titles and a descriptive title.

## Findings
- **Sales trend upward over the four years.** There was a small dip in 2015, and then sales grew strongly in 2016 and 2017.
- **Sales are seasonal.** The strongest months are towards the end of the year. For example, November 2017 was the highest month (118,448), and in 2016 November (79,412) and December (96,999) were also high.
- **Early months are weak.** February 2017 was the lowest month of that year (20,301), compared to 118,448 in November.

## Files
- `Monthly_Sales_Trend.xlsx` – workbook with the Raw Data tab and the Monthly Trend tab (table, formulas and line chart)
- `monthly_trend_screenshot.png` – screenshot of the Monthly Trend tab
- `README.md`

## Tools used
Microsoft Excel (EDATE, EOMONTH, SUMIFS, COUNTIFS, line chart)

## Author
Rabia
