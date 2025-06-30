# Global Happiness Power BI Dashboard (2015–2023)

## Overview

This Power BI project analyzes nine years of World Happiness Report data (2015–2023), providing an interactive, multi-dimensional view of well-being, economic indicators, and global trends across countries and regions.

It demonstrates the use of Power Query transformations, data modeling, DAX calculations, and Power BI storytelling techniques.

---

## Data Sources

| Dataset | Description |
|---------|-------------|
| `happiness_data.csv` | Merged and cleaned dataset from WHR 2015–2023 |
| Source | [Kaggle: World Happiness Report](https://www.kaggle.com/datasets/mathurinache/world-happiness-report) |

Merged in Power Query from yearly reports into one unified `HappinessData` table.

---

## Dashboard Features

- Time slider: 2015–2023 happiness trends
- Interactive map by country & region
- KPI cards for GDP, Freedom, Generosity, Health
- GDP vs Happiness scatter plot
- Slicers: Year, Region, Country
- Correlation and YoY comparisons

---

## DAX Measures Used

- `Avg Happiness Score`
- `Avg GDP`, `Avg Freedom`, `Avg Generosity`, `Avg Health`
- `YoY Happiness Change`
- `Min/Max Rank by Country`
- `GDP vs Happiness Correlation (RANKX + AVERAGE + SCATTER)`

---

## Visual Highlights

| Visual | Description |
|--------|-------------|
| Map | Happiness score by country |
| Line chart | Global average over time |
| Bar chart | Top 10 happiest countries |
| KPI cards | Metric summaries |
| Scatter plot | GDP vs Happiness |


---

## Model View

This project uses:
- 9 separate WHR tables → merged into `HappinessData`
- Star schema with date and measures tables
- Custom DAX measures stored in `MeasuresTable`
- `YearTable` for time intelligence

---

## Folder Structure

global_happiness_powerbi/
├── data/
│ └── happiness_data.csv
├── dashboard/
│ └── global_happiness_dashboard.pbix
├── screenshots/
│ ├── overview_page.png
│ ├── narrativeq&a.png
│ └── model_view.png
└── README.md

---

## Author

**Don Richardson Bayya**  
---


