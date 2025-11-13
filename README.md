# House-Price-Prediction-ML
A Machine Learning project for predicting house prices using advanced feature engineering and multiple regression models such as Linear Regression, Ridge, Lasso, Gradient Boosting, and XGBoost. Includes EDA, outlier analysis, lag/rolling features, synthetic external features, model comparison, and prediction visualization.
🏡 House Price Prediction using Machine Learning

This project builds a complete end-to-end Machine Learning pipeline to predict house prices using advanced regression techniques, feature engineering, and performance evaluation.

📌 Project Highlights

✔ Dataset with 21,607 rows
✔ EDA + Outlier Detection
✔ Advanced Feature Engineering
✔ Lag Features, Rolling Features
✔ Structure Index & Property Quality Index
✔ Synthetic external features (crime rate, malls, hospitals, metro stations)
✔ Linear + Tree-based Model Comparison
✔ XGBoost selected as best-performing model
✔ SHAP Explainability
✔ User Input Prediction Function

📁 Project Structure
project/
│
├── data/
│   └── Raw_Housing_Prices2.csv
│
├── notebook/
│   └── HousePricePrediction.ipynb
│
├── images/
│   ├── heatmap.png
│   ├── boxplots.png
│   ├── fit_chart.png
│   └── shap_summary.png
│
├── README.md
├── requirements.txt

🛠 Feature Engineering Summary
🔹 Rolling Window Features (per zipcode)

rolling_price5_zip

rolling_max5_zip

rolling_min5_zip

rolling_std5_zip

🔹 Lag Feature

lag_price_zip

🔹 Indices

Structure_Index

Property_Quality_Index

🔹 Synthetic External Features

crime_rate_index

no_of_malls

no_of_hospitals

no_of_metro_stations

📊 Modeling Approach
✔ Linear Models (with StandardScaler)

Linear Regression

Ridge Regression

Lasso Regression

✔ Tree Models (without scaling)

Gradient Boosting Regressor

XGBoost Regressor

🏆 Model Performance Summary
Scaled Linear Models
Model	R²	RMSE	MAE
Linear Regression	0.795	112k	83k
Ridge Regression	0.795	112k	83k
Lasso Regression	0.795	112k	83k
Tree Models
Model	R²	RMSE	MAE
🌟 XGBoost Regressor	0.883	85k	60k
Gradient Boosting	0.881	86k	60k

✔ Best Model → XGBoost (non-linear patterns capture karta hai)

📈 Visualizations Included

Distribution Plots

Scatter: Area vs Price

Boxplots for Outliers

Correlation Heatmap

Actual vs Predicted Fit Charts

SHAP Feature Importance

🎯 How to Run

Clone repo

git clone https://github.com/your-username/House-Price-Prediction-ML.git


Install requirements

pip install -r requirements.txt


Run Jupyter

jupyter notebook


Open HousePricePrediction.ipynb

Run all steps sequentially

🧪 Prediction Function

User can input:

Bedrooms / Bathrooms

Area

Zipcode

Renovation year

Structure Index

Quality Index

Engineered Features

Model returns predicted house price in rupees.

⭐ Conclusion

The project demonstrates that powerful feature engineering combined with ensemble models like XGBoost significantly improves model accuracy. Extensive EDA, synthesized locality features, and SHAP explainability make this model robust and highly interpretable.
