# Titanic Dataset - Data Cleaning & Preprocessing

## Overview

This project demonstrates the complete process of cleaning and preprocessing the Titanic dataset before using it for Machine Learning. Raw datasets often contain missing values, categorical data, inconsistent formats, and outliers that need to be handled to improve the quality of the data. The goal of this project is to prepare the dataset so that it can be used effectively for further analysis and predictive modeling.

---

## Objective

The main objective of this project is to learn and apply common data preprocessing techniques, including:

* Exploring and understanding the dataset
* Handling missing values
* Encoding categorical features
* Scaling numerical features
* Detecting and handling outliers
* Creating a clean dataset suitable for Machine Learning

---

## Tools and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Dataset

The project uses the classic **Titanic Dataset**, which contains information about passengers such as age, gender, passenger class, fare, cabin details, and survival status.

---

## Steps Performed

### 1. Data Exploration

The dataset was first loaded into a Pandas DataFrame. Basic exploration was performed using functions such as:

* `head()`
* `shape`
* `info()`
* `describe()`
* `isnull().sum()`

This helped in understanding the structure of the dataset, identifying data types, and locating missing values.

---

### 2. Handling Missing Values

The missing values were treated as follows:

* Missing values in the **Age** column were replaced using the **median** because it is less affected by extreme values.
* Missing values in the **Embarked** column were filled using the **mode**, which represents the most frequently occurring value.
* The **Cabin** column contained a large number of missing values, so it was removed from the dataset.

---

### 3. Encoding Categorical Features

Since Machine Learning algorithms cannot work directly with text data, categorical columns were converted into numerical values.

* The **Sex** column was encoded using **Label Encoding**.
* The **Embarked** column was converted using **One-Hot Encoding**.

---

### 4. Feature Scaling

The numerical columns **Age** and **Fare** were standardized using **StandardScaler** from Scikit-learn. Feature scaling ensures that numerical features are on a similar scale, which improves the performance of many Machine Learning algorithms.

---

### 5. Outlier Detection and Handling

Outliers were visualized using **boxplots** created with Seaborn.

The **Interquartile Range (IQR)** method was used to identify and remove outliers from the **Fare** column. Boxplots were generated before and after removing outliers to compare the results.

---

### 6. Saving the Cleaned Dataset

After completing all preprocessing steps, the cleaned dataset was saved as a new CSV file for future use in Machine Learning tasks.

---

## Project Structure

```
Task_one_dataset_processing/
│
├── Task_one.ipynb
├── titanic.csv
├── cleaned_titanic.csv
├── README.md
└── images/
    ├── boxplot_age.png
    └── boxplot_fare.png
    └── boxplot_fare_updated.png

```

---

## Results

After preprocessing:

* Missing values were successfully handled.
* Categorical features were converted into numerical format.
* Numerical features were standardized.
* Outliers in the Fare column were identified and removed.
* A clean dataset was generated for further Machine Learning applications.

---

## Conclusion

Data preprocessing is one of the most important steps in any Machine Learning workflow. Through this project, I learned how to inspect a dataset, clean missing values, transform categorical data into numerical form, scale numerical features, and identify outliers. These preprocessing techniques help improve data quality and prepare the dataset for building reliable Machine Learning models in future tasks.
