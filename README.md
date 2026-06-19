# ❤️ Heart Disease Risk Analysis using Python

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on a heart disease dataset to uncover patterns and relationships between patient health indicators and the presence of heart disease. Using Python, the dataset is cleaned, explored, and visualized to understand how factors such as age, sex, cholesterol, blood pressure, and chest pain type relate to heart disease outcomes.

---

## 🎯 Objectives

* Load and inspect the structure of the heart disease dataset.
* Clean the data by checking for missing values and removing duplicates.
* Explore patient demographics (age, sex) and their distribution.
* Analyze how individual health indicators relate to heart disease.
* Visualize relationships using count plots, histograms, box plots, and a correlation heatmap.
* Identify which features are most strongly correlated with heart disease.

---

## 📊 Dataset Information

The dataset (`Heart-disease.csv`) contains 303 unique patient records (after removing duplicates) with the following features:

| Feature  | Description                              |
| -------- | ----------------------------------------- |
| age      | Age of the patient                       |
| sex      | Gender of the patient (1 = male, 0 = female) |
| cp       | Chest pain type                          |
| trestbps | Resting blood pressure                   |
| chol     | Serum cholesterol level                  |
| fbs      | Fasting blood sugar                      |
| restecg  | Resting ECG results                      |
| thalach  | Maximum heart rate achieved              |
| exang    | Exercise-induced angina                  |
| oldpeak  | ST depression induced by exercise        |
| slope    | Slope of peak exercise ST segment        |
| ca       | Number of major vessels colored          |
| thal     | Thalassemia status                       |
| target   | Heart disease presence (0 = No, 1 = Yes) |

---

## 🛠️ Tech Stack

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🔍 Analysis Performed

### Data Understanding & Cleaning

* Dataset overview (`info()`, `head()`, `tail()`, `shape`, `columns`, `describe()`)
* Missing value check
* Duplicate record detection and removal
* Data type inspection

### Univariate Analysis

* Heart disease distribution (count plot)
* Age distribution (histogram)
* Gender value counts

### Bivariate Analysis

* Gender vs. heart disease
* Cholesterol vs. heart disease (box plot)
* Fasting blood sugar vs. heart disease (line plot)
* Resting blood pressure vs. heart disease (box plot)

### Correlation Analysis

* Full correlation matrix across all numeric features
* Correlation heatmap visualization

---

## 📈 Visualizations

All plots generated in the notebook are saved to the `images/` folder:

* `number of patients_distribution.png` — Heart disease distribution
* `age_distribution.png` — Age distribution of patients
* `Gender Vs Patients.png` — Gender vs. heart disease
* `cholestrol_Analysis.png` — Cholesterol levels vs. heart disease
* `Blood_Sugar distribution.png` — Fasting blood sugar vs. heart disease
* `Blood pressure_distribution.png` — Resting blood pressure vs. heart disease
* `HeatMap_distribution.png` — Correlation heatmap of all features

---

## 💡 Key Insights

* After removing duplicates, the dataset contains 303 patient records, with 206 male and 96 female patients.
* Chest pain type (`cp`) and maximum heart rate (`thalach`) show the strongest **positive** correlation with heart disease.
* Exercise-induced angina (`exang`), ST depression (`oldpeak`), and number of major vessels (`ca`) show the strongest **negative** correlation with heart disease.
* Age and sex show weaker, but still notable, negative correlations with heart disease presence in this dataset.
* The correlation heatmap helps highlight which clinical features are most worth focusing on for further analysis or modeling.

---

## 🚀 Future Enhancements

* Build a Machine Learning model (e.g., Logistic Regression, Random Forest) to predict heart disease presence.
* Perform feature scaling and encoding for ML readiness.
* Evaluate model performance using accuracy, precision, recall, and confusion matrix.
* Explore feature importance to confirm insights from the correlation analysis.

---

## 📚 Learning Outcomes

Through this project, practical experience was gained in:

* Data cleaning and preprocessing with Pandas
* Exploratory Data Analysis (EDA)
* Data visualization with Matplotlib and Seaborn
* Correlation analysis and heatmap interpretation
* Drawing healthcare insights from real-world tabular data
