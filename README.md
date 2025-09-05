# 📱 Google Play Store EDA & Feature Engineering Project

## 📌 Project Overview

This project explores the **Google Play Store dataset** to uncover insights about mobile applications. The focus is on **Exploratory Data Analysis (EDA)** and **Feature Engineering (FE)** to prepare the dataset for potential machine learning tasks such as predicting app ratings or installs.

Through data cleaning, visualization, and feature transformation, this project highlights patterns in app categories, user preferences, monetization strategies, and other factors influencing app success.

---

## 🎯 Objectives

* Perform **data cleaning** to handle missing, inconsistent, and noisy values.
* Conduct **Exploratory Data Analysis (EDA)** to extract insights.
* Engineer new **features** that can be useful for predictive modeling.
* Visualize trends in categories, installs, reviews, and ratings.
* (Optional) Build a baseline predictive model for app ratings or popularity.

---

## 📂 Dataset

The dataset is sourced from **Kaggle**: [Google Play Store Apps Dataset](https://www.kaggle.com/lava18/google-play-store-apps).

**Key Columns:**

* `App` → App name
* `Category` → App category (e.g., GAME, TOOLS, EDUCATION)
* `Rating` → Average rating (0–5)
* `Reviews` → Number of user reviews
* `Size` → App size (e.g., "19M", "Varies with device")
* `Installs` → Number of installs (e.g., "10,000+")
* `Type` → Free or Paid
* `Price` → App price (if paid)
* `Content Rating` → Age group suitability
* `Genres` → Sub-categories of apps
* `Last Updated` → Date when the app was last updated

---

## 🛠️ Project Workflow

### 1. **Data Cleaning**

* Removed duplicates and irrelevant entries.
* Handled missing values using imputation/dropping.
* Converted categorical and numeric values (e.g., `Installs`, `Size`, `Price`).
* Corrected data types for consistency.

### 2. **Exploratory Data Analysis (EDA)**

* Category-wise distribution of apps.
* Rating distribution and skewness.
* Free vs Paid app comparison.
* Popularity analysis based on installs and reviews.
* Correlation heatmaps for numerical features.

### 3. **Feature Engineering (FE)**

* Converted `Size` to MB for uniformity.
* Transformed `Installs` and `Price` to numeric.
* Extracted **year/month** from `Last Updated`.
* Created new features:

  * `Reviews_per_Install = Reviews / Installs`
  * `Revenue_Potential = Price * Installs`
  * `Days_Since_Last_Update`

### 4. **(Optional) Predictive Modeling**

* Regression → Predict app ratings.
* Classification → Predict app popularity (High vs Low installs).

---

## 📊 Visualizations & Insights

* **Top Categories**: Game, Tools, and Productivity dominate.
* **Ratings**: Most apps have ratings between 3.5–4.5.
* **Free vs Paid**: Free apps attract more downloads, while paid apps have slightly better ratings.
* **App Updates**: Recently updated apps tend to have higher ratings.

---

## 🚀 Tech Stack

* **Python**
* **Pandas / NumPy** → Data cleaning & preprocessing
* **Matplotlib / Seaborn / Plotly** → Data visualization
* **Scikit-learn** → Feature engineering & baseline ML models
* **Jupyter Notebook / Google Colab** → Development environment

---

## 📈 Future Improvements

* Build advanced ML models for rating prediction.
* Deploy interactive dashboards with **Streamlit** or **Dash**.
* Add NLP analysis on app descriptions (if available).

---

---

