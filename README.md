# Real Estate Price Analysis and Prediction

## Project Overview

This project focuses on analyzing real estate property data and predicting property prices using machine learning techniques. The goal of the project is to understand the key factors influencing property prices and build a predictive model that can estimate property values based on property characteristics.

The project applies the complete data science workflow including **data cleaning, exploratory data analysis (EDA), feature engineering, and machine learning modeling**.

---

## Problem Statement

Property buyers and investors often struggle to determine the fair value of a property. Property prices depend on multiple factors such as area size, furnishing condition, floor level, and price per square foot.

This project aims to analyze real estate data and build a machine learning model capable of predicting property prices based on these factors.

---

## Dataset Description

The dataset contains information about various real estate properties.

**Total Records:** 4525 properties

### Dataset Features

| Column Name    | Description                               |
| -------------- | ----------------------------------------- |
| property_name  | Name of the property                      |
| areaWithType   | Area description of the property          |
| square_feet    | Property size in square feet              |
| transaction    | Type of transaction (Resale/New Property) |
| status         | Construction status                       |
| floor          | Floor information                         |
| furnishing     | Furnishing type                           |
| facing         | Property facing direction                 |
| price_per_sqft | Price per square foot                     |
| price          | Total property price                      |

---

## Project Workflow

### 1. Data Cleaning

* Handled missing values in categorical columns.
* Removed currency symbols and text from price columns.
* Converted string values into numerical format.
* Extracted floor numbers from floor descriptions.
* Filled missing numerical values using median.

Notebook:
`notebooks/1_data_cleaning.ipynb`

---

### 2. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand relationships between variables and property prices.

Key analyses performed:

* Price distribution visualization
* Square feet vs price relationship
* Furnishing status vs price
* Correlation heatmap for numerical variables

Notebook:
`notebooks/2_eda.ipynb`

---

### 3. Feature Engineering

Categorical variables such as transaction type, furnishing, status, and facing were converted into numerical features using **One-Hot Encoding**.

Additional features such as **floor_number** were extracted for better modeling.

Notebook:
`notebooks/3_analysis.ipynb`

---

### 4. Machine Learning Model

A **Linear Regression model** was used to predict property prices based on the processed features.

Steps performed:

* Feature selection
* Train-test split (80% training, 20% testing)
* Model training
* Prediction on test dataset

---

## Model Evaluation

The model performance was evaluated using the following metrics:

* **Mean Absolute Error (MAE)**
* **Mean Squared Error (MSE)**
* **R² Score**

These metrics help measure how accurately the model predicts property prices.

---

## Key Insights

* Larger properties tend to have higher prices.
* Price per square foot strongly influences the total property price.
* Furnished properties may have slightly higher values.
* Property features can be effectively used to predict real estate prices.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Project Structure

```
real-estate-price-analysis/

data/
   raw_data.csv
   cleaned_data.csv

notebooks/
   1_data_cleaning.ipynb
   2_eda.ipynb
   3_analysis.ipynb

reports/
   executive_summary.pdf
   technical_report.pdf

presentations/
   business_presentation.pptx

README.md
```

---

## Future Improvements

Possible improvements for the project include:

* Using advanced machine learning models such as Random Forest or XGBoost
* Including location-based features
* Adding more property characteristics such as number of bedrooms and amenities
* Developing a web application for real-time property price prediction

---

## Conclusion

This project demonstrates how data science techniques can be used to analyze and predict real estate prices. Through data cleaning, exploratory analysis, and machine learning modeling, meaningful insights were obtained from the dataset and a predictive model was developed.

---

## Author

**Aishwarya Selvakumar**
Artificial Intelligence & Machine Learning Student
