# Smart Agricultural Supply Chain – Agrifair IBM Project

An AI and data analytics-based project focused on improving agricultural supply-chain understanding through demand estimation, price analysis, transportation cost analysis, and spoilage comparison.

## Project Overview

The Smart Agricultural Supply Chain project aims to analyze agricultural supply-chain data and identify insights that can benefit farmers, consumers, and transportation management.

The project uses Python, Exploratory Data Analysis (EDA), and a Random Forest Regression model to analyze different agricultural supply-chain parameters.

## Objectives

- Analyze agricultural commodity prices.
- Compare estimated demand with harvest quantities.
- Study transportation costs across different transport modes.
- Compare traditional and fair retail prices.
- Analyze baseline and optimized agricultural spoilage.
- Apply machine learning for demand estimation.
- Generate a final project performance dashboard.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Random Forest Regressor

## Dataset Information

The dataset contains 120 records and 24 original columns, covering six agricultural commodities:

- Apple
- Banana
- Cauliflower
- Onion
- Potato
- Tomato

It includes information related to harvest quantity, predicted demand, transportation, commodity prices, farmer payouts, and spoilage.

## Project Implementation

### Part 1: Data Loading and Preprocessing

- Imported required Python libraries.
- Uploaded and loaded the Excel dataset.
- Inspected dataset structure and statistical information.
- Checked missing values and duplicate records.
- Handled missing values.
- Converted the date column.
- Exported the cleaned dataset.

### Part 2: Exploratory Data Analysis (EDA)

Performed analysis using statistical summaries and visualizations:

- Commodity-wise price comparison.
- Predicted demand vs harvest quantity.
- Transportation cost distribution.
- Transportation cost by transit mode.
- Monthly price analysis.
- Baseline vs optimized spoilage.
- Correlation heatmap.

### Part 3: Machine Learning and Analysis

Implemented a Random Forest Regressor for demand estimation.

The model uses selected agricultural and transportation-related features.

Model evaluation metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

Additional analysis includes consumer savings, fair retail pricing, transportation costs, farmer payouts, and spoilage comparisons.

### Part 4: Final Dashboard and Reporting

Generated a final project summary containing:

- Total records and commodities.
- Average demand estimate and harvest quantity.
- Machine learning performance.
- Traditional vs fair retail prices.
- Consumer savings.
- Transportation cost.
- Spoilage comparison.
- Farmer fair payout.

Final CSV datasets and a text project report are also generated.

## Key Results

| Performance Indicator | Result |
|---|---:|
| Total Records | 120 |
| Total Commodities | 6 |
| Traditional Retail Price | ₹88.10/kg |
| Fair Retail Price | ₹58.19/kg |
| Consumer Savings | 32.65% |
| Baseline Spoilage | 2.14% |
| Optimized Spoilage | 0.97% |
| Spoilage Reduction | 1.17 percentage points |
| Average Transportation Cost | ₹3.60/kg |
| Farmer Fair Payout | ₹34.52/kg |

### Random Forest Model Performance

| Metric | Result |
|---|---:|
| MAE | 193.55 |
| MSE | 54,894.83 |
| RMSE | 234.30 |
| R² Score | 0.5807 |

*These are the saved results from the executed notebook.*

## Output Visualizations

The project includes visualizations for:

1. Commodity-wise price analysis.
2. Demand and harvest comparison.
3. Transportation cost analysis.
4. Random Forest prediction comparison.
5. Consumer savings distribution.
6. Spoilage comparison.
7. Correlation analysis.
8. Final dashboard.

See the `screenshots` folder for output graphs.

