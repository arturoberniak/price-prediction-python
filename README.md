# Real Estate Price Prediction

This project presents a complete data science workflow for predicting residential property prices based on selected apartment and building parameters. The solution demonstrates practical use of modern data exploration and machine learning techniques in real estate analytics.

## Project Overview

- **Task:** Predict the price of a property (in thousands PLN) from features provided in a dataset.
- **Approach:** Data analysis, preprocessing, exploration, modeling, and evaluation in Python using open libraries.
- **Key method:** Random Forest Regressor for robust price estimation and feature importance ranking.
- **End goal:** Transparent, reproducible, and interpretable property pricing workflow.

## Features Used

- `area_m2` - Apartment area in square meters  
- `distance_to_center_km` - Distance to city center (km)  
- `floor` - Apartment floor  
- `building_age_years` - Age of the building (years)  
- `high_standard` - High finishing standard (0 = no, 1 = yes)

## Workflow

1. **Data Loading:**  
   Reads data from `housing_prices.csv`  
2. **Exploratory Data Analysis:**  
   - First look at distributions and summary statistics  
   - Detection of missing values/outliers  
   - Correlation analysis  
3. **Feature Engineering and Preprocessing:**  
   - Handling missing values (median imputation)  
   - Numeric scaling (standardization)  
   - No categorical encoding required (`high_standard` is binary)
4. **Visualization:**  
   - Distribution histograms  
   - Scatterplots of features vs price  
   - Correlation heatmap  
   - Standard impact on price (boxplot, bar)  
5. **Modeling:**  
   - Random Forest Regressor (100 estimators, max_depth=10)  
   - Training and testing set split (80/20)
6. **Evaluation:**  
   - Metrics: RMSE, MAE, R², MAPE  
   - Residuals and error analysis  
   - Feature importance plot
7. **Reporting:**    
   - Includes all major results, plots, and business recommendations

## How to Run

1. Place `housing_prices.csv` in the project directory.
2. Install dependencies:
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Run the main script in a Jupyter Notebook or as a Python script.

## Results

- **Accurate price predictions** on test data (checked via error metrics).
- **Key drivers of price** are transparently ranked.
- **Robustness** through cross-validated ensemble approach.

## Recommendations

- Extend with more advanced models (XGBoost, LightGBM, CatBoost).
- Add additional geographic and neighborhood features for even higher accuracy.
- Monitor temporal trends for agiler price modeling.

## License

Distributed under the MIT License. See `LICENSE` for details.

---
**Date:** January 2026
