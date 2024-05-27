### **Time Forecast Prediction**
Project Description
This project involves time series forecasting using machine learning models to predict sales. The project includes data preprocessing, model training, hyperparameter tuning, and evaluation.

### **Objectives**
Understand the data: Gain insights into the store sales data, including store-specific information, product families, promotions, and sales numbers. This understanding will enable the company to make informed business decisions.

Predict store sales: Develop a reliable time series forecasting model that accurately predicts the unit sales for different product families at various Favorita stores. This will help the company optimize inventory management, plan promotions, and improve overall sales performance.

### **File Descriptions and Data Field Information**
train.csv: The training data contains time series information, including store_nbr, family, onpromotion, and the target variable sales. It provides insights into the store, product, promotion, and sales data.

test.csv: The test data has the same features as the training data. The task is to predict the target sales for the dates in this file. The dates in the test data are for the 15 days following the last date in the training data.

transaction.csv: This file includes the date, store_nbr, and the number of transactions made on each specific date.

stores.csv: This file contains store metadata, including city, state, type, and cluster. The cluster column represents the grouping of similar stores.

oil.csv: Daily oil prices, which include values during both the train and test data timeframes. Oil prices are significant because Ecuador is an oil-dependent country, and its economy is vulnerable to shocks in oil prices.

holidays_events.csv: This file provides information about holidays and events, including metadata. The "transferred" column indicates if a holiday was officially transferred to another date by the government. Additional details about different holiday types are also provided.

Additional Notes
Wages in the public sector are paid every two weeks on the 15th and the last day of the month. This information could affect supermarket sales.

An earthquake with a magnitude of 7.8 struck Ecuador on April 16, 2016. The earthquake led to relief efforts and donations, which significantly impacted supermarket sales for several weeks after

### **Methodology**
To achieve the objectives, we will follow a structured approach:

Data Exploration: Thoroughly explore the provided datasets to understand the available features, their distributions, and relationships. This step will provide initial insights into the store sales data and help identify any data quality issues.

Data Preparation: Handle missing values, perform feature engineering, and encode categorical variables as necessary. This step may involve techniques like imputation, scaling, and one-hot encoding.

Time Series Analysis: Analyze the temporal aspects of the data, including trends, seasonality, and potential outliers. This analysis will provide a deeper understanding of the underlying patterns in-store sales over time.

Model Selection and Training: Select appropriate time series forecasting models and train them using the prepared data. Consider incorporating external factors like promotions, holidays, and oil prices, if available, to enhance forecasting accuracy.

Model Evaluation: Evaluate the trained models using appropriate metrics, such as mean absolute error (MAE), root mean squared error (RMSE), or mean absolute percentage error (MAPE). Assess the models' performance and identify the most accurate and reliable forecasting model.

Model Deployment and Forecasting: Deploy the chosen model to predict store sales for future time periods, leveraging the provided test dataset. Generate forecasts for the target period and assess the model's ability to capture the sales patterns accurately.

### **Additional Notes**
Wages in the public sector are paid every two weeks on the 15th and the last day of the month. This information could affect supermarket sales.

An earthquake with a magnitude of 7.8 struck Ecuador on April 16, 2016. The earthquake led to relief efforts and donations, which significantly impacted supermarket sales for several weeks afterwards.

### **Models**
This project includes the following machine learning models:

ARIMA (AutoRegressive Integrated Moving Average)

XGBoost (Extreme Gradient Boosting)

SARIMA (Seasonal AutoRegressive Integrated Moving Average)

LightGBM (Light Gradient Boosting Machine)

Autoregression model

Linear Regression


### **Hyperparameter Tuning**
Hyperparameters for the models are tuned using GridSearchCV with time series split

### **License**
This project is licensed under the MIT License.

### **Author**
Joy Koech
