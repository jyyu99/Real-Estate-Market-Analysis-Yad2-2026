🏠 Real Estate Market Analysis 2026 | Yad2 Insights
An end-to-end data analytics project featuring a Python-based ETL pipeline and an interactive Power BI Dashboard. This project analyzes real estate listings from Israel's leading portal (Yad2) to uncover pricing trends, regional demand, and investment opportunities in 2026.

(Replace this with your actual image path later)

🚀 Project Overview
This project bridge the gap between raw web-scraped data and actionable business intelligence. It covers:

Data Wrangling: Cleaning messy Hebrew-based real estate data using Python.

Feature Engineering: Calculating KPIs like Price per SQM and identifying market outliers.

Interactive Visualization: A user-friendly dashboard for deep-diving into neighborhoods and street-level data.

🛠️ Tech Stack
Language: Python 3.x

Libraries: Pandas, NumPy (Data Cleaning & Analysis)

Visualization: Power BI Desktop

DAX: Advanced measures for dynamic KPIs

Dataset: Cleaned Yad2 listings (2026)

📂 Directory Breakdown
data/: Separating raw and cleaned data is crucial for reproducibility. The cleaned_data.csv is the result of the Python pipeline.

notebooks/: Contains the "heavy lifting." This is where I handled Hebrew string reversals, removed outliers (e.g., apartments with 0 rooms or 1m NIS/sqm), and formatted prices.

dashboard/: The .pbix file. This contains the DAX measures, the data model, and the final interactive UI.

images/: Essential for GitHub. Since people can't "run" a Power BI file inside GitHub, these screenshots act as your portfolio's front window.
🧠 Phase 1: Python Data Cleaning
The raw data was "noisy" with Hebrew encoding issues and missing values. Key steps included:

Normalization: Standardized area (SQM) and price formats.

Outlier Removal: Filtered out unrealistic listings (e.g., 0 NIS prices or 1,000,000 SQM apartments).

Hebrew Support: Handled Right-to-Left (RTL) string formatting for cities and streets.

Calculated Columns: Created Price_per_SQM to allow fair comparisons between regions.

📊 Phase 2: Power BI Dashboard Features
The dashboard is designed for both casual buyers and professional investors:

Dynamic KPIs: Real-time tracking of Total Listings, Average Price, and Price per SQM.

Hierarchical Slicers: Drill down from City ➔ Neighborhood ➔ Street.

Regional Heatmap: Visualizing property density across Israel.

Price Distribution: Bar charts comparing "Average Price per SQM" by settlement to identify "Value for Money" areas.

Quick Reset: A dedicated button to clear all filters instantly.

💡 Key Market Insights (2026)
This dashboard leverages data from over 9,900 active listings to reveal critical market dynamics:

Valuation Disparities: The "Price per SQM" ranking exposes significant valuation gaps between central hubs and peripheral cities, helping users identify undervalued areas relative to the national average of ~₪15,600/sqm.

Luxury Market dominance: As highlighted in the "Top 10 Settlements" chart, the luxury segment is led by exclusive communities (e.g., Kfar Shmaryahu, Savyon), where average asking prices far exceed the national baseline of ₪3.45M.

Supply Composition: The "Property Type" donut chart reveals a market heavily skewed towards standard apartments (~67%), with niche assets like Garden Apartments and Penthouses representing a smaller, premium fraction of the inventory.

Demand Hotspots: The geographic heatmap visually confirms that market activity and high-price clusters are densely concentrated in the Gush Dan (Tel Aviv Metropolitan) and coastal regions, fading significantly as you move inland.

📝 How to Use
Python: Run the data_cleaning.ipynb to see the transformation logic.

Power BI: Open yad2_analysis_2026.pbix (requires Power BI Desktop).

Explore: Use the sidebar to filter by budget and location.
