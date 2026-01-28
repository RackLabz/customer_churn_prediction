# customer_churn_prediction

# Customer Churn Prediction Using Machine Learning

Customer churn is one of the most costly problems faced by subscription-based businesses. Retaining an existing customer is often significantly cheaper than acquiring a new one, making early churn detection a high-impact use case for machine learning.

This project applies **applied machine learning** techniques to predict customer churn and, more importantly, to understand *why* customers leave. The emphasis is not just on predictive accuracy, but on building a **robust, reproducible, and interpretable end-to-end data science pipeline** that reflects real-world practice.

---

## Project Objective

The main goals of this project are to:

- Predict whether a customer is likely to churn using supervised machine learning  
- Compare multiple classification models under a **fair and consistent evaluation framework**  
- Translate model outputs into **actionable business insights** that can support retention strategies  

---

## Dataset Overview

The dataset consists of customer demographic information, account details, and service usage patterns, alongside a binary churn indicator.

Key characteristics of the data include:

- A mix of numerical and categorical features  
- **Class imbalance**, with fewer churned customers relative to retained ones  
- Realistic noise and feature correlations commonly observed in business datasets  

These properties make the dataset well-suited for demonstrating applied machine learning challenges.

---

## Workflow Summary

### 1. Data Inspection & Preprocessing

- Inspected dataset structure, missing values, and target distribution  
- Implemented preprocessing using **scikit-learn Pipelines** and **ColumnTransformer**  
- Ensured all transformations were fit exclusively on training data to prevent data leakage  

---

### 2. Exploratory Data Analysis (EDA)

- Examined feature distributions and relationships  
- Analyzed correlations and churn patterns  
- Identified early signals and variables associated with increased churn risk  

---

### 3. Model Training & Evaluation

Multiple classification models were trained using identical preprocessing pipelines to ensure an unbiased comparison.

Key decisions included:

- Selecting **ROC-AUC** as the primary evaluation metric due to class imbalance  
- Evaluating all models on unseen test data  
- Using comparative performance to guide final model selection  

---

### 4. Threshold Optimization

- Predicted probabilities were used instead of fixed class labels  
- Decision thresholds were tuned to balance recall and precision  
- Business cost considerations were incorporated, with particular attention to the cost of missing high-risk churn customers  

---

### 5. Model Interpretation

- Feature importance analysis was conducted  
- Key drivers of customer churn were identified  
- Model results were translated into clear, business-friendly insights  

---

## Key Findings

- The selected model demonstrated strong discriminatory power in separating churned and retained customers  
- Several service usage and account-related features emerged as strong predictors of churn  
- Threshold tuning significantly improved the model’s ability to identify high-risk customers  

---

## Business Value

The resulting model can support:

- Proactive churn prevention strategies  
- Targeted customer retention and engagement campaigns  
- Data-driven decision-making for customer management teams  

---

## Limitations & Future Work

While the model performs well, several limitations remain:

- External behavioral and market-level factors were not included  
- Customer behavior was modeled as static rather than time-dependent  

Potential future improvements include:

- Cost-sensitive learning approaches  
- Time-based or sequential churn modeling  
- Validation using real-time or external datasets  

---

## Tools & Technologies

- Python  
- pandas, NumPy  
- scikit-learn  
- matplotlib, seaborn  
- Jupyter Notebook  

---

## Author

**Ugwuoke Shedrack Chinonso**  
