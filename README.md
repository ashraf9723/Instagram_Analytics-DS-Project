# Instagram Analytics & Performance Prediction

## 📌 Project Overview
This project provides a comprehensive analysis of Instagram post performance using a dataset sourced from **Kaggle**. The goal is to understand the key drivers of engagement, optimize content strategies, and build a machine learning model to predict future engagement rates.

## 📂 Dataset
* **Source:** Kaggle
* **File:** `Instagram_Analytics.csv`
* **Size:** 29,999 records
* **Key Columns:** `likes`, `comments`, `shares`, `saves`, `reach`, `impressions`, `hashtags_count`, `content_category`, `engagement_rate`.

## 🛠️ Technologies
* Python 3.x
* Pandas & NumPy (Data Manipulation)
* Matplotlib & Seaborn (Visualization)
* Scipy (Statistical Analysis)
* Scikit-Learn (Machine Learning)

## 🚀 Analysis Summary

### 1. Statistical Analysis
* **ANOVA Test:** We tested if the type of media (Reel vs Photo vs Video) impacts engagement. 
    * *Finding:* No statistically significant difference was found ($p > 0.05$).
* **Category Analysis:** "Beauty" and "Photography" categories showed the highest average engagement.

### 2. Optimization
* **Hashtag Strategy:** Analyzed the relationship between hashtag count and engagement.
    * *Optimal Count:* The analysis suggests **0 hashtags** (or minimal usage) correlates with higher engagement in this specific dataset.

### 3. Signal Processing
* Applied a **7-Day Moving Average** filter to the time-series data to smooth out daily volatility and visualize the underlying engagement trend.

### 4. Predictive Modeling
* **Model:** Random Forest Regressor
* **Accuracy:** $R^2$ Score of **0.59**
* **Key Drivers:** `Impressions`, `Likes`, and `Saves` were identified as the most important features for predicting engagement.

## 💻 How to Run
1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy scikit-learn
