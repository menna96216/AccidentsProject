# AccidentsProject
 
## Description

This project predicts accident severity using three 2018 UK road datasets: **Accidents**, **Casualties**, and **Vehicles**. The datasets were merged, cleaned, and preprocessed to handle missing values, outliers, and categorical encoding. The project explores data visualization, feature engineering, and applies multiple machine learning models to predict accident severity.

---

## Datasets

* **Accidents_2018.csv** – Road accident details
* **Casualties_2018.csv** – Casualty information
* **Vehicles_2018.csv** – Vehicle details involved in accidents

**Target:** `Accident_Severity`
Values: 1, 2, 3 (from least to most severe)

---

## Data Processing

* Merged the 3 datasets into one main dataframe
* Handled missing values using **KNNImputer** and **IterativeImputer**
* Removed or capped outliers using **np.clip**, **IQR**, and **boxplots**
* Categorical features encoded using **LabelEncoder**
* Date and time features extracted and processed

---

Data Visualization

Explored feature distributions using histograms, boxplots, and bar charts

Investigated relationships between features and Accident_Severity using scatter plots, correlation heatmaps, and count plots

Visualized outliers and trends to aid preprocessing and feature engineering

---

## Models Used

* Logistic Regression
* GaussianNB / BernoulliNB
* SVC / KNN
* Decision Tree / Random Forest / ExtraTrees
* Bagging / AdaBoost / GradientBoosting / HistGradientBoosting
* XGBoost / CatBoost / LightGBM

**Evaluation Metrics:**

* Accuracy, Precision, Recall, F1-score
* Confusion Matrix
* ROC Curve (One-vs-Rest)
