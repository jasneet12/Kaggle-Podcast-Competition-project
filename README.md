# 🎧 Kaggle Podcast Competition: Predicting Listening Time

![Kaggle](https://img.shields.io/badge/Kaggle-Competition-blue.svg)
![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📌 Overview

This project is a solution to the **Kaggle Podcast Competition**, where the objective is to **predict the listening time** of podcast episodes based on metadata such as host popularity, episode length, publication day, sentiment, and more.

The notebook includes:
- Comprehensive Exploratory Data Analysis (EDA)
- Feature engineering
- Model building with XGBoost
- Final predictions for submission

---

## 📂 Dataset

The dataset was provided by Kaggle and includes the following key features:

| Feature                        | Description                                     |
|-------------------------------|-------------------------------------------------|
| `Podcast_Name`                | Title of the podcast                            |
| `Episode_Title`              | Title of the episode                            |
| `Episode_Length_minutes`     | Duration of the episode                         |
| `Host_Popularity_percentage` | Popularity score of the host                    |
| `Guest_Popularity_percentage`| Popularity score of the guest (if present)      |
| `Number_of_Ads`              | Number of advertisements in the episode         |
| `Episode_Sentiment`          | Sentiment label (Positive/Neutral/Negative)     |
| `Listening_Time_minutes`     | Target variable (minutes listened)              |

---

## 📊 Approach

### 🔍 Exploratory Data Analysis (EDA)
- Handled missing values
- Checked class balance and correlations
- Visualized feature distributions and relationships

### 🧠 Feature Engineering
- Encoded categorical variables
- Extracted temporal features from `Publication_Time`
- Mapped `Episode_Sentiment` to numerical scores

### 🔧 Model Building
- Model: `XGBoost Regressor`
- Cross-validation with `KFold`
- Metric: **Root Mean Squared Error (RMSE)**

### 🧪 Evaluation
- Final public leaderboard score: **12.72 RMSE**
- Working towards improving it beyond **11.54557 RMSE**

---

## 📁 Repository Structure

