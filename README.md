# Rossman Retail Sales Prediction

Rossman is a drug store that operates over 3,000 stores in European countries. The task is to forecast the "Sales" column for the test set. Two datasets are provided, Rossman Store Dataset including the Sales and Stores dataset as CSV files. We imported these two datasets in Google Colaboratory and converted them into data frames (df_sales and df_stores). Each row of the df_sales (Rossman Stores df) has attributes namely ‘Store’, ‘DayOfWeek’, ‘Date’, ‘Sales’, ‘Customers’ , ‘Open’ , ‘Promo’ , ‘Stateholiday’ , ‘SchoolHoliday’. Similarly, for df_stores (Store df) ‘Store’, ‘StoreType’, ‘Assortment’, ‘Competition Distance’, ‘Competition Open Since Month’, ‘Competition Open Since Year’, ‘Promo2’, ‘Promo2 Since Week’, ‘Promo2 Since Year’ and ‘Promo Interval’.

## Data Cleaning and Preparation
We performed various data cleaning operations such as dropping or substituting null values as per requirement, eliminating some irrelevant instances, extracting day, months, and year from the date column, and mapped some instances having similar values with different notations. We added some features to gain further insights.

## Exploratory Data Analysis (EDA)
After all the cleaning operations, we did data visualization and made some data transformations wherever required. We did Univariate Analysis, Bivariate Analysis, and Multivariate Analysis to get some insights from the dataset and made some changes in the features suitable for Feature Engineering and Modeling.

## Feature Engineering
Moving towards Feature Engineering, we did One Hot Encoding for some categorical features and treated Multicollinearity using Heatmap and Variance Inflation Factor algorithm. We then proceeded with determining the Independent variables best suited to apply to the model for predicting our dependent variable i.e., ‘Sales’ column.

## Model Building
We split the whole dataset in 70:30 ratio into Training dataset and Testing dataset and applied fit transform into the independent variables for standardization. Then we applied different Machine Learning algorithms such as Linear Regression, Lasso Regression, Ridge Regression, Decision Tree, and Random Forest and fitted our dataset into them one by one. We used Hyperparameter Tuning in Lasso Regression by using Grid Search CV and tried to determine the best Alpha value to increase the accuracy of our model. Random Forest came out to be the best model among all with the highest training (99%) and testing (97%) scores.

## Model Evaluation
We determined some evaluation metrics for each model such as Root Mean Squared Error, Mean Absolute Percentage Error, R2 Score. We also determined the feature importance as per Random Forest and predicted our Target Variable.

## Business Insight:

The sales prediction model can help Rossman in making data-driven decisions for improving their business. By accurately predicting the sales, Rossman can optimize their inventory management, staff scheduling, and promotional activities. They can identify the factors that impact their sales the most and focus on improving those areas.

## Future Scope:

The sales prediction model can be further improved by incorporating external factors like weather conditions, economic indicators, and events. This will help in making more accurate predictions as these external factors also impact the sales. Additionally, Rossman can use this model to forecast sales for new stores before opening them. They can also use this model for making predictions at a more granular level, i.e., predicting sales for individual products or categories.

In conclusion, we were able to forecast the "Sales" column for the test set of Rossman stores with high accuracy using Random Forest algorithm. The insights obtained from the EDA helped us make informed decisions during feature engineering and model building.
