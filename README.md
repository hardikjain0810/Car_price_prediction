<h2>🚗 Used Car Price Prediction</h2>
This project focuses on predicting the selling price of used cars in the Indian market using various machine learning regression techniques. The model leverages data scraped from CarDekho.com to provide accurate price suggestions to sellers based on current market conditions.

<h2>📌 Problem Statement</h2>
Determining the fair market value of a used car is challenging due to numerous influencing factors like brand, age, fuel type, and mileage. This project builds a predictive engine that:
<ul>
<li>Helps users estimate the resale value of their vehicles.</li>

<li>Provides sellers with data-driven price suggestions.</li>

<li>Analyzes the impact of features like vehicle_age, km_driven, and max_power on pricing.</li>
</ul>

<h2>🛠️ Tech Stack</h2>
<ul>
<li>Language: Python</li>

<li>Libraries: Pandas, NumPy, Scikit-learn, XGBoost</li>

<li>Visualization: Matplotlib, Seaborn, Plotly</li>
</ul>

<h2>🚀 Final Results (After Hyperparameter Tuning)</h2>
After performing a RandomizedSearchCV to find the best parameters, the models were retrained with the following results:

<b>Random Forest Regressor (Best Model)</b>
<ul>
<li>Test R2 Score: 0.9405</li>

<li>Test Root Mean Squared Error (RMSE): 211,600.5275</li>

<li>Test Mean Absolute Error (MAE): 97,275.5594</li>

<li>Best Parameters: n_estimators: 200, max_depth: 15, max_features: 8, min_samples_split: 2.</li>
</ul>

<b>XGBoost Regressor</b>
<li>Test R2 Score: 0.8550</li>

<li>Test RMSE: 330,411.0813</li>

<li>Test MAE: 103,493.6172</li>

<li>Best Parameters: n_estimators: 300, max_depth: 5, learning_rate: 0.1, colsample_bytree: 0.5.</li>

Conclusion: The Random Forest Regressor is the superior model for this specific dataset, providing the highest accuracy for predicting used car prices.



<h2>📝 Future Improvements</h2>
<ul><li>Implement a web interface using Streamlit for real-time user predictions.<li>
<li>Incorporate more granular data like "City" or "Owner Type" to improve local accuracy.</li>
  <li>Experiment with Stacking Regressors to combine the strengths of XGBoost and Random Forest.</li>
</ul>
