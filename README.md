# Retail_Sales_Prediction
Rossmann operates over 3,000 drug stores in 7 European countries. Rossmann store managers are currently tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school, and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. My work includes various plots and graphs, visualizations, feature engineering, ensemble techniques, and different ML algorithms with their respective parameter tuning, analysis, and trends.

The goal is to predict the Sales of a given store on a given day.

The dataset consists of two CSV files: store and Rosmann Data
Data Files:

Rosmann Data holds info about each store. store.csv holds the sales info per day for each store.
1. Business Problem. Rossmann operates over 3,000 drug stores in 7 European countries. Rossmann store managers are currently tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school, and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

2. Steps for solving the business problem:

a) Collecting Data- That will be involved upload the .csv file, and thoroughly checking the independent and dependent variables by using .head(), .info(), .describe(), etc.
b) Preparing the Data- Cleaning the data to remove unwanted data, missing values, rows, and columns, duplicate values, data type conversion, etc. Visualize the data to understand how it is structured and the relationship between independent and dependent variables. Splitting the cleaned data into two sets - a training set and a testing set. The training set teaches the model to recognize patterns and relationships in the data and optimize its parameters to minimize the error on the training set. A testing set is used to check the accuracy of the model after training.

c) Choosing and training the model. d) Hyparameter Tuning. e) Making Predictions.

Conclusion We saw that the Sales column contains 172817 rows with 0 sales. So we created a new data frame in which we removed 0 sales rows and tried to train our model. We used various algorithms and got an accuracy score of around 74%.

We were also curious about the total dataset(including Sales = 0 rows). So we trained another model using various algorithms and we got an accuracy near about 98% which is far better than the previous model.

So we came to the conclusion that removing sales=0 rows actually removes a lot of information from the dataset as it has 172817 rows which is quite large and therefore we decided not to remove those values. We got our best glimpse score from the Random Forest model, Gradient boosting techniques like adaboost, and Xgboost, we tried taking an optimum parameter so that our model doesn't overfit.
