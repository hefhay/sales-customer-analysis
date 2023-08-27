# sales-customer-analysis

```sql
SELECT 
    Datekey, 
    FullDateAlternateKey AS `Date`, 
    EnglishDayNameOfWeek AS `Day`,
    WeekNumberOfYear AS week_no, 
    EnglishMonthName AS `Month`, 
    MonthNumberOfYear AS month_no, 
    LEFT(EnglishMonthName, 3) AS month_short,
    CalendarQuarter AS `Quarter`, 
    CalendarYear AS `Year`
FROM dimdate;
