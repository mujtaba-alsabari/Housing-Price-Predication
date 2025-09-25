# Housing-Price-Predication
Housing Price Predication Using Linear_Reg and Other models
This project builds and compares machine learning models to predict housing prices based on features such as area, bedrooms, bathrooms, stories, parking, and categorical attributes like mainroad access, guestroom, and furnishing status.

We evaluate multiple regression techniques and explore how log-transforming the target price impacts performance.

Dataset

The dataset includes the following key features:

Numerical Features:

area, bedrooms, bathrooms, stories, parking

Categorical Features:

mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, furnishingstatus

Target Variable:

price

Models Trained

Linear Regression

With and without log(price)

Random Forest Regressor

With and without log(price)

XGBoost Regressor

With and without log(price)

Best Model: Linear Regression with log(price)

R² ~ 0.69

MAE ~ 672K

Predictions within ~15% error on average

Exploratory Data Analysis (EDA)

Correlation analysis shows area has the strongest positive correlation with price.

Scatter plots with trend lines reveal linear relationships between area, bathrooms, stories, and price.

Boxplots indicate higher prices for houses with:

Access to mainroad

Guestroom

Air conditioning

Located in preferred areas

Conclusion & Recommendation

Linear Regression with log-transformed price is the recommended deployment model.

It outperforms Random Forest and XGBoost on this dataset, balancing accuracy, interpretability, and efficiency.

Tree-based models may improve with hyperparameter tuning, but LR currently provides the most reliable results.
