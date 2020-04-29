# Predicting Rainfall in Australia

## Group Members
* Hanumasri Bollepalli
* Madhuri Pawle
* Pavanitha Jampala

## Research Question

Exploratory data analysis will be used to visualize imporant trends in the data. EDA will also provide input into the need for feature pre-processing such as dimensionality reduction, null handling and feature scaling. The pre-processed data (pertinent features) will be used to analyze the research question: Will it rain tomorrow?

## Source & Domain

* Domain: Weather forecasting. Precisely to predict whether it will rain tomorrow or not?

* Source: Kaggle, https://www.kaggle.com/jsphyg/weather-dataset-rattle-package

## About the Dataset

* This dataset contains about 10 years of daily weather observations from numerous Australian weather stations.

* It consists of 24 columns and 142193 rows. It has numerical, categorical and boolean data.

* It is an unbalanced dataset, as the target column RainTomorrow has 110316 "No" entries and 31877 "Yes" entries.

* The columns that effect the RainTomorrow column the most are Humidity3pm and Cloud3pm. 

## Target Audience

The target audience would be the general public of respective areas in Australia. The dataset consists of 49 locations so people living in those 49 locations can have the benifit of knowing if it will rain the next day or not and plan their day accordingly.

## Data Preprocessing

The data cleaning steps that we are going to follow are :
* Make sure the datatypes are correct.
* Drop the columns that have less than 60% of data.
* Drop rows that consist of missing values in any of the columns.
* Handle outlier using top-coding approach.
* Encode Categorical data using One Hot Encoding as Logistic Regression cannot handle categorical data.

## Tentative Plan

* Load Data onto BigQuery
* Exploratory Data Analysis and Data Preprocessing using AI Platform
* Dashboard for User group, Dashboard for Data Engineers
* Apply Logistic Regression Model on the dataset.
* Evaluation of Results using confusion matrix, precision, recall and f1-score
* Steps for production model
* Final Dashboard for User Group
