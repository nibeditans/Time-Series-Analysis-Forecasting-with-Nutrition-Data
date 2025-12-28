# Nutrition Time Series Analysis (2022–2025)

## About This Project

This repository contains my **end-to-end Time Series Analysis project**, built using a **synthetic nutrition dataset**.

I created this project to deeply understand **how time-based data works in real-world scenarios**, not just from an analysis point of view, but also from a **data storytelling and business perspective**.

Instead of jumping straight into complex models, I intentionally focused on:

* Designing a realistic dataset using **NumPy** and **Pandas**
* Handling dates and time correctly
* Building strong intuition around trends and seasonality
* Communicating insights clearly using **Power BI** and **Tableau**

Check out the complete article I have written on this Project: [Building a Real-World Time Series Project with Nutrition Data](https://nsdsda.medium.com/building-a-real-world-time-series-project-with-nutrition-data-eff2970c2c8f).

If you wanna explore from the very basic, go for this first: [Handling Dates, Times & Time Series Data in Pandas](https://pub.towardsai.net/handling-dates-times-time-series-data-in-pandas-d4e8fcc46c62).


## What I Wanted to Achieve?

Through this project, I aimed to:

* Learn how **time series data should be structured and handled**
* Avoid common mistakes related to dates, aggregation, and leakage
* Analyze **trends, seasonality, and variability** in a simple and explainable way
* Build **clean dashboards** that make sense to non-technical users 
* Showcase my skills across **Python, Power BI, and Tableau**


## 📂 Project Structure

```
├── Notebooks/
│   ├── 00_Notebook.ipynb (Data Generation Code using NumPy and Pandas)
│   ├── 01_Notebook.ipynb (Handling Time-Based Data)
│   ├── 02_Notebook.ipynb (Time Series Analysis)
│   └── 03_Notebook.ipynb (Time Series Forecasting)
│
├── Data/
│   ├── nutrition_data.csv
│   ├── nutrition_updated.csv
│   └── nutrition_meal_summary.csv
│
├── Power_BI/
│   └── TSAF.pbix
│   └── TSAF.pdf
│
├── Tableau/
│   └── TSAF_Tableau.png
│
└── README.md
```


## About the Dataset

### Dataset Nature

* The dataset is **synthetic but realistic**
* I intentionally added **noise, missing values, and skipped meals**
* This helps mimic how real nutrition or habit-tracking data behaves

### Time Coverage

* **Date Range:** January 2022 - December 2025
* **Granularity:** Meal-level data, later aggregated to daily and monthly levels

### Key Columns

* `Date`
* `Meal` (Breakfast, Lunch, Supper, Dinner)
* `Calories`
* Macros in grams: `Protein_g`, `Carbs_g`, `Fat_g`
* Water in ml: `Water_ml` 

Missing values are intentional and are used later to demonstrate **realistic cleaning and analysis workflows**.


## Notebooks Walkthrough

### 1. Dataset Generation & Overview

In this notebook, I:

* Generate the full synthetic dataset
    * NumPy for Generating Data
    * Pandas for Storing the data into DataFrame
* Explain the assumptions behind the data
* Save the dataset as `nutrition_data.csv` for reuse

### 2. Handling Dates, Times, and Time Series Data

Here, I focus on:

* Converting and validating datetime columns
* Setting up a proper time index
* Resampling and aggregating time-based data
* Building intuition around rolling windows and time slicing

### 3. Time Series Analysis

In this notebook, I:

* Aggregate data to daily and monthly levels
* Explore trends, seasonality, and noise
* Apply moving averages and decomposition
* Introduce stationarity concepts using simple explanations

### 4. Time Series Forecasting

Finally, I:

* Perform time-aware train–test splitting
* Start with Naive baselines
* Apply simple forecasting models (Exponential Smoothing, basic ARIMA)
* Evaluate forecasts using MAE and RMSE

The focus here is **understanding behavior**, not chasing perfect predictions.


## Business Intelligence Dashboards

### Power BI

I built a **2-page Power BI report**:

* **Overview & Trends**: long-term nutrition patterns.
* **Meal-wise Behavior Analysis**: how different meals contribute?

The goal was to translate Python analysis into **clear and business-friendly visuals**.

### Tableau

I also created a **single-page Tableau dashboard**:

* Clean and minimal design
* Focused on trend visualization
* Built to showcase Tableau as a separate BI skill

I intentionally kept Tableau simple and elegant, without overloading it with filters or KPIs.
![TSAF_Tableau.png](https://github.com/nibeditans/Time-Series-Analysis-Forecasting-with-Nutrition-Data/blob/main/TSAF_Tableau.png)

Tableau Public Tashboard: [Nutrition Trends Overview (2022–2025)](https://public.tableau.com/views/NutritionTrendsOverview20222025/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)


## Tools & Technologies I Used

### Programming & Analysis

* Python
* NumPy
* Pandas
* Matplotlib
* StatsModels
* Scikit-learn

### Visual Storytelling

* Power BI
* Tableau


⭐ If you found this project helpful or interesting, feel free to star and fork the repository!
