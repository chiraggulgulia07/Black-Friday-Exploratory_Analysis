# Black-Friday-Exploratory_Analysis
Black Friday Sales Prediction & Customer Behavior Analysis
Project Overview
This project delves into the purchasing behavior of customers of a retail company, "ABC Private Limited," during a Black Friday sales event. The primary objective is to build a predictive model that can estimate a customer's purchase amount for various products. By understanding the key drivers of purchase behavior—such as customer demographics (gender, age, marital status) and product categories—the model aims to empower the company to create personalized offers, optimize inventory, and enhance overall sales strategy.

This notebook focuses on the critical initial stages of the machine learning pipeline: Exploratory Data Analysis (EDA), Data Cleaning, Feature Engineering, and Data Preprocessing to prepare the dataset for model training.

Key Features & Workflow
Data Cleaning & Preprocessing:

Executed robust data cleaning by merging the training and testing datasets to ensure consistent transformations.

Handled missing values in categorical features (Product_Category_2 and Product_Category_3) by employing mode imputation, a strategic choice for discrete data.

Cleaned and standardized the Stay_In_Current_City_Years column by removing special characters ('+') and converting the data type to integer for numerical analysis.

Feature Engineering:

Transformed categorical variables into numerical representations to make them suitable for machine learning models.

Applied One-Hot Encoding on the City_Category column, effectively converting nominal data into a usable format while avoiding the dummy variable trap (drop_first=True).

Implemented Manual Ordinal Encoding for the Age column and Label Encoding for Gender, preserving the inherent order and simplifying binary features.

Exploratory Data Analysis (EDA):

Utilized Seaborn and Matplotlib to create insightful visualizations, including bar plots to analyze the relationship between key demographic features (Age, Occupation, Gender) and the total purchase amount.

Uncovered a key insight from the analysis: Males demonstrated a significantly higher purchasing power compared to females across most product categories and age groups.

Feature Scaling:

Prepared the dataset for model training by separating the independent variables (X) and the target variable (y).

Applied StandardScaler from Scikit-learn to scale the features. This step standardizes the data to have a mean of 0 and a standard deviation of 1, which is crucial for the performance of many regression algorithms.

Technologies Used
Data Analysis & Manipulation: Pandas, NumPy

Data Visualization: Seaborn, Matplotlib

Machine Learning & Preprocessing: Scikit-learn (StandardScaler, train_test_split)

Project Outcome
The dataset has been successfully cleaned, transformed, and scaled, making it ready for the application of advanced regression models. This comprehensive preprocessing ensures that any subsequent model (like XGBoost, Random Forest, or Linear Regression) will be trained on a high-quality, robust dataset, leading to more accurate predictions of customer purchase amounts.
