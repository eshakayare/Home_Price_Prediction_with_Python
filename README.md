# Home_Price_Prediction_with_Python

Home Price Prediction using Regression Analysis in Python

📌 Project Overview
This project explores predictive modeling techniques to estimate the median house value in California neighborhoods using census block group data. The focus is on identifying the most influential factors and selecting the best regression model for accurate, reliable predictions. The outcome offers powerful tools for real estate analysis, urban planning, and financial decision-making.

💼 Business Question
"How can we accurately predict the median house value in California neighborhoods using census block group data, and which factors most influence these predictions?"

🎯 Objectives
* Predict median house values using regression models.

* Identify key predictors influencing housing prices.

* Compare model performance to select the best approach.

* Derive actionable business and economic insights from the analysis.

📊 Dataset Overview
* Total Observations: 20,640

* Target Variable: median_house_value

* Independent Variables: longitude, latitude, housing_median_age, total_rooms, total_bedrooms, population, households, median_income, ocean_proximity

* Missing Values: total_bedrooms: 207 rows dropped (<1% of data)

* Categorical Variable: ocean_proximity encoded using dummy variables (excluding 'ISLAND' due to low frequency)

🧪 Methodology
* Exploratory Data Analysis (EDA) : Univariate and bivariate analysis, log transformations for skewed variables, outlier removal using IQR, and correlation checks.

* Feature Engineering

-- Dropped multicollinear features (total_bedrooms, households)

-- Removed spatial features (latitude, longitude)

* Model Evaluation Metrics:

-- Mean Squared Error (MSE)

-- Mean Absolute Error (MAE)

-- Root Mean Squared Error (RMSE)

-- R-squared (R²)

🤖 Regression Models Applied
Model	 R² (Train) 	R² (Test)  	Notes
Linear Regression	~0.54	~0.54	Simple, interpretable, good generalization
Decision Tree	High	~0.20	Overfits, poor test performance
Support Vector Regression (SVR)	Low	Low	High error, consistent across sets
Random Forest	~0.84	~0.50	Strong train fit, weaker test generalization
Tuned Random Forest	~0.66	~0.55	Balanced performance
Gradient Boosting	~0.63	~0.54	Generalizes well, robust to overfitting
Voting Regressor	Moderate	~0.55	Best overall performance
🏆 Best Performing Models
Linear Regression (for interpretability and stability)

Voting Regressor (for balanced and robust performance)

💡 Business Implications
* Pricing Strategy: Optimize listing and valuation accuracy

* Market Segmentation: Identify high-value neighborhoods

* Lending Insights: Improve mortgage risk assessment

* Urban Planning: Allocate resources based on housing trends
