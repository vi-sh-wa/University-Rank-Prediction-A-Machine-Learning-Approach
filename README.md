# University Rank Prediction: A Machine Learning Approach

## Project Overview
This project demonstrates the application of data analysis and machine learning to predict the **overall score** of universities worldwide. By analyzing key factors such as research, citations, and international outlook, this model provides insights that help university authorities, prospective students, and government bodies understand the mechanics of global academic rankings.

[For indepth analysis of the Project, Click Here](https://vi-sh-wa.github.io/University-Rank-Prediction-A-Machine-Learning-Approach/project.html)

## Key Features
* **Predictive Modeling**: Utilizes regression techniques to forecast university scores based on 17 distinct variables.
* **Comprehensive Preprocessing**: Features advanced data cleaning including type casting, unit conversion, and custom feature engineering (e.g., extracting the number of subjects offered).
* **Robust Imputation**: Handles missing data using **CART (Classification and Regression Trees)**, which was found to preserve the original data distribution better than other methods.
* **Target Encoding**: Efficiently manages high-cardinality categorical data (e.g., 127 unique university locations) to avoid dimensionality issues.

## Methodology & Workflow
The project follows a rigorous data science pipeline to ensure model reliability and prevent data leakage:

1.  **Data Cleaning**: Converting numerical variables read as characters and handling special characters in scores.
2.  **Feature Selection**: Filtering out uninformative features with near-zero variance.
3.  **Exploratory Data Analysis (EDA)**: Conducting univariate, bivariate, and multivariate analyses to detect trends and outliers.
4.  **Normalization**: Scaling data to a range of [0, 1] to improve computation speed and model performance.
5.  **Model Training**: Comparing multiple algorithms including **Robust Linear Regression (RLM)**, **Support Vector Machines (SVM)**, and **Random Forest (RF)**.

## 🏆 Results
* **Top Performing Model**: **Random Forest** achieved the best metrics after fine-tuning, significantly reducing computation time while maintaining high accuracy.
* **Predictive Accuracy**: The final model achieved an **RMSE of 0.03** and explained **98.05%** of the variability in the data.
* **Key Drivers**: Analysis revealed that **research and citation scores** are the most influential factors in determining a university’s overall rank.

## 🛠 Tools & Libraries Used
* **Language**: R
* **Core Packages**: 
    * `caret`: For data partitioning, feature selection, and model training.
    * `mice`: For advanced data imputation (CART).
    * `ggstatsplot`: For correlation analysis (`ggcorrmat`).
    * `base R`: For data type conversion and manipulation.

---
