# 🛒 E-Commerce Customer Segmentation & Prediction

An end-to-end machine learning project that segments e-commerce customers based on purchasing behavior and predicts customer segments to enable **targeted marketing, customer retention, and inventory optimization**.

---

## 📌 Project Overview

Understanding customer behavior is critical for improving marketing efficiency and retention in e-commerce.  
This project leverages **transactional data and machine learning** to:

- Segment customers using **RFM and behavioral features**
- Predict customer segments using supervised ML models
- Translate ML outputs into **actionable business strategies**

The solution combines **descriptive analytics (segmentation)** with **predictive analytics (classification)** to support data-driven decision-making.

---

## 🎯 Business Objectives

- Identify high-value and at-risk customers
- Enable personalized marketing strategies
- Improve customer retention
- Support inventory planning and cost optimization

---

## 📊 Dataset Description

The dataset contains **e-commerce transactional data**, including:

- Customer purchase history
- Product information
- Order quantities and values
- Cancellations and returns
- Purchase timestamps

---

## 🧠 Methodology

### 1️⃣ Exploratory Data Analysis (EDA)
- Transaction trends analysis
- Customer purchase behavior
- Revenue and order distribution
- Cancellation analysis

### 2️⃣ Feature Engineering
Created customer-level features including:
- **Recency**
- **Frequency**
- **Monetary Value**
- **Average Order Value**
- **Product Diversity**
- **Cancel Rate**
- **Customer Lifetime Value (CLV)**

These features capture both **value and behavior**.

---

### 3️⃣ Customer Segmentation (Unsupervised Learning)

Tested and compared multiple clustering algorithms:

| Algorithm | Purpose |
|---------|--------|
| K-Means | Final segmentation (interpretable & scalable) |
| Hierarchical | Structural insights |
| DBSCAN | Noise & density detection |
| GMM | Probabilistic clustering |

**Model Selection Metrics:**
- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Score

✅ **K-Means selected** for final deployment.

---

### 4️⃣ Segment Interpretation & Labeling

| Segment | Label |
|------|------|
| 0 | Champions / VIP Customers |
| 1 | Low-Value / One-Time Customers |
| 2 | Loyal Customers |
| 3 | At-Risk / High-Churn Customers |

Each segment was mapped to **business-ready actions**.

---

### 5️⃣ Predictive Modeling (Supervised Learning)

Built models to **predict customer segments**:

- Logistic Regression
- Random Forest
- XGBoost (final model)

**Evaluation Metrics:**
- Accuracy
- Precision / Recall
- F1-Score
- ROC-AUC

🏆 **XGBoost achieved ~97% F1-Score**

---

## 🎯 Business Actions by Segment

| Segment | Recommended Action |
|------|------------------|
| Champions | Loyalty rewards, exclusive offers |
| Loyal | Cross-sell & repeat purchase incentives |
| Low-Value | Low-cost promotions or onboarding |
| At-Risk | Win-back campaigns, churn reduction |

---

## 📦 Inventory Management Insights

- Prioritize stock for **Champions & Loyal customers**
- Reduce overstocking for **Low-Value segments**
- Forecast demand using segment behavior

---

## ⚠️ Notes on Data Leakage

- Labels are derived from historical transactions
- Random train-test split used due to lack of future timestamps
- In production, **time-based validation** is recommended

---

## 🛠️ Tech Stack

- **Python**
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---
## 📁 Repository Structure
---
├── data/
│ └── ecommerce_customer_segmentation_dataset.csv
├── notebooks/
│ └── E-commerce Customer Segmentation & Prediction.ipynb
├── models/
│ └── final_model.pkl
├── README.md

---

## 🚀 Key Outcomes

- Actionable customer segmentation
- High-performance predictive model
- Strong alignment between **ML and business goals**
- Ready for **real-world deployment**

---

## 📌 Future Improvements

- Time-based validation to avoid leakage
- Real-time segment updates
- Integration with CRM & marketing automation tools
- Power BI / Tableau dashboards

---


## 📁 Repository Structure
