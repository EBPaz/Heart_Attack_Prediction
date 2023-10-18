# Heart Attack Risk Prediction
Group Project 4 - Eva Pazdera, Adam Salinas, Tracy Tachick, Peter Xiong

# About
Can you determine the likelihood of a heart attack?  
Heart attacks are a major health problem in the United States as well as globally.  If medical professionals could better predict an individual’s risk for a heart attack, we could potentially decrease the number of occurrences. There are seemingly main factors that could contribute to a person’s risk for a heart attack. This project aims at using these factors to create a machine learning model that can accurately predict a patient’s risk of heart attack.

This project utilizes machine learning to create a model for assessing future heart attack risk. The dataset comes from Kaggle.com and includes 24 different variables that could contribute to heart attack risk. This is a synthetic dataset that was made via an algorithm. This data mimics real world data without violating any HIPPA laws. The dataset was also critiqued with tableau and visualizations were created to gain insight into individual risk factors. 

# Getting Started / Installation
Most of our work was done in Jupyter Notebook files with the exception of big data machine learning models which were created in Google Colab

Pre-Processing:  
Import pandas as pd
From pathlib import Path

Machine Learning Models (various versions, not all used on the same notebook):
KNearFull
KNearestNeighbors
NeuralNet
RandomForest
Logistic Regression
NeuralNet
KerasTuner

Specific imports can be found at the beginning of each notebook related to the above machine learning model.

# Analysis
During pre-processing we eliminated the columns “Patient ID” and “BMI” as variables we did not deem important to the dataset. We then split our data into 2 different dataframes. One included all variables a person had control over and the other included all variables a person did not have control over.  

The controlled variable dataframe had a blood pressure column that was categorized from typical blood pressure readings to 4 categorical labels. The uncontrolled variable dataframe had an Age column that was binned from 73 distinct ages to 10 ranges of ages.  

The data in each model test was then scaled and encoded. Some of the datasets were adjusted with undersampling models to account for the imbalance of the data. We then ran various machine learning models with each individual dataframe as well as the overall dataframe for potential risk prediction.  

The full dataset was then taken to Tableau to visualize any unique characteristics and to look for trends in the variables.  

# Summary
After many machine learning trials with different models and hyperperameter adjustments, our most accurate model was only 66% for no risk of a heart attack predictions. This came from a random forest model run on the top 7 variables in the dataset. 

The most consistent variable indicating a risk in heart attack was smoking. Other than that, none of the variables stood out as highly important compared to others. 

# References
Our synthetic dataset came from Kaggle at
https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset 
