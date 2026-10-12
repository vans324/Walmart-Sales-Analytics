# Walmart Sales Analytics Dashboard

A responsive, single-file interactive data visualization dashboard built using **Tailwind CSS** and **Chart.js**. The dashboard processes retail sales performance, macroeconomic indicators (CPI, Unemployment), and holiday impact based on the `Walmart_Sales.csv` dataset.

---

## 🌟 Key Features

- **Header Controls & Dynamic Filtering**:
  - **Store Selector**: Drill down into specific stores (Store 1 to 45) or view aggregated metrics for all stores combined.
  - **Holiday Filter**: Toggle view between all weeks, holiday weeks only, or non-holiday weeks.
  - **Year Filter**: Filter dynamic performance by calendar year (2010, 2011, 2012).
  - **Reset Button**: One-click action to reset all dropdown filters to default settings.

- **Real-Time KPI Cards**:
  - **Total Weekly Sales**: Aggregated total revenue formatted dynamically.
  - **Average Weekly Sales**: Mean weekly revenue across current selections.
  - **Active Stores Count**: Total active store network locations.
  - **Macroeconomic Indicators**: Average Consumer Price Index (CPI) and Unemployment Rate.

- **Interactive Charts (Chart.js)**:
  1. **Time-Series Sales Trend (Line Chart)**: Tracks weekly sales over time to highlight seasonal and holiday demand spikes.
  2. **Holiday Impact (Doughnut Chart)**: Compares total sales volume share between holiday and non-holiday weeks.
  3. **Top 10 Stores Performance (Bar Chart)**: Ranks top-performing locations by average weekly sales.
  4. **Macroeconomic Correlation (Scatter Plot)**: Analyzes relationships between Unemployment Rate and Weekly Sales revenue.

- **Interactive Data Table**:
  - Aggregated performance summary table per store.
  - Quick search filter to find specific store entries.
  - Instant **Drill Down** action buttons that filter the entire dashboard to a target store.

---

## 🚀 Tech Stack

- **HTML5 & Vanilla JavaScript**: Core structure, dataset processing, and dynamic reactivity without heavy frame dependencies.
- **Tailwind CSS (via CDN)**: Utility-first styling for layout, custom scrollbars, and modern UI cards.
- **Chart.js (via CDN)**: Interactive rendering for lines, bars, doughnut charts, and scatter plots.
- **FontAwesome (via CDN)**: Vector icons for intuitive visual cues.

---

## 📁 File Structure

```text
├── walmart_dashboard.html   # Complete single-file application (HTML, CSS, JS, and Dataset)
└── README.md                # Project documentation
```

---

## 💻 Getting Started

Since the dashboard is built inside a single client-side file with an embedded dataset structure, **no server setup, npm installation, or database configuration is required**.

1. Download or clone `walmart_dashboard.html`.
2. Double-click or open `walmart_dashboard.html` in any modern web browser (Google Chrome, Mozilla Firefox, Edge, or Safari).
3. Start interacting with the filters, charts, and drill-down buttons!

---

## 📊 Dataset Schema Reference

The dataset structure processed by the dashboard follows standard schema conventions:

| Column Header | Data Type | Description |
| :--- | :--- | :--- |
| `Store` | Integer | Store identification number (1–45) |
| `Date` | String | Weekly date stamp (`YYYY-MM-DD`) |
| `Weekly_Sales` | Float | Total revenue generated in a given week |
| `Holiday_Flag` | Integer | Binary indicator (`1` = Holiday week, `0` = Non-Holiday week) |
| `Temperature` | Float | Average regional temperature during the week (°F) |
| `Fuel_Price` | Float | Cost of fuel in the region ($/gal) |
| `CPI` | Float | Consumer Price Index metric |
| `Unemployment` | Float | Regional unemployment rate percentage |

---

## 📜 License

This project is open-source and available for educational, personal, and portfolio demonstration purposes.
```