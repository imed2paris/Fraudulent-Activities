# Fraudulent activities


## Topic

* In e-commerce, one of the main tasks is fraud detection.
* Most of the time, fraudulent purchases are discovered too late: it would be very useful to recognize the common characteristics of fraudulent activities and to block them before the end of the purchasing process.
* In this project, we will rely on a sample of transactions made in 2015 on an anonymous website.


## Objective

* We are faced with a classification problem where supervised learning algorithms will try to identify fraudulent activities.
* The aim is to build a model that minimises Type II error so that as few fraudulent transactions as possible pass through.
* To carry out this task, we have a dataset containing more than 150 000 transactions from an anonymous website that sells handmade clothing worldwide.


## Issues

* The dataset does not mention the country from which the customer placed the order: to solve this problem, we will use an auxiliary dataset that gives the lower and upper limits of IP addresses for each country.
* No specific provision has been made for the fact that the data is very unbalanced.
* In the Data Understanding files, there is a description of each field in both datasets, and a detailed explanation of each step in the join process.
* In the "Data preparation" file, we specify the steps of aggregation, dummyfication, partition and normalisation of the data.
* We use boosting algorithms in the modeling and evaluation phase: as with other models, we have to take into account the imbalance of the data by modifying the hyperparameters.


## Technologies

* I use python packages in this project: 
    * Pandas for data wrangling, 
    * Seaborn and Matplotlib for data visualisation, 
    * Scikit-learn for modeling.
* A specific python package, xgboost, is used to implement a boosting algorithm.