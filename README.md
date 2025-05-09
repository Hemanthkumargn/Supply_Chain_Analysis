
# Fraud Detection & ABC Analysis in Supply Chain Data

## Objective

The aim of this project is to develop a machine learning pipeline to detect fraudulent transactions within the supply chain domain and to classify products using ABC inventory analysis. This approach helps in mitigating financial losses and improving operational efficiency through better inventory planning and risk management.

## Dataset Overview

The dataset used consists of approximately 180,000 records from the supply chain industry. It includes key features related to transaction details, product specifications, shipping modes, costs, and revenue metrics.

## Features Used

- Transaction ID – Unique identifier for each transaction  
- Product Category – Type or classification of the product  
- Shipping Mode – Mode of transport used for delivery  
- Cost and Revenue – Financial values used for ABC classification  
- Fraudulent Flag – Binary indicator for fraud detection  
- Additional derived features used in modeling and segmentation

## Methodology

The project follows a structured analytics pipeline:

### 1. Data Preparation
- Cleaned and encoded categorical features
- Handled missing and anomalous values
- Performed normalization and feature selection

### 2. Fraud Detection Modeling
- Built classification models including:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - Naïve Bayes
- Evaluated models using accuracy, precision, recall, and F1-score
- Tuned model parameters using GridSearchCV
- Best model achieved 92% accuracy

### 3. ABC Inventory Analysis
- Ranked products based on total revenue contribution
- Classified inventory into:
  - Category A: Top 75% of revenue
  - Category B: Next 20%
  - Category C: Bottom 5%
- Identified top 6 products as most valuable for operational focus

## Summary of Findings

- The fraud detection model successfully identifies high-risk transactions, enabling organizations to take preemptive action.
- ABC analysis revealed that a small group of products (6) accounts for the majority of revenue, supporting strategic inventory control.
- The combined approach enhances both financial oversight and supply chain performance.

## Tools & Libraries

- Python  
- Pandas, NumPy – Data preprocessing and transformation  
- Matplotlib, Seaborn – Data visualization  
- Scikit-learn – Machine learning and evaluation metrics  
- GridSearchCV – Hyperparameter tuning  

## Business Value

This analytics solution enables supply chain organizations to:
- Detect and prevent fraudulent activities early
- Improve profitability through efficient resource allocation
- Strategically manage inventory based on revenue contribution
