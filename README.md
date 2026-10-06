# Titanic-Survival-Prediction-Data-Cleaning-Project

##📌 Overview
This project focuses on **Data Preprocessing and Exploratory Data Analysis (EDA)** on the classic Kaggle Titanic Dataset. The goal is to clean missing values, encode categorical columns into numerical formats, visualize distributions, and export a processed dataset ready for Machine Learning modeling.

---

## 🛠️ Assignment Objectives
1. **Exploratory Analysis**: Load data using `pandas` and inspect statistical summaries (`.info()`, `.describe()`).
2. **Data Imputation**: Handle missing values in critical columns using median and mode imputation strategy.
3. **Categorical Encoding**: Encode non-numeric variables (`Sex`, `Embarked`) using `LabelEncoder` and `OneHotEncoder` (`pd.get_dummies`).
4. **Data Visualization**: Visualize passenger age distribution using `Seaborn` and `Matplotlib`.
5. **Data Export**: Export the cleaned dataset to a new CSV file (`cleaned_titanic_dataset.csv`).

---

## 📊 Summary of Data Processing Steps

| Feature / Column | Problem | Solution Applied |
| :--- | :--- | :--- |
| **`Age`** | 177 missing values | Imputed missing values with column **Median** |
| **`Embarked`** | 2 missing values | Imputed missing values with column **Mode** (most frequent value) |
| **`Cabin`** | >75% missing values | Column dropped due to excessive missingness |
| **`Sex`** | Categorical text (`male`/`female`) | Transformed using **LabelEncoder** (`0` / `1`) |
| **`Embarked`** | Categorical ports (`C`, `Q`, `S`) | Encoded using **One-Hot Encoding** into separate binary columns |

---

## 🚀 How to Run the Project


   📁 Repository Structure
   ├── Titanic-Dataset.csv           # Raw input dataset
   ├── cleaned_titanic_dataset.csv   # Cleaned and preprocessed output dataset
   ├── Untitled.ipynb                # Jupyter notebook with complete Python analysis
   └── README.md                     # Project documentation
