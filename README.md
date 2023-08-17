**Project Name - Retail Sales Prediction**
#

![WhatsApp Image 2023-08-15 at 09 58 49](https://github.com/MansiKaushik123/Retail_Sales_Prediction/assets/140509411/b3da392b-c617-494b-9f9a-772771393429)

**Problem Statement:-**

Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school, and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. You are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set. Note that some stores in the dataset were temporarily closed for refurbishment.

**Data Overview:-**
**Rossmann Srores Data.csv---Historical data including Revenue**

**store.csv - supplemental information about the store**

*Data fields Most of the fields are self-explanatory. The following are clarifications for those that aren't.*

**Id** - an identifier that represents a (Store, Date) pair within the test set.

**store**-- a distinct Identifier for each store.

**Sales** - the revenue for any given day (this is what you are forecasting)

**Customers** - the count of customers on a given day.

**Open** - Open - an indicator for whether the store was open: 0 = closed, 1 = open StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None

**SchoolHoliday**- signifies if the (Store, Date) was impacted by the closure of public schools

**StoreType** - distinguishes between 4 different store models: a, b, c, d

**Assortment** - characterizes an assortment level: a = basic, b = extra, c = extended

**CompetitionDistance** - the distance in meters to the nearest competitor store

**CompetitionOpenSince[Month/Year]** - provides the approximate year and month of the time the nearest competitor was opened

**Promo** - indicates whether a store is running a promotion on that day

**Promo2** - Promo2 is an ongoing and successive promotion for some stores: 0 = store is not involved, 1 = store is involved

**Promo2Since[Year/Week]** - specifies the year and calendar week when the store commenced participating in Promo2

**PromoInterval** - outlines the successive intervals Promo2 is initiated, listing the months the promotion begins again. For example, "Feb, May, Aug, Nov" means each cycle starts in February, May, August, and November of any given year for that store.

**Approach:-**
EDA and Feature Selection

Removed Multicollinearity.

Feature Selection.

Splitting Dataset into train and test set.

Model Training.

Model Evaluation.


**Conclusion:-**
Write the conclusion here.

1. We found that there were 172,817 rows with zero sales in the Sales column. To improve our model, we made a new dataset by excluding these zero sales rows. Using various techniques, we trained the model and achieved around 74% accuracy.

2. We were interested in the entire dataset, even the rows with zero sales. So, we trained another model using different methods and achieved an accuracy of about 98%, which is much better than the previous model.

3. This led us to conclude that removing rows with zero sales actually removes a lot of valuable information from the dataset, as it comprises a significant number of rows (172,817). Therefore, we decided to keep those values. Our best Root Mean Squared Percentage Error (RMPSE) score came from the Random Forest model and Gradient Boosting techniques like AdaBoost and XGBoost. We took care to choose optimal parameters to prevent overfitting in our model.

 ![238556309-0830854b-6f64-40f7-ac3c-eec15583b041](https://github.com/MansiKaushik123/Retail_Sales_Prediction/assets/140509411/f4b7a678-26b1-4386-81b0-19e8aebcffc3)


   
