# Electricity Demand Forecasting Using Machine Learning and Time Series Models

## Project Overview

Accurate electricity demand forecasting is essential for maintaining a stable and efficient power grid. Reliable forecasts help utility companies optimize electricity generation, improve resource planning, reduce operational costs, and ensure a consistent supply of power.

This project develops an end-to-end electricity demand forecasting pipeline using both machine learning and traditional time series forecasting techniques. The workflow includes data preprocessing, exploratory data analysis, feature engineering, model development, performance evaluation, and model comparison to determine the most effective forecasting approach.

## Objectives

The primary objectives of this project are to:

- Analyse historical electricity demand data.
- Explore patterns and trends through exploratory data analysis.
- Engineer meaningful time-based and lag features.
- Build and evaluate multiple forecasting models.
- Compare machine learning and statistical forecasting techniques.
- Identify the most accurate model for electricity demand prediction.

## Dataset

**Dataset:** AEP Hourly Electricity Consumption

**Target Variable:** AEP_MW (Hourly Electricity Demand)

**Data Type:** Time Series

The dataset contains more than 120,000 hourly electricity demand observations collected over several years, making it suitable for developing and evaluating forecasting models.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Statsmodels
- Prophet

## Project Workflow

1. Data Loading
2. Data Inspection
3. Data Cleaning
4. Exploratory Data Analysis (EDA)
5. Feature Engineering
6. Train-Test Split
7. Baseline Forecasting
8. Random Forest
9. Feature Importance Analysis
10. Residual Analysis
11. XGBoost
12. ARIMA
13. SARIMA
14. Prophet
15. Model Evaluation & Performance Comparison
16. Final Conclusion

## Forecasting Models

The following forecasting approaches were implemented and compared:

- Baseline Model(Linear Regression)
- Random Forest Regressor
- XGBoost Regressor
- ARIMA
- SARIMA
- Prophet

## Model Performance

Model | Summary |
Random Forest | Best overall performance |
XGBoost | Very close to Random Forest |
Baseline | Strong benchmark model |
Prophet | Successfully modelled trend and seasonality but struggled with short-term fluctuations |
ARIMA | Lower predictive accuracy |
SARIMA | Lowest performance on this dataset |

## Best Performing Model

Among all the forecasting models, **Random Forest** achieved the highest predictive performance. It produced the lowest prediction error and the highest R² score while effectively capturing the nonlinear relationships and temporal dependencies within the electricity demand data.

Although XGBoost delivered very similar results, Random Forest slightly outperformed it on this dataset, demonstrating that the best-performing model depends on the characteristics of the data rather than the complexity of the algorithm.

## Evaluation Metrics

The forecasting models were evaluated using:

- Mean Absolute Error (MAE)
- R^2 Score

These metrics were used to compare prediction accuracy and determine the overall performance of each forecasting approach.

## Visualizations

This project includes several visualizations to better understand the data and model performance, including:

- Exploratory Data Analysis
- Correlation Heatmap
- Feature Importance
- Actual vs Predicted Values
- Residual Analysis
- Model Performance Comparison

## Future Improvements

There are several opportunities to extend this project in the future:

- Develop Deep Learning models such as LSTM and GRU.
- Explore Transformer-based forecasting models.
- Perform hyperparameter optimisation using Optuna.
- Incorporate weather and holiday information as additional features.
- Build a real-time forecasting pipeline.
- Deploy the model using Streamlit or FastAPI.

## Conclusion

This project compared six different forecasting approaches, including a Baseline model, Random Forest, XGBoost, ARIMA, SARIMA, and Prophet.

Among all the models, **Random Forest achieved the best overall performance**, producing the lowest prediction error and the highest R^2 score. XGBoost followed closely behind, demonstrating that tree-based ensemble methods are highly effective for forecasting electricity demand when combined with appropriate feature engineering.

Traditional statistical models such as ARIMA and SARIMA were able to capture temporal relationships but were less effective than the machine learning approaches for this dataset. Prophet successfully modelled the overall trend and seasonality; however, it struggled to predict short-term fluctuations with the same level of accuracy as Random Forest and XGBoost.

Feature importance analysis showed that lag-based features, particularly **lag_1**, had the greatest influence on the model's predictions, highlighting the strong temporal dependency present in electricity demand forecasting.

Overall, this project demonstrates the value of combining feature engineering with ensemble machine learning techniques for accurate electricity demand forecasting and reinforces the importance of selecting forecasting models based on the characteristics of the data rather than assumptions about a model's general performance.

## Key Skills Demonstrated

- Time Series Forecasting
- Machine Learning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Model Evaluation
- Ensemble Learning
- Python Programming
- Data Visualization

## Author

**Kishore Krishna Moorthy**

**Master of Data Science**  
**The University of Western Australia**

GitHub: https://github.com/kishorekrishna-ds
