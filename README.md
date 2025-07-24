# Crop Recommendation & Strategy System

## Project Overview

This project is a comprehensive, data-driven system designed to assist farmers in making informed decisions about crop selection. It leverages a dataset of soil and weather conditions to provide two key functionalities through user-friendly web applications:
1.  **Harvest Helper Pro**: A tool that recommends the most suitable crop based on user-inputted environmental data and provides detailed strategic insights on profitability and seasonal planning.
2.  **Analytics Dashboard**: A visualization platform for exploring the underlying data, allowing users to understand the relationships between environmental factors and crop suitability.

The core of the project is a machine learning model trained on the "Crop Recommendation Dataset" from Kaggle.

---

## Features

### Harvest Helper Pro (`harvest-helper-pro.html`)
* **Personalized Crop Recommendations**: Enter soil data (N, P, K, pH) and weather data (temperature, humidity, rainfall) to get an instant crop suggestion.
* **Crop Strategy Planner**: Look up any crop to see a detailed breakdown of its profitability, planting season, duration, and a crop rotation suggestion.
* **Ideal Conditions Lookup**: View the optimal environmental conditions for any crop in the dataset.

### Analytics Dashboard (`analytics-dashboard.html`)
* **Interactive Visualizations**: Explore the data through a series of charts.
* **Profitability & Calendar Matrix**: A master chart comparing all crops by estimated profit and planting season.
* **Dynamic Filtering**: Filter environmental charts by a specific crop to see its unique data profile.
* **Data-driven Insights**: Understand trends in nutrient requirements, climate needs, and more.

### Python Analysis (`analysis/crop_analysis.py`)
* **Guided EDA**: A Python script that walks through a step-by-step exploratory data analysis.
* **Model Training**: Trains a Random Forest Classifier that achieves ~99% accuracy on the dataset.
* **Modular Visualizations**: Generates individual plots for data distributions, correlations, and conditions per crop.

---

## Technologies Used

* **Backend & Analysis**: Python, Pandas, Scikit-learn, Matplotlib, Seaborn
* **Frontend**: HTML, Tailwind CSS, JavaScript
* **Data Visualization**: Chart.js

---

## How to Run

### 1. Python Analysis
* Navigate to the `analysis/` directory.
* Make sure you have the required libraries installed: `pip install pandas scikit-learn matplotlib seaborn`
* Run the script from your terminal: `python crop_analysis.py`
* The script requires the `Crop_recommendation.csv` file to be in the same directory.

### 2. Web Applications
* No installation is needed.
* Simply open the `harvest-helper-pro.html` or `analytics-dashboard.html` files from the `web-apps/` folder in any modern web browser.
