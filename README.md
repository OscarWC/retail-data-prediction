# Retail Data Prediction

A short project on predicting sales units for individual products using a machine learning model. The dataset is from a seasonal retailer which contains information on sales, inventory, orders and prices. See summary of project below.

•	I combined exploratory data analysis (EDA) with feature engineering, using heatmaps and various plots to identify key features from the dataset and generate new ones.

•	Lagged sales and inventory data emerged as the most promising features for model training. I assumed that these features would be available during real-time predictions, avoiding any risk of data leakage.

•	As a baseline model, I implemented Ridge Regression, which achieved an R² score of 0.6971 on the test data.

•	To improve performance, I employed XGBoost Regressor with parameter tuning. This model outperformed Ridge Regression, achieving an R² score of 0.7597 on the test data as well as lower mean squared error and mean absolute error, and was selected as the best-performing model.

•	I plotted the results for individual products and observed that the model performed slightly worse for extreme sales values, likely due to their infrequency in the training dataset. Residual analysis showed no noticeable skew or patterns, suggesting no major issues with the model.

•	Given more time, I would explore additional feature engineering, including creating features for promotion history of products and temporal factors to capture seasonality and trends. I would also perform more advanced hyperparameter tuning for the XGBoost Regressor and experiment with deep learning methods, such as recurrent neural networks (RNNs). Furthermore, I would produce additional final prediction plots, including date-based analyses, to further evaluate the results. I would also conduct in-depth error analysis on the results to identify specific areas where the model struggles and implement targeted improvements.
