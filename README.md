# Predicting Rainfall in Australia

## Group Members
* Hanumasri Bollepalli
* Madhuri Pawle
* Pavanitha Jampala

## Research Question

The main aim of the project will be to predict if it will rain or not. There are 24 columns in the dataset, we will pre-process the data and visualize the data to find out how each column like pressure, temperarure, humidity etc effects the target column "RainTomorrow".

## Source & Domain

* Domain: Weather forecasting. Precisely to predict whether it will rain tomorrow or not?

* Source: Kaggle, https://www.kaggle.com/jsphyg/weather-dataset-rattle-package

* We stored the data on BigQuery in Google Cloud Platform.

## Target Audience

The target audience would be the general public of respective areas in Australia. The dataset consists of 49 locations so people living in those 49 locations can have the benifit of knowing if it will rain the next day or not and plan their day accordingly.

## Data Preprocessing

The data cleaning steps that we are going to follow are :
* Make sure the datatypes are correct.
* Replace missing numerical values with Median of the column.
* Handle outlier using top-coding approach.
* Replace missing categorical data with the most frequent label.
* Encode Categorical data using One Hot Encoding as Logistic Regression cannot handle categorical data.

## Tentative Plan

* Exploratory Data Analysis and Preprocessing
* Dashboard for User group, Dashboard for Data Engineers
* GCP further processing - ML
* Evaluation of results
* Steps for production model
* Final Dashboard for User Group
