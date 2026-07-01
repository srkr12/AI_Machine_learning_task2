# Titanic Dataset - Exploratory Data Analysis (EDA)

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on the Titanic dataset. The aim is to understand the data by using summary statistics and different visualizations. Through this analysis, I explored the dataset to identify patterns, trends, relationships, and outliers that could be useful before building any Machine Learning model.

---

## Tools Used

* Python
* Pandas
* Matplotlib
* Seaborn

---

## Dataset

The project uses the Titanic dataset, which contains information about passengers such as age, gender, passenger class, ticket fare, and survival status.

---

## Tasks Performed

* Loaded and explored the dataset.
* Generated summary statistics using Pandas.
* Created histograms to understand the distribution of numerical features.
* Created boxplots to detect outliers.
* Generated count plots for categorical features.
* Created a correlation heatmap to study relationships between numerical features.
* Used a pairplot to visualize relationships among selected features.
* Analyzed the visualizations to identify patterns, trends, and anomalies in the dataset.

---

## Key Observations

* Most passengers were young adults.
* The majority of passengers traveled in Third Class.
* Most passengers paid relatively low fares, while a few paid very high fares.
* The Fare column contains several outliers.
* Passenger Class and Fare show a noticeable relationship.
* The dataset provides useful insights into passenger characteristics and survival-related features.

---

## Project Structure

```text
Task_two_dataset_analysis/
│
├── Task_two.ipynb
├── titanic.csv
├── README.md
└── images/
    ├── age_boxplot.png
    └── fare_boxplot.png
    └── age_histogram.png
    └── fare_histogram.png
    ├── correlation_matrix.png
    └── countplot_pclass.png
    └── countplot_sex.png
    └── parch_histogram.png
    └── countplot_survived.png
    └── pairplot_on_survived.png
    └── sibsp_histogram.png
```

---

## Conclusion

This project helped me understand how Exploratory Data Analysis is used to examine a dataset before applying Machine Learning algorithms. By using statistics and visualizations, I was able to better understand the data, identify important patterns, and detect outliers that may affect model performance.
