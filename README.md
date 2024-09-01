# Customer Churn Analysis and Predictive Modeling

## Overview

This project addresses the challenge of customer churn in the telecommunications industry. By analyzing customer data and developing predictive models, the goal is to identify customers at high risk of churn and implement proactive retention strategies. This repository contains code and documentation related to the exploratory data analysis (EDA), machine learning models, and business recommendations.

## Project Structure

- **data/**: Contains raw and processed datasets.
- **notebooks/**: Jupyter notebooks for EDA, data cleaning, and model development.
- **README.md**: This file.

## Data Description

The primary dataset used for this project is the Telco Customer Churn dataset, which includes various customer attributes and churn information. Key variables include:

- `customerID`: Unique identifier for each customer.
- `gender`: Gender of the customer.
- `SeniorCitizen`: Indicates if the customer is a senior citizen.
- `Partner`: Indicates if the customer has a partner.
- `Dependents`: Indicates if the customer has dependents.
- `tenure`: Number of months the customer has stayed with the company.
- `PhoneService`: Indicates if the customer has a phone service.
- `MultipleLines`: Indicates if the customer has multiple lines.
- `InternetService`: Type of internet service the customer has.
- `OnlineSecurity`: Indicates if the customer has online security.
- `OnlineBackup`: Indicates if the customer has online backup.
- `DeviceProtection`: Indicates if the customer has device protection.
- `TechSupport`: Indicates if the customer has tech support.
- `StreamingTV`: Indicates if the customer has streaming TV.
- `StreamingMovies`: Indicates if the customer has streaming movies.
- `Contract`: Type of contract the customer has.
- `PaperlessBilling`: Indicates if the customer is using paperless billing.
- `PaymentMethod`: Payment method used by the customer.
- `MonthlyCharges`: The amount charged to the customer monthly.
- `TotalCharges`: The total amount charged to the customer.
- `Churn`: Indicates if the customer has churned.

## Analysis

### Exploratory Data Analysis (EDA)

The EDA focuses on understanding feature distributions and identifying key patterns:

- **Churn Predictors**: High monthly and total charges are associated with higher churn rates. Shorter tenures also correlate with increased churn.
- **Contract Type Impact**: Month-to-month contracts are linked to higher churn rates compared to longer-term contracts.
- **Service Features**: Fiber optic internet users and customers with phone service exhibit higher churn rates.
- **Data Characteristics**: The dataset shows right-skewed distributions for charges and class imbalance in churn rates.

### Machine Learning Models

Several models are evaluated to predict customer churn:

- **Random Forest**: The top-performing model, balancing precision and recall effectively.
- **Decision Tree**: Strong recall but slightly lower precision compared to Random Forest.
- **XGBoost**: Effective but slightly less performant compared to Random Forest and Decision Tree.

**Model Tuning**: Hyperparameter tuning improved the Random Forest model's accuracy, precision, and recall, making it more reliable for predicting churn.

**Evaluation Metrics**: Models demonstrate high performance with strong discrimination between churned and non-churned customers.

## Business Recommendations

Based on the analysis and model insights, the following recommendations are made:

- **Target High-Risk Customers**: Focus on customers with high charges, short tenures, and month-to-month contracts.
- **Enhance Contract Appeal**: Improve the attractiveness of longer-term contracts to reduce churn.
- **Address Service Features**: Improve the experience of customers with fiber optic internet and phone service.
- **Optimize Resource Allocation**: Use model insights to design personalized retention strategies.

## License

This project is licensed under the [MIT License].

## Contact

For any questions or suggestions, please contact [Altamash Ajaz](mailto:altamashajaz0606@gmail.com).
