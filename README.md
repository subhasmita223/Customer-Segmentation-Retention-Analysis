# Customer-Segmentation-Retention-Analysis


## 📌 Overview

This project builds an end-to-end customer analytics pipeline to segment users and predict churn using real-world datasets. It simulates how subscription platforms, e-commerce companies, and mobility apps (e.g., ride-sharing, food delivery, SaaS platforms) analyze user behavior to improve retention and maximize customer lifetime value (CLV).

The system integrates data preprocessing, feature engineering, unsupervised segmentation, supervised churn modeling, and business decision mapping into a single reproducible workflow.

---

## 🎯 Objectives

* Segment customers based on behavioral patterns using RFM (Recency, Frequency, Monetary) analysis
* Predict customer churn using supervised machine learning
* Identify high-value and high-risk customer segments
* Translate model outputs into actionable retention strategies
* Optimize marketing and retention resource allocation

---

## 📊 Datasets

### 1️⃣ Customer Churn Dataset (Telecom Domain)

* Customer demographics
* Service subscriptions
* Billing and contract information
* Target variable: **Churn (Yes / No)**

Used for churn prediction modeling and churn driver analysis.

### 2️⃣ Online Retail Dataset

* Transaction-level purchase data
* Invoice history
* Quantity, price, timestamps

Used for behavioral segmentation via RFM analysis.

---

## 🛠️ Tech Stack & Methods

### Tech Stack

* Python (pandas, numpy)
* Scikit-learn (Random Forest, K-Means, preprocessing)
* Matplotlib / Seaborn (visualization)
* Jupyter Notebook

### Core Methods

* Data Cleaning & Missing Value Handling
* Feature Engineering (tenure, spending patterns, service usage)
* Encoding of categorical variables
* RFM (Recency, Frequency, Monetary) scoring
* K-Means clustering for behavioral segmentation
* Random Forest classifier for churn prediction
* Model evaluation using ROC-AUC, confusion matrix, precision-recall
* Feature importance analysis to interpret churn drivers

---

## 🔍 Project Workflow

Data Ingestion
↓
Data Cleaning & Feature Engineering
↓
RFM Calculation & Behavioral Segmentation
↓
Churn Prediction Modeling
↓
Segment-Level Risk Analysis
↓
Retention Strategy Design

---

## 📈 Key Results & Insights

### 🔹 Churn Prediction

* Built a Random Forest model achieving **ROC-AUC ≈ 0.84**
* Identified key churn drivers:

  * Short customer tenure
  * Month-to-month contracts
  * High monthly charges
  * Lack of bundled services

These insights highlight contract flexibility and pricing sensitivity as major churn factors.

---

### 🔹 Customer Segmentation (RFM + Clustering)

Customers were grouped into four primary behavioral segments:

* **High-Value Loyal** – Recent, frequent, high-spending users
* **Frequent Buyers** – High frequency, moderate spending
* **At Risk** – Inactive customers with declining engagement
* **Low Engagement** – Low activity and low spending users

---

### 🔹 Retention Targeting Strategy

By combining segmentation with churn probability:

* High-value + high-risk customers were flagged for proactive retention campaigns
* Loyal customers identified for loyalty rewards and upsell strategies
* Low-value, high-risk customers deprioritized to optimize marketing spend

---

## 💡 Business Impact

This project demonstrates how data science can directly influence product and growth decisions:

* Improve retention by prioritizing high-LTV users
* Reduce churn through targeted contract or pricing adjustments
* Optimize marketing spend by focusing on valuable customer segments
* Support lifecycle management strategies in subscription and mobility platforms

The approach mirrors real-world customer analytics systems used in SaaS, e-commerce, and ride-sharing platforms.

---

## 📂 Repository Structure

```
customer-segmentation-retention-analytics/
│
├── data/
│   ├── raw/                # Original datasets
│   └── processed/          # Cleaned datasets and model outputs
│
├── notebooks/
│   └── Customer_Segmentation_and_Retention.ipynb
│
├── src/
│   └── utils.py            # Helper functions
│
├── results/
│   ├── churn_drivers.png
│   ├── segment_profiles.csv
│   └── high_value_at_risk_customers.csv
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## ⚙️ How to Run

```bash
git clone <repo-link>
cd customer-segmentation-retention-analytics
pip install -r requirements.txt
jupyter notebook notebooks/Customer_Segmentation_and_Retention.ipynb
```

---

## 🚀 Future Enhancements

* Customer Lifetime Value (CLV) prediction
* XGBoost comparison for improved churn performance
* SHAP-based model explainability
* Unified churn + segmentation scoring system
* Deployment-ready scoring API

---

## 👤 Author


