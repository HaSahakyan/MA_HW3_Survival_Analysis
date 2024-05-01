# Telecom Customer Churn Analysis

This repository contains code and a report for a homework assignment on survival analysis and customer churn prediction in a telecom dataset. The analysis includes building parametric survival models, comparing their performance, and calculating Customer Lifetime Value (CLV) per customer based on the final model. Additionally, valuable customer segments are identified, and suggestions for retention strategies are provided.

## Contents

- **Code and Report**: Jupyter notebook containing Python code for data preprocessing, model fitting, CLV calculation, and visualization. Included report summarizing the findings of the analysis, including interpretations of coefficients, identification of valuable segments, annual retention budget estimation, and retention strategy suggestions.
- **Dataset**: telco.csv file containing the data for the CLV analysis.
- **Requirements.txt**: File listing the required Python packages for running the code.
- **Readme.md**: This file, providing a brief introduction to the repository.

## Introduction

The goal of this analysis is to understand the factors influencing customer churn in a telecom dataset. By building survival models and calculating CLV, we aim to identify valuable customer segments and propose effective retention strategies to minimize churn.

## How to Use

1. Clone the repository to your local machine.
2. Ensure you have Python installed along with the necessary packages listed in `requirements.txt`.
3. Open the Jupyter notebook (`Telecom_Customer_Churn_Analysis.ipynb`) to view and run the code.
4. Read the report (`Report.md`) to understand the findings and recommendations.

## About the Dataset

The dataset contains various attributes of telecom subscribers, including region, tenure, age, marital status, income, education level, and customer category. The target variable is churn, indicating whether a customer has churned or not.

## Findings and Conclusions

- Survival analysis using parametric models (Weibull, Exponential, Log-Normal, and Log-Logistic distributions) showed that the Log-Normal distribution had the lowest AIC and BIC values, indicating the best fit for the data.
- The AFT (Accelerated Failure Time) versions of the models confirmed that the Log-Normal distribution performed the best among the AFT models as well.
- Significant features influencing churn risk include tenure at the same address, age, customer category (especially E-service, Plus service, and Total service), internet service, marital status, and voice service.
- Valuable customer segments identified include those with Plus and E-Service subscriptions, married customers, and those without voice services.
- The CLV analysis revealed varying CLV distributions among different customer categories, highlighting the importance of targeted retention strategies.
- The estimated annual retention budget, based on survival probabilities and a threshold of 0.8, is $41000.
- Proposed retention strategies include personalized communication, loyalty programs, proactive customer service, and predictive analytics to foresee and prevent churn.
