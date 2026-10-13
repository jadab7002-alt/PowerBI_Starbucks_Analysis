# Starbucks Beverage & Store Analysis

A Power BI dashboard that compares Starbucks beverage categories by calories, sugar and caffeine, and shows Starbucks' global store presence.

## Questions Answered

- Which beverage categories are highest in calories, sugar and caffeine?
- How many drinks does each category offer?
- Where are Starbucks stores located?

## Dashboard

- **KPI cards:** total beverages, average sugar, average calories, average caffeine
- **Area chart:** average calories by beverage category
- **Column chart:** Starbucks global presence
- **Donut chart:** beverage category distribution
- **Bar chart:** average caffeine by category
- **Top 5 highest caffeine beverages:** ranked with images
- **Slicers:** protein range, beverage prep

## Data Model

| Table | Contents |
|---|---|
| `starbucks` | Beverage nutrition data (calories, fat, sugars, protein, caffeine, etc.) |
| `directory` | Store locations (city, country, latitude, longitude, etc.) |
| `Top5_Caffeine` | Beverages with the highest caffeine |
| `Measure` | DAX measures |

## DAX Measures

```DAX
Total Beverages = DISTINCTCOUNT(starbucks[Beverage])
Avg calories    = AVERAGE(starbucks[Calories])
Avg sugars      = AVERAGE(starbucks[ Sugars (g)])
Avg Caffeine    = AVERAGE(starbucks[Caffeine (mg)])
```

## Tools

Power BI Desktop, Power Query, DAX

## How to Open

Download `PowerBI_Starbucks_Analysis.pbix` and open it in Power BI Desktop (Windows).

## ScreenShots

DashBoard_Preview: (https://github.com/jadab7002-alt/PowerBI_Starbucks_Analysis/blob/main/Dashboard_View.png)
