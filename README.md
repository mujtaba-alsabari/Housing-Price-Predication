# Housing-Price-Predication
Housing Price Predication Using Linear_Reg and Other models
Housing Price Prediction – Conclusion
Model Comparison

Linear Regression with log(price) performed the best overall:

Lowest MAE and RMSE

Highest R² (~0.69, explaining ~70% of variance)

Lowest MAPE (~15%), meaning predictions are on average within 15% of the true price

Random Forest models underperformed:

R² stuck around 0.49–0.52

Larger errors (MAE > 820K, MAPE > 17%)

XGBoost showed moderate performance:

Better than Random Forest but still weaker than Linear Regression

R² ~0.53 (no log) and ~0.52 (with log)

Key Insights

Log-transforming the target price improves model performance for both Linear Regression and Random Forest.

Linear Regression is surprisingly strong: simple, interpretable, and effective for this dataset.

Tree-based models (RF, XGB) may require deeper hyperparameter tuning or more data to outperform LR.

Feature importance (from correlation and scatterplots):

Area has the strongest positive correlation with price.

Features like bathrooms, stories, air conditioning, and prefarea also push prices upward.

Categorical features such as mainroad access and guestroom availability show clear price differences in boxplots.
