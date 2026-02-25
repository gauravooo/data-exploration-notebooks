# Real Estate Exploratory Data Analysis (EDA)

## Project Overview
This repository contains an end-to-end Exploratory Data Analysis (EDA) on the Ames Housing dataset. The objective of this notebook is to ingest raw, real-world data, handle missing values (imputation), and extract statistical and visual insights to determine which features most strongly predict the final sale price of a home. 

## Key Findings
* **Primary Value Driver:** The correlation heatmap reveals that `OverallQual` (Overall Material and Finish Quality) is the single strongest mathematical predictor of a home's `SalePrice`.
* **Secondary Drivers:** `GrLivArea` (Above Ground Living Area) and `GarageCars` also show highly positive linear correlations with price.
* **Price Distribution:** The target variable (`SalePrice`) exhibits a right-skewed distribution, indicating a concentration of homes in the median price range with a long tail of high-value outliers.

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn

## Engineering Pipeline
1. **Data Ingestion & Inspection:** Loaded tabular data and identified structural gaps.
2. **Data Cleaning:** Implemented systematic imputation techniques (e.g., `.fillna()`) to handle missing `NaN` values without unnecessarily dropping valuable rows.
3. **Statistical Aggregation:** Utilized Pandas `groupby()` and `.agg()` to summarize metrics.
4. **Visual Storytelling:** Built distribution histograms, scatter plots for linear relationships, and a correlation matrix heatmap to isolate mathematical weights.

## How to Run Locally
1. Clone this repository:
   `git clone https://github.com/gauravooo/data-exploration-notebooks.git`
2. Ensure you have the required libraries installed:
   `pip install pandas numpy matplotlib seaborn`
3. Download the `train.csv` file from the [Kaggle House Prices Competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) and place it in the project root.
4. Open and run `house_prices_eda.ipynb` in Jupyter Notebook or VS Code.