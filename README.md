# Integrated Retail Analytics for Store Optimization & Demand Forecasting

**Author:** Allan Cheerakunnil Alex  
**Project Type:** Machine Learning Capstone (Regression, Clustering, Association)

## Project Overview
In the highly competitive retail sector, optimizing store performance and accurately predicting demand is critical for preventing stockouts and reducing holding costs. This project transitions raw, multi-department retail data into an automated, data-driven strategy engine using a multi-faceted Machine Learning pipeline.

The core objectives achieved in this project include:
1. **Demand Forecasting:** Predicting weekly store and department sales with high accuracy.
2. **Store Segmentation:** Grouping physical stores into actionable performance tiers.
3. **Market Basket Inference:** Identifying cross-selling opportunities across departments without relying on individual customer receipt data.

## Tech Stack & Methodology
* **Language:** Python
* **Data Processing & Feature Engineering:** Pandas, NumPy (Zero-imputation for sparse markdowns, datetime extraction).
* **Anomaly Detection:** Scikit-Learn (`IsolationForest`) to remove extreme, corrupted sales spikes.
* **Predictive Modeling:** Scikit-Learn (`RandomForestRegressor`) for non-linear time-series forecasting.
* **Clustering:** Scikit-Learn (`KMeans`) validated via Silhouette Score.
* **Statistical Analysis:** Pearson Correlation matrix for market basket inference; Welch's T-Test for hypothesis validation.

## Key Results & Business Impact
* **Forecasting Accuracy:** The Random Forest Regressor achieved an **R-Squared of 0.978** and an RMSE of $2,756, proving that physical store capacity and baseline department history are the strongest predictors of future sales.
* **Data-Driven Segmentation:** Stores were segmented into High, Medium, and Low-volume tiers (Silhouette Score: 0.58), allowing executives to replace "one-size-fits-all" budgets with targeted, tier-specific operational strategies.
* **Macroeconomic Resilience:** Statistical testing proved that the retail business is highly resilient; rising regional unemployment and fuel prices did not significantly negatively impact baseline weekly sales.

## Repository Structure
* `Integrated_Retail_Analytics_Main.ipynb`: The complete, fully documented machine learning pipeline and exploratory data analysis.
* `retail_rf_model.joblib`: The serialized, production-ready Random Forest forecasting model.
* `Presentation.pptx`: The executive slide deck summarizing business challenges, methodologies, and strategic recommendations.

## Strategic Recommendations
1. **Tier 1 Inventory Automation:** Deploy automated, aggressive restocking pipelines exclusively for Tier 1 (High-Volume) stores to maximize Q4 throughput.
2. **Joint Promotional Marketing:** Bundle highly correlated departments (e.g., Dept 33 & 24) for joint promotional MarkDowns based on the Market Basket analysis.
3. **Targeted Economic Adaptation:** While the business is recession-resistant, heavy promotional markdowns should be targeted specifically at smaller (Tier 3) stores during periods of peak inflation to maintain baseline foot traffic.
