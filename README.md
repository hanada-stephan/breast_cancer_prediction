# Breast cancer prediction: Project overview

- This notebook is part of learning the first steps on Kaggle guided project on Coursera, "Breast Cancer Prediction Using Machine Learning" by Priya Jha ([Link](https://www.coursera.org/projects/breast-cancer-prediction-using-machine-learning)). 
- Created a model that diagnoses breast cancer. 
- Performed features scaling.
- Label encoded target variable.

## Code and resources

Platform: Google Colab

Python version: 3.7.6

Packages: itertools, os, matplotlib, pandas, numpy, seaborn and sklearn

## Data set

**Data set URL: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data**

## Data cleaning

There was one column, "Unnamed: 32", to drop which all the values were null. Also, since the target variable was categorical, it needed to be converted into numerical as 0 for non-malignant and 1 for malignant.

## Model building

First, I performed feature scaling to avoid model bias. Then, I split the data into train and test sets with a test size of 25% and no need for a stratified shuffle due to the balanced target variable.

I tried only one model, the logistic regression, that performed well, and there was no need to try other algorithms.

## Model performance

The logistic regression had an accuracy of 0.97 with only five false negatives.

