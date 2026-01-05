# 🏠 Real Estate Market Analysis 2026 | Yad2 Insights

An end-to-end data analytics project featuring a **Web-Scraping & Python-based ETL pipeline** and an interactive **Power BI Dashboard**. This project analyzes real estate listings from a leading portal (Yad2) to uncover pricing trends, regional demand, and investment opportunities in 2026.

![yad2_dashboard_page-0001](https://github.com/user-attachments/assets/3caf1b55-dd0e-47fe-86bf-3001e6789367)

---

## 🚀 Project Overview
This project bridges the gap between raw web-scraped data and actionable business intelligence. It covers:
* **Data Acquisition:** Scraping real-time listings to build a proprietary dataset.
* **Data Wrangling:** Cleaning messy, Hebrew-based real estate data using Python.
* **Feature Engineering:** Calculating KPIs like Price per SQM and identifying market outliers.
* **Interactive Visualization:** A user-friendly dashboard for deep-diving into neighborhoods and street-level data.

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy (Data Cleaning & Analysis), Selenium/BeautifulSoup (Scraping)
* **Visualization:** Power BI Desktop
* **DAX:** Advanced measures for dynamic KPIs
* **Dataset:** 9,900+ Yad2 listings (2026)

---

## 📂 Directory Breakdown
* `data/`: Contains `raw_data.csv` and the final `cleaned_data.csv` resulting from the Python pipeline.
* `notebooks/`: Contains the "heavy lifting" (Jupyter Notebooks). Includes scraper logic and data cleaning (handling Hebrew RTL, outlier removal, and price formatting).
* `dashboard/`: The `.pbix` file containing the data model, DAX measures, and the interactive UI.
* `images/`: High-resolution screenshots of the dashboard for quick previewing.

---

## 🧠 Phase 1: Data Acquisition & Cleaning
The project starts with raw data that is inherently "noisy" due to web-scraping artifacts and Hebrew encoding.

1. **Scraping:** Automated collection of listing details (Price, Area, Rooms, Location).
2. **Normalization:** Standardized numerical formats for prices and square footage.
3. **Outlier Removal:** Filtered unrealistic listings (e.g., ₪1 prices or 1,000,000 SQM apartments) to protect KPI accuracy.
4. **Hebrew Support:** Resolved Right-to-Left (RTL) formatting for correct display of cities and streets.
5. **Calculated Columns:** Engineered the `Price_per_SQM` metric to enable fair regional comparisons.

---

## 📊 Phase 2: Power BI Dashboard Features
The dashboard is designed for both casual buyers and professional investors:
* **Dynamic KPIs:** Real-time tracking of Total Listings, Average Price, and Price per SQM.
* **Hierarchical Slicers:** Deep-drill functionality from **City ➔ Neighborhood ➔ Street**.
* **Regional Heatmap:** Visualizes property density and demand clusters.
* **Price Distribution:** Bar charts comparing "Average Price per SQM" by settlement to identify "Value for Money" areas.
* **Quick Reset:** Integrated UX button to clear all active filters instantly.

---

## 💡 Key Market Insights (2026)
Based on the analysis of **9,900+ active listings**:
* **Valuation Disparities:** The ranking exposes significant valuation gaps between central hubs and peripheral cities, identifying undervalued areas relative to the national average.
* **Luxury Market Dominance:** The luxury segment is led by exclusive communities (e.g., **Kfar Shmaryahu, Savyon**), where asking prices far exceed the ₪3.45M baseline.
* **Supply Composition:** Standard