## Output
<img width="1089" height="590" alt="01_commodity_price_comparison" src="https://github.com/user-attachments/assets/01c99e51-3b9c-41f4-88b8-0306328fc9f4" />
<img width="989" height="590" alt="02_demand_vs_harvest" src="https://github.com/user-attachments/assets/57035075-7c30-450c-b81d-3306abdc250b" />
<img width="889" height="490" alt="03_transport_cost_distribution" src="https://github.com/user-attachments/assets/32949edf-899c-432d-912b-417f56a7ea3a" />
<img width="889" height="490" alt="04_transport_cost_by_mode" src="https://github.com/user-attachments/assets/4fda0b73-d9ac-4a65-b377-19c8135d8ed4" />
<img width="789" height="490" alt="05_spoilage_comparison" src="https://github.com/user-attachments/assets/2bf47287-67c9-43d8-a427-b6c3bf9bd8b2" />
<img width="1375" height="989" alt="06_correlation_heatmap" src="https://github.com/user-attachments/assets/a767a918-604c-42bd-8d3f-ab6622e2b4d8" />
<img width="889" height="590" alt="07_random_forest_prediction_comparison" src="https://github.com/user-attachments/assets/1b1584b6-2498-4e34-a938-19b6e50cd8e8" />
<img width="889" height="590" alt="07_random_forest_prediction_comparison" src="https://github.com/user-attachments/assets/04c106a6-e744-4eb3-8ed7-e2c26021cffc" />
<img width="790" height="490" alt="08_traditional_vs_fair_price" src="https://github.com/user-attachments/assets/22db0684-9439-42ee-ae06-02e4c2f36948" />
<img width="789" height="490" alt="09_consumer_savings_distribution" src="https://github.com/user-attachments/assets/6e40e367-c8ab-4b71-9e14-fe1ea843bd03" />
<img width="889" height="490" alt="10_transport_cost_comparison" src="https://github.com/user-attachments/assets/640e6ad1-c1d1-4f59-ad24-94fc237b352c" />
<img width="789" height="490" alt="11_baseline_vs_optimized_spoilage" src="https://github.com/user-attachments/assets/058abc68-6c67-4e97-bbe7-5327f8936ffd" />
<img width="790" height="490" alt="12_farmer_payout_distribution" src="https://github.com/user-attachments/assets/88fd18dd-5ddc-4780-b071-c02b113c4299" />
<img width="889" height="490" alt="13_commodity_distribution" src="https://github.com/user-attachments/assets/e0e7c80f-c4f8-4de5-97b1-307a912d5bb1" />
<img width="690" height="490" alt="14_final_demand_vs_harvest" src="https://github.com/user-attachments/assets/668742ec-9f1c-4527-b9fc-b00ed515e2a0" />
<img width="889" height="490" alt="15_final_ml_estimates" src="https://github.com/user-attachments/assets/ee4e3e1d-3536-422c-8b5e-162635e72158" />
<img width="790" height="490" alt="16_final_price_comparison" src="https://github.com/user-attachments/assets/27915718-f072-43a5-8051-19127dba002c" />
<img width="889" height="490" alt="17_final_transport_comparison" src="https://github.com/user-attachments/assets/8a4142a3-d4ca-40e7-b068-79ec0ea63f85" />
<img width="789" height="490" alt="18_final_spoilage_comparison" src="https://github.com/user-attachments/assets/5137630f-89e1-40c7-a49e-8b0c95ef7a36" />
<img width="1296" height="889" alt="19_final_correlation_heatmap" src="https://github.com/user-attachments/assets/385da825-0833-4d17-9b29-9ac6957782c9" />


## How to Run the Project

1. Download or clone this repository.
2. Open Google Colab.
3. Upload `AgrifairIBM_Project.ipynb`.
4. Run the notebook cells sequentially.
5. Upload the agricultural dataset when prompted.
6. View the generated graphs, model evaluation results, and dashboard.
7. Download the final CSV and TXT files.

## Limitations

- The dataset contains 120 records and requires larger-scale validation.
- The model predicts the existing `Predicted_Demand_KG` dataset field rather than independently verified future demand.
- Only August 2026 records are available, limiting seasonal analysis.
- Harvest quantity is not necessarily equivalent to confirmed market supply.
- Fair retail prices and optimized spoilage are existing dataset values used for comparison, not outputs of a newly developed optimization algorithm.

## Future Scope

- Integrate larger real-world agricultural datasets.
- Use verified historical demand for future demand forecasting.
- Develop an independent price optimization algorithm.
- Incorporate real-time transportation information.
- Explore cloud-based agricultural supply-chain monitoring.
- Develop an interactive web dashboard for farmers and stakeholders.

## Conclusion

The Smart Agricultural Supply Chain project demonstrates how data analytics and machine learning can be applied to understand agricultural supply-chain operations.

Through data preprocessing, exploratory analysis, Random Forest demand estimation, and dashboard reporting, the project provides insights into commodity pricing, transportation expenses, farmer payouts, consumer savings, and agricultural spoilage.

The project establishes a foundation for further development of intelligent and data-driven agricultural supply-chain solutions.
