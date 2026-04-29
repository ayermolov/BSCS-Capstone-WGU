# Retail Inventory Demand Forecaster

## Overview
This project is a machine learning-based application designed to help retail managers optimize inventory levels by accurately predicting product demand. By moving away from static historical averages, this tool uses a **Random Forest Regressor** to estimate sales volume based on dynamic variables such as pricing, seasonal trends, weather conditions, and promotional discounts. 

The goal of this project is to provide a data-driven approach to inventory management, minimizing the financial risks associated with overstocking (wasted capital/space) and stockouts (lost sales).

## Key Features
*   **Exploratory Data Analysis (EDA):** Generates automated visualizations (Histograms, Scatter Plots, and Bar Charts) to explore historical sales trends, pricing correlations, and seasonal/weather impacts.
*   **Data Preprocessing:** Handles categorical variables through One-Hot Encoding to prepare raw CSV data for machine learning ingestion.
*   **Predictive Modeling:** Utilizes a Random Forest Regressor, trained on an 80/20 data split, to forecast future sales.
*   **Interactive User Interface:** Features a built-in Jupyter Notebook widget dashboard allowing users to input hypothetical scenarios (Price, Discount, Weather, Season, Holiday) and receive instant sales predictions.

## Tech Stack
*   **Language:** Python 3
*   **Environment:** Jupyter Notebook
*   **Data Manipulation:** Pandas, NumPy
*   **Machine Learning:** Scikit-Learn
*   **Data Visualization:** Matplotlib, Seaborn
*   **User Interface:** IPyWidgets

## Installation & Setup
To run this project locally on your machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ayermolov/BSCS-Capstone-WGU.git
   cd WGU-BSCS-Capstone
   ```

2. **Install the required dependencies:**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn ipywidgets notebook
   ```

3. **Launch the application:**
   ```bash
   jupyter notebook
   ```
   *Click on `Capstone_Task_2_v2.ipynb` to open the project.*

## How to Use
1. Once the Jupyter Notebook is open, click **Cell > Run All** from the top menu.
2. The notebook will automatically clean the data, generate the historical charts, train the machine learning model, and output the validation metrics (MSE and R-squared).
3. Scroll to the very bottom of the notebook to find the **Retail Inventory Forecaster** dashboard.
4. Adjust the sliders and dropdown menus for Price, Discount, Holiday, Weather, and Season.
5. Click **Predict Sales** to see the machine learning model's forecasted unit sales for that specific scenario!

## Model Evaluation
The predictive model is evaluated using standard regression metrics to ensure accuracy:
*   **R-squared ($R^2$) Score:** Measures how well the variance in the independent variables explains the variance in units sold.
*   **Mean Squared Error (MSE):** Calculates the average squared difference between the estimated values and the actual values.

---
*Note: This project was completed as the final Capstone for the B.S. Computer Science program at Western Governors University (WGU).*

***

