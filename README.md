# Electric Vehicle Market Analysis in India (2014–2024)

## Introduction
This repository contains an exploratory data analysis (EDA) project evaluating the adoption, growth trajectories, and market dynamics of Electric Vehicles (EVs) across India over a decade (2014–2024). Analysing over 96,000 regional registration records, the project uncovers structural trends in micro-mobility, state-level penetration, and commercial fleet electrification.

---

## Data Source
* **Primary Origin:** Central registration records from the **Vahan Dashboard**, maintained by the **Ministry of Road Transport and Highways (MoRTH), Government of India**.
* **Access Platform:** Sourced via **Kaggle** as a compiled multi-year dataset spanning vehicle categories, specific classes, monthly registration counts, and regional states/UTs.

---

## Project Description & Workflow
The analysis is implemented in a single Jupyter Notebook (`india_ev_sales_analysis.ipynb`) using pure Python, Pandas, Matplotlib, and Seaborn:

1. **Environment Setup & Data Hygiene:** Verified structural integrity, zero missing values, and duplicate-free baseline data.
2. **Data Transformation & Memory Optimisation:** Optimised DataFrame memory consumption by over 65% through schema casting (`datetime64`, `int32`, `category`).
3. **Feature Engineering:** Extracted temporal components (Quarters, Year-Month periods) and segmented vehicles into commercial, personal, shared, and freight categories.
4. **Visualisation Suite (20 Visualisations):**
   * **Macro Trends:** National volume trajectories, complete-year Year-over-Year (YoY) growth rates, monthly seasonality heatmaps, and 3-month moving average trends.
   * **Segment Dynamics:** Category market share donut charts, 100% stacked area evolution, top 10 vehicle class breakdowns, and personal vs commercial fleet adoption.
   * **Geographic Hotspots:** Top 10 vs Bottom 10 state comparisons, multi-year state trajectories, state-category heatmaps, and Pareto concentration analysis (80/20 rule).
   * **Sectoral Deep-Dives:** 2-Wheeler vs 3-Wheeler micro-mobility preferences, public transit bus electrification, and log-scaled sales volatility box plots.
   * **Commercial Fleet & Freight:** Cargo EV adoption by state, 4-Wheeler personal vs fleet growth, quarterly purchasing cycles, and E-Rickshaw vs regular auto splits.

---

## Key Commercial Insights

* **Micro-Mobility Dominance:** 2-Wheelers and 3-Wheelers represent over **95% of total cumulative EV registrations**. High-speed passenger cars (4-Wheelers) and public transit buses remain in early adoption stages.
* **Geographic Pareto Concentration:** The top 10 states drive approximately **80% of all national EV volume**, led by Uttar Pradesh, Maharashtra, Karnataka, and Delhi.
* **Regional Dichotomy:** Northern, Central, Eastern and North-Eastern states (e.g., Uttar Pradesh, Bihar, Uttarakhand, Assam, Madhya Pradesh) are heavily driven by commercial 3-Wheeler E-Rickshaws, whereas Southern and Western states (e.g., Maharashtra, Karnataka, Telangana, Rajasthan, Gujarat) are dominated by personal 2-Wheeler (scooters) and 4-Wheelers (cars).
* **Commercial Freight Uptick:** Cargo 3-Wheelers and light commercial delivery fleets have seen rapid acceleration post-2021 due to favourable total cost of ownership (TCO) in urban logistics.

---

## How to Run
1. Clone or download this repository.
2. Ensure you have the required libraries installed:

   ```bash
   pip install numpy pandas matplotlib seaborn
   ```

3. Open `india_ev_sales_analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab and run all cells sequentially.
