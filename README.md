# Medical Insurance Charges Data Analysis and Prediction

This repository contains a Jupyter notebook that performs both exploratory data analysis (EDA) and predictive modeling on a dataset of medical insurance charges. The goal is to understand the factors affecting insurance charges and build a predictive model to estimate the charges based on those factors.

## Project Overview

The notebook is divided into the following key sections:

1. **Loading the Data**:
   - The dataset contains information about medical insurance charges and associated features such as age, sex, BMI, number of children, smoking status, and region.

2. **Data Cleaning**:
   - Handling missing values (if any) and converting categorical variables (sex, smoker, region) into numerical form using one-hot encoding or label encoding.

3. **Exploratory Data Analysis (EDA)**:
   - **Box plots**: To visualize the distribution of charges across categories like sex, smoking status, region, and number of children.
   - **Correlation analysis**: To identify relationships between continuous variables like age, BMI, and insurance charges.
   - **Statistical summaries**: To compute summary statistics for insurance charges across various groups.

4. **Modeling**:
   - Several machine learning models are implemented to predict medical insurance charges based on the available features:
     - **Linear Regression**: A baseline model to predict charges using all the features.
     - **Ridge Regression**: A regularized linear model to handle potential overfitting by applying L2 regularization.
     - **Random Forest Regression**: A powerful ensemble model that captures non-linear relationships between the features and the target variable.

5. **Model Evaluation**:
   - The models are evaluated based on common regression metrics:
     - **Mean Absolute Error (MAE)**
     - **Mean Squared Error (MSE)**
     - **R² Score**
   - Comparison of model performances to choose the best model for predicting insurance charges.

## Key Visualizations

- **Box plots** comparing insurance charges across various categories (sex, smoker, region, number of children).
- **Correlation heatmaps** and **pair plots** for continuous variables like age, BMI, and charges.
- **Feature importance** from the Random Forest model to understand which features contribute most to predicting charges.

## Results & Insights

- **Smokers** have significantly higher medical insurance charges compared to non-smokers.
- **Age** and **BMI** are positively correlated with charges, meaning older individuals and those with higher BMIs incur more costs.
- The **Linear Regression** and **Ridge Regression** models performed well, but the **Random Forest** model provided the most accurate predictions due to its ability to capture non-linear relationships.

## Conclusion

This project not only provides insights into the factors influencing medical insurance charges but also demonstrates the use of machine learning models to predict those charges. The most significant factors influencing the charges are smoking status, age, and BMI. The Random Forest model performed the best in terms of predictive accuracy.
