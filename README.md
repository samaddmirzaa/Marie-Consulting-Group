# Marie Consulting Group: Data Visualization Portfolio

A collection of data analysis and visualization projects completed as part of a simulated consulting role at **Marie Consulting Group (MCG)**, a multinational advisory firm. Each notebook tackles a real client brief across three industries: hospitality, coffee, and automotive.

---

## Projects

### 01 | Hotel Industry: Matplotlib Foundations
**Client: Internal (MCG Onboarding)**

Exploratory analysis of hotel customer data using core Matplotlib techniques.

- Line charts tracking monthly lodging and other revenue over time
- Dual-axis charts comparing two scaled metrics on a single figure
- Pie and donut charts breaking down revenue share by customer nationality
- Scatter and bubble charts comparing average nights stayed vs. revenue per customer
- Overlapping histograms comparing customer age distributions across countries

**Data:** `Data/HotelCustomersDataset.xlsx`

---

### 02 | Coffee Industry: Deep Dive (Part 1)
**Client: Sarah Shark, Managing Director**

Analysis of global coffee production and trade dynamics, with a focus on Brazil's position relative to other producing and importing nations.

- Bar chart of the top 10 coffee-producing nations (1990 to 2018)
- Line chart tracking the top 5 producers over time
- Stacked area chart comparing Brazil vs. the rest of the world
- Donut charts showing Brazil's share of global production in 1990 and 2018
- Dual-axis bar chart comparing importer consumption volumes against average prices paid

**Data:** `Data/total-production.csv`, `Data/imports.csv`, `Data/retail-prices.csv`

---

### 02 | Coffee Industry: Summary Report (Part 2)
**Client: Clarissa Café, Coffee Client**

Combines the findings from Part 1 into a single multi-panel figure report using `GridSpec` and Matplotlib subplots.

- Meshgrid layout composing five charts into one exportable figure
- National flag colors applied to each country's bars and chart segments
- Horizontal bar chart of top producers with a paired pie chart for 2018 market share
- Subplot grid of price-paid-to-growers histograms for Brazil, Colombia, Ethiopia, and all other nations

**Data:** `Data/total-production.csv`, `Data/imports.csv`, `Data/prices-paid-to-growers.csv`

---

### 03 | Hotel Industry: Subplots and Grid Layouts
**Client: Internal (MCG Onboarding)**

Builds on the hotel dataset using more advanced layout techniques.

- 2x3 subplot grid of lodging revenue distributions across the top 5 customer countries
- GridSpec-based month-end revenue report combining a time series line chart, a flag-colored bar chart by country, and a donut chart tracking France's 2018 revenue goal

**Data:** `Data/HotelCustomersDataset.xlsx`

---

### 04 | Hotel Industry: Seaborn Charts
**Client: Internal (MCG Onboarding)**

Uses Seaborn to explore the hotel dataset with more advanced statistical chart types.

- Histogram of lodging revenue distribution with investigation into zero-revenue bookings
- Horizontal bar chart of average room nights for the top 5 customer countries
- Box plots and violin plots comparing lodging revenue and age distributions across nationalities
- Regression plots (regplot and lmplot) examining the relationship between room nights and revenue
- Pairplot matrix of numeric hotel features
- Heatmaps of a nationality-by-market-segment pivot table and the full correlation matrix

**Data:** `Data/HotelCustomersDataset.xlsx`

---

### 05 | Automotive Industry: Fleet Truck Procurement (Final Project)
**Client: Aaron Auto, VP of Fleet Management**

Analyzes a used car auction dataset to identify the best Ford F-150 XLT models for fleet acquisition.

- Pairplot with body-style hue to explore numeric variable relationships
- Correlation heatmap of all numeric features
- `lmplot` regression lines comparing odometer vs. selling price across four major brands
- Bar chart of average price deviation from MMR (market recommended price) by exterior color
- Heatmap of average selling price by trim level and condition rating
- Two-panel bar chart comparing price-to-MMR ratio and available inventory by state to pinpoint the best sourcing location

**Data:** `Data/car_prices.csv`

---

## Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data ingestion, reshaping, groupby aggregations, pivot tables |
| `numpy` | Numerical operations and array manipulation |
| `matplotlib` | Core charting, subplots, GridSpec layouts, dual-axis figures |
| `seaborn` | Statistical charts, regression plots, heatmaps, pairplots |

---

## Repository Structure

```
.
├── Data/
│   ├── HotelCustomersDataset.xlsx
│   ├── total-production.csv
│   ├── imports.csv
│   ├── retail-prices.csv
│   ├── prices-paid-to-growers.csv
│   └── car_prices.csv
├── 01_assignments.ipynb
├── 02_Coffee_Project_Part1.ipynb
├── 02_Coffee_Project_Part2.ipynb
├── 03_assignments.ipynb
├── 04_assignments.ipynb
├── 05_final_project.ipynb
└── README.md
```

---

## Getting Started

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install pandas numpy matplotlib seaborn openpyxl
jupyter notebook
```

Open any notebook and run the cells in order. All data files are expected in the `Data/` folder relative to each notebook.
