# Smart Agricultural Supply Chain – Agrifair IBM Project

An exploratory data analysis and machine-learning project focused on understanding key factors in an agricultural supply chain, including commodity prices, demand estimates, harvest quantities, transportation costs, farmer payouts, consumer savings, and spoilage.

The project is implemented in **Python using Google Colab** and is organized into four parts.

## Project objectives

- Load and preprocess agricultural supply-chain data.
- Explore commodity-wise prices and compare demand estimates with harvest quantities.
- Analyze transportation costs across different transit modes.
- Compare traditional and dataset-provided fair retail prices.
- Examine baseline and dataset-provided optimized spoilage values.
- Train a Random Forest regression model to estimate the dataset's existing demand-estimate field.
- Summarize the analysis through a final dashboard and exported reports.

## Project structure

The notebook follows this four-part workflow:

| Part | Description |
|---|---|
| Part 1 | Data loading and preprocessing |
| Part 2 | Exploratory Data Analysis (EDA) |
| Part 3 | Random Forest demand-estimate modeling and supply-chain comparisons |
| Part 4 | Final project summary, dashboard, and report generation |

## Dataset overview

The notebook's dataset contains **120 records and 24 original columns**, covering **6 commodities**:

- Apple
- Banana
- Cauliflower
- Onion
- Potato
- Tomato

The data includes fields related to commodities, dates, harvest quantity, predicted demand, source and destination markets, transit mode, transit distance and time, transportation cost, prices, farmer payout, and spoilage.

The preprocessing section checks missing values and duplicates, handles missing numerical and categorical values if present, converts the date field, and saves a cleaned CSV file.

## Technologies and libraries

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Excel / CSV for dataset input and output

## Methodology

### Part 1 – Data loading and preprocessing

1. Import the required Python libraries.
2. Upload the Excel or CSV dataset.
3. Inspect the first records, dimensions, columns, data types, and descriptive statistics.
4. Check missing values and duplicate records.
5. Handle missing numerical values using the median and categorical values using the mode.
6. Convert the `Date` column to a datetime format when available.
7. Export the cleaned dataset.

### Part 2 – Exploratory Data Analysis

The EDA section generates visualizations and summary statistics for:

- Traditional versus fair retail prices by commodity.
- Dataset demand estimates versus harvest quantities.
- Transportation-cost distribution and average cost by transit mode.
- Monthly average traditional retail price.
- Baseline versus optimized spoilage values.
- Correlations among numerical variables.

**Data interpretation note:** `Harvest_Quantity_KG` represents harvest quantity in this dataset. It is not treated as confirmed delivered or market supply. The dataset contains records from August 2026 only, so it is not sufficient to establish seasonal trends.

### Part 3 – Machine learning and supply-chain analysis

A **Random Forest Regressor** is trained using selected available input features. The target field is:

`Predicted_Demand_KG`

The data is split into training and testing sets, with 80% used for training and 20% for testing. The notebook reports:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² score

The section also compares traditional and fair retail prices, calculates row-wise consumer savings, analyzes transportation costs by mode, compares spoilage values, and summarizes farmer fair payout.

**Important modeling limitation:** `Predicted_Demand_KG` is already an estimated-demand field in the supplied dataset. Therefore, this model learns to estimate that existing dataset field; it does not demonstrate forecasting against independently verified actual future demand. The reported metrics should be interpreted in that context.

### Part 4 – Final dashboard and report

The final section consolidates the notebook's results into a performance summary and exports:

- Final analysis dataset (CSV)
- Dashboard summary (CSV)
- Text project report (TXT)

## Results captured in the executed notebook

The following values are from the saved notebook outputs. If the notebook is rerun with a different dataset or different code, results may change.

| Indicator | Recorded result |
|---|---:|
| Dataset records | 120 |
| Commodities | 6 |
| Average traditional retail price | ₹88.10/kg |
| Average fair retail price | ₹58.19/kg |
| Average row-wise consumer savings | 32.65% |
| Average baseline spoilage | 2.14% |
| Average optimized spoilage | 0.97% |
| Spoilage difference | 1.17 percentage points |
| Average transportation cost | ₹3.60/kg |
| Average farmer fair payout | ₹34.52/kg |

### Random Forest results

| Metric | Recorded result |
|---|---:|
| MAE | 193.55 |
| MSE | 54,894.83 |
| RMSE | 234.30 |
| R² | 0.5807 |

These are the outputs saved in the uploaded notebook execution, not guaranteed results for every run.

## How to run the project

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `AgrifairIBM_Project.ipynb`.
3. Run the notebook cells in order: Part 1, Part 2, Part 3, and Part 4.
4. When prompted in Part 1, upload the agricultural supply-chain Excel or CSV dataset.
5. Allow each section to finish before running the next one.
6. Download the generated CSV and TXT outputs from the Colab session when prompted.

## Limitations and future improvements

- The dataset contains 120 records; a larger and more diverse dataset would be needed for stronger generalization.
- The target is an existing demand estimate, not independently verified actual demand.
- More historical dates are needed for meaningful seasonal analysis and time-series forecasting.
- Harvest quantity should not be interpreted as confirmed market supply without additional distribution or delivery data.
- The fair-price and optimized-spoilage fields are supplied in the dataset and are compared in this project; the notebook does not independently derive an optimization solution for them.
- Future work could use verified historical demand, delivered-supply records, a broader date range, and a separately validated optimization method.

## Project conclusion

This project demonstrates a Python-based workflow for preprocessing agricultural supply-chain data, exploring pricing and logistics patterns, training a Random Forest regression model on the dataset's demand-estimate field, and presenting key indicators in a final summary. It provides an initial analytical view of farmer, consumer, transportation, and spoilage-related measures while identifying the data requirements for more reliable forecasting and optimization in future work.
