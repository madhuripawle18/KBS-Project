# Predicting Rainfall in Australia

# Group Members
* Hanumasri Bollepalli
* Madhuri Pawle
* Pavanitha Jampala

# Research Question

Exploratory data analysis will be used to visualize imporant trends in the data. EDA will also provide input into the need for feature pre-processing such as dimensionality reduction, null handling and feature scaling. The pre-processed data (pertinent features) will be used to analyze the research question: Will it rain tomorrow?

# Source & Domain

* Domain: Weather forecasting. Precisely to predict whether it will rain tomorrow or not?

* Source: Kaggle, https://www.kaggle.com/jsphyg/weather-dataset-rattle-package

# About the Dataset

* This dataset contains about 10 years of daily weather observations from numerous Australian weather stations.

* It consists of 24 columns and 142193 rows. It has numerical, categorical and boolean data.

* It is an unbalanced dataset, as the target column RainTomorrow has 110316 "No" entries and 31877 "Yes" entries.

* The columns that effect the RainTomorrow column the most are Humidity3pm and Cloud3pm. 

# Target Audience

The target audience would be the general public of respective areas in Australia. The dataset consists of 49 locations so people living in those 49 locations can have the benifit of knowing if it will rain the next day or not and plan their day accordingly.

# Data Preprocessing

The data cleaning steps that we are going to follow are :
* Make sure the datatypes are correct.
* Drop the columns that have less than 60% of data.
* Drop rows that consist of missing values in any of the columns.
* Handle outlier using top-coding approach.
* Encode Categorical data using One Hot Encoding as Logistic Regression cannot handle categorical data.

# Tentative Plan

## Load data onto BigQuery
After observing the column in the dataset and their importance in order to predict if it will rain tomorrow or not, we have to do the data prre processing and cleaning the data. Selecting the features from dataset that effect the model. 
## Exploratory Data Analysis and Data Preprocessing using AI Platform
This part of the project will involve visualizing the dataset based on different features from the dataset.Creating graphs that analyze the importance of the columns.Distribution graph inferes observation on different locations according to the dataset. 
## Dashboard for User group, Dashboard for Data Engineers
Dashboard for user consists of basic graph that depicts rain fall prediction by yes or no. The aim is to convey simple imformation from correlated features to get the target variable.Dashboard for Data Engineers helps them predict the correlation between the features that affected the target result and understand the database.
## Apply Logistic Regression Model on the dataset.
Creating Logistic Regression model and running the model on the dataset help to predict the output variable with high accuracy.
## Evaluation of results using confusion matrix, precision, recall and f1-score
## Steps for production model
The dataset will be read using BigQuery, then for every record, model prediction will be carried out, and the results are written back to BigQuery.
## Final Dashboard for User Group
The final dashboard will consist of predicted data in form of a graph and it will depict the results of the model.

![Image of user_dashboard.png](https://github.com/hanumasribollepalli/KBS-Project/blob/master/user%20dashboard.png)

![Image of Heatmap.png](https://github.com/hanumasribollepalli/KBS-Project/blob/master/Heatmap.png)

![Image of Pairplot.png](https://github.com/hanumasribollepalli/KBS-Project/blob/master/Pairplot.png)

![Image of Boxplot_to_detect_Outliers.png](https://github.com/hanumasribollepalli/KBS-Project/blob/master/Boxplot%20to%20detect%20Outliers.png)


# References

* S. Navadia, P. Yadav, J. Thomas and S. Shaikh, "Weather prediction: A novel approach for measuring and analyzing weather data," 2017 International Conference on I-SMAC (IoT in Social, Mobile, Analytics and Cloud) (I-SMAC), Palladam, 2017, pp. 414-417.

* A. Omary, A. Wedyan, A. Zghoul, A. Banihani and I. Alsmadi, "An interactive predictive system for weather forecasting," 2012 International Conference on Computer, Information and Telecommunication Systems (CITS), Amman, 2012, pp. 1-4.

* P. C. Reddy and A. S. Babu, "Survey on weather prediction using big data analystics," 2017 Second International Conference on Electrical, Computer and Communication Technologies (ICECCT), Coimbatore, 2017, pp. 1-6.
