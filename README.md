
# food-delivery-time-prediction-ml

Machine Learning project for predicting food delivery time using a Kaggle dataset. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning models to analyze factors affecting delivery time.

# 🍔 Food Delivery Time Prediction using Machine Learning

## 📌 Project Overview

This project focuses on analyzing a food delivery dataset and preparing it for machine learning. The main goal is to understand the data, clean it, and perform visualization so that it can be used in later phases to build a delivery time prediction model.

This repository currently includes **Phase 1 , Phase 2 and Phase 3** of the project.

---

# Phase 1: Dataset Selection

## 📂 Dataset

In this phase, a suitable dataset for the food delivery prediction problem was selected. The dataset contains information related to food delivery orders such as:

* Delivery person details
* Restaurant and delivery locations
* Order and pickup time
* Weather conditions
* Road traffic density
* Type of vehicle used for delivery
* City information
* Time taken to deliver the order

### 🎯 Objective of Dataset Selection

The dataset was selected because it contains multiple features that influence delivery time, allowing us to analyze how different factors affect food delivery efficiency.

The **target variable** in this dataset is:

**Time_taken(min)** – the total time required to deliver an order.

This dataset provides enough features to perform exploratory analysis and later build machine learning models.

---

# Phase 2: Data Visualization and Preprocessing

In this phase, the dataset was analyzed and prepared for machine learning. This includes cleaning the dataset, handling missing values, and understanding the distribution of different features.

---

## 📊 Data Visualization

Visualization techniques were used to better understand the dataset and identify patterns.

Some of the visualizations performed include:

* **KDE plots** to understand the distribution of delivery time.
* **Box plots** to detect outliers in numerical features.
* **Bar charts** to analyze orders across different months and days.
* **Location-based analysis** to observe order patterns across different cities.

These visualizations helped in understanding the structure of the data and identifying issues such as outliers, missing values, and invalid coordinates.

---

## 🧹 Data Preprocessing

Several preprocessing steps were performed to clean and prepare the dataset.

### Data Cleaning

* Removed unnecessary columns that were not useful for analysis.
* Extracted useful information from existing columns.

### Feature Extraction

* Extracted **city information** from the delivery person ID.
* Extracted **delivery time in minutes** from the `Time_taken(min)` column.
* Extracted **month and day** from the order date.

### Handling Missing Values

Different techniques were used to handle missing values in the dataset:

* **Random value imputation** for delivery person age.
* **Median imputation** for delivery person ratings.
* **Mode imputation** for categorical columns such as traffic density and festival information.
* Weather condition values were balanced and filled where missing.

### Handling Invalid Data

Some restaurant coordinates had values **(0,0)** which do not represent real locations. These entries were removed from the dataset.

---
# Phase 3: Feature Engineering

## 🛠 Feature Engineering

Feature engineering was performed to enhance the predictive power of the dataset:

* **City Area**: Categorized cities into urban, semi-urban, and metropolitan to capture location impact on delivery time.
* **Cluster Feature**: Created using **K-Means clustering** on scaled numerical features to represent hidden patterns in orders.
* **Standardization**: All numerical features were scaled to ensure equal importance in the model.
* **Feature Importance Analysis**: Evaluated features using multiple methods (Random Forest, LightGBM, SelectKBest, Mutual Information, Correlation) to identify the most impactful features.
* **Dropping Less Important Features**: Columns with very low importance or irrelevant to delivery time (e.g., ID) were dropped to reduce noise and improve model efficiency.

**Significance of Feature Engineering:**

* Helps models learn patterns more effectively.
* Reduces irrelevant information to improve performance.
* Generates new insights, such as identifying clusters of similar delivery orders.
* Prepares data for better accuracy in predictive modeling.

---

## ⏳ Saving Preprocessed and Feature-Engineered Dataset

The final dataset, after preprocessing and feature engineering, was saved in **CSV format**. This ensures future notebooks can load the prepared dataset directly for modeling, saving time and maintaining consistency.

# 📊 Phase-4: Methodology Implementation & Results

## ⚙️ Methodology

The following steps were implemented:

### 1. Data Collection

The dataset was collected and loaded into the notebook. It contains relevant features required for analysis and prediction.

### 2. Data Preprocessing

* Missing values were handled
* Categorical variables were encoded
* Data was cleaned and formatted
* Feature scaling was applied where necessary

### 3. Feature Engineering

* New features were created from existing data
* Irrelevant features were removed
* Important features were selected
* Data representation was improved for better learning

### 4. Exploratory Data Analysis (EDA)

* Data visualizations were created (histograms, bar charts, heatmaps)
* Relationships between variables were analyzed
* Trends, patterns, and outliers were identified

### 5. Model Training

The dataset was split into training and testing sets. The following models were trained:

* Logistic Regression
* Decision Tree
* Random Forest

### 6. Model Evaluation

Models were evaluated using:

* Accuracy Score
* Classification Report

The performance of each model was compared to identify the best one.

---

## 📈 Results

* All models were successfully trained and tested
* Random Forest (or your best model) achieved the highest accuracy
* Feature engineering and preprocessing improved model performance

---

## 🧾 Conclusion

The implemented methodology successfully achieved the project objectives. Data preprocessing, feature engineering, and EDA helped in understanding the dataset, while machine learning models provided accurate predictions.

The best-performing model can be used for future predictions and real-world applications.
---

# 📁 Project Structure

```
food-delivery-time-prediction-ml
│
├── phase 2
├── phase 3
├── phase 4
└── README
```

---

# 👩‍💻 Author

**Kashaf Fatima**
Roll no: **BCSF23M522**
Course: **Machine Learning**

Machine Learning Project – Food Delivery Time Prediction
