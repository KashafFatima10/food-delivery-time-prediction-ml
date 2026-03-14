# food-delivery-time-prediction-ml
Machine Learning project for predicting food delivery time using a Kaggle dataset. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning models to analyze factors affecting delivery time.

# 🍔 Food Delivery Time Prediction using Machine Learning

## 📌 Project Overview

This project focuses on analyzing a food delivery dataset and preparing it for machine learning. The main goal is to understand the data, clean it, and perform visualization so that it can be used in later phases to build a delivery time prediction model.

This repository currently includes **Phase 1 and Phase 2** of the project.

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

## ⏳ Saving Preprocessed Dataset

To save time in future phases, the cleaned dataset was saved in **CSV format**. This allows future notebooks to load the processed dataset directly instead of repeating the entire preprocessing pipeline.

---

# 📁 Project Structure

```
food-delivery-time-prediction-ml
│
├── data pre processing & Visualization.ipynb
└── README.md
```

---

# 👩‍💻 Author

**Kashaf Fatima** Roll no: **BCSF23M522**
Course: **Machine Learning**

Machine Learning Project – Food Delivery Time Prediction

