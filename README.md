# 🎬 Cinema Audience Forecasting Challenge

**IIT Madras – Kaggle Tournament**

🏆 **Final Rank: 17 / 2,632 participants**

📅 **Duration:** 3 Months

🎯 **Objective:** Forecast daily audience counts for **826+ cinemas** across India

---

## 🚀 Project Summary

An **end-to-end machine learning project** built from scratch as part of an IIT Madras–hosted Kaggle competition.
The task involved predicting daily cinema footfall using **messy, multi-source data**, requiring careful data selection, feature engineering, and time-aware modeling.

This project secured a **Top-20 finish** in a highly competitive leaderboard.

---

## 🔍 Problem Framing

* Multi-theatre **panel time-series forecasting**
* Strong **weekly seasonality**
* Theatre-level behavior differences
* Structural shift due to **platform expansion** (mid-2023)

Key insight:
📌 Audience spikes were **supply-driven (new theatres)**, while **weekly viewing behavior remained stable and predictable**.

---

## 🧠 Data & Feature Engineering

* Started with **7+ raw CSV files**
* After extensive experimentation, retained **only the most predictive sources**:

  * Daily audience counts
  * Booking activity trends
  * Calendar features (day, week, month)
* Built a unified modeling table using **time-safe left joins**

**Core features:**

* Lag features (1, 7, 14 days)
* Rolling means (7, 14 days)
* Weekend indicators
* Theatre-level encoded identifiers

Final dataset: **213K+ rows × 12 features**

---

## ⚙️ Modeling Approach

* Time-based train–validation split
* Evaluated multiple models:

  * Gradient Boosting
  * LightGBM
  * XGBoost
  * Random Forest
  * Linear baselines
* Hyperparameter tuning via **RandomizedSearchCV**

🏆 **Best Model:** Tuned Gradient Boosting
Chosen for strongest generalization and leaderboard performance

---

## 📊 Results

* **Final Rank:** 17 / 2,632
* Robust performance across unseen theatres and future dates
* Successfully handled seasonality, noise, and platform-level shifts

---

## 📁 Repository Structure

* `Cinema_Dataset/` – Complete raw dataset
* `CompleteCodeNotebook_IITM.ipynb` – Full end-to-end pipeline
* `HighestScoringNotebook_Code.ipynb` – Optimized notebook used for the **Rank 17 submission**
* `README.md` – Project overview

---

## 📝 Detailed Walkthrough

👉 **Full project explanation & insights:**
**[Lights, Camera, Prediction: Forecasting Cinema Audiences with Machine Learning](https://medium.com/@pragyatripathii19/lights-camera-prediction-forecasting-cinema-audiences-with-machine-learning-ae752f417fa0)**

---

## 🔑 Why This Project Stands Out

✔ Built from raw, multi-source data

✔ Clear time-series reasoning

✔ Strong feature engineering focus

✔ Competitive, ranked ML solution

✔ Mirrors real-world forecasting challenges

---

### ⚠️ Disclaimer

Completed as part of an academic Kaggle competition. Data used solely for learning and evaluation purposes.

---
