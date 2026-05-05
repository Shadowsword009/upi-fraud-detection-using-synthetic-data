# 💳 UPI Fraud Detection using Synthetic Behavioral Data

## 📌 Overview
This project builds a **machine learning-based fraud detection system** for UPI transactions using **synthetic but behaviorally realistic data**.

Instead of relying on simple rule-based signals, the system incorporates **user behavior patterns** such as transaction deviation, device changes, and transaction velocity to simulate real-world fraud scenarios.

---

## 🚀 Key Highlights
- Detects **Fraud (1)** vs **Legit (0)** transactions
- Uses **behavioral features** (not just static rules)
- Implements **Random Forest Classifier** for robust tabular learning
- Optimizes decision threshold using **Precision–Recall trade-off**
- Demonstrates real-world ML concept:  
  👉 *High recall vs precision trade-off in fraud detection*

---

## 🧠 Features Used

### 🔹 Transaction Features
- Amount
- Time (encoded using sine/cosine transformation)
- Transaction Type
- Location
- Device

### 🔹 Behavioral Features (Core Strength)
- **RelAmount** → deviation from user's normal spending
- **DeviceChange** → new device usage
- **LocationChange** → unusual location
- **Velocity** → number of recent transactions

---

## 🛠 Tech Stack
- Python 🐍  
- Pandas  
- NumPy  
- Scikit-learn  

---

## 📂 Dataset
- Fully **synthetic dataset (~15,000 transactions)**
- Fraud rate: **~10% (realistic distribution)**
- Designed to simulate:
  - high-risk behavior patterns  
  - normal user activity  
  - probabilistic fraud occurrence  

---

## 🤖 Model
- **Random Forest Classifier**
- Handles mixed feature types and non-linear patterns effectively
- Uses **class balancing** for imbalanced fraud detection

---

## 📈 Results

| Metric | Value |
|------|------|
| Precision | ~0.25 |
| Recall | ~0.54 |
| Accuracy | ~0.85 |

### 🔍 Interpretation
- High recall ensures most fraud cases are detected  
- Moderate precision reflects realistic false-positive trade-offs  

---

## ⚖️ Key Insight
Fraud detection is not about maximizing accuracy.

This project demonstrates:
> **“Balancing fraud detection (recall) and user experience (precision)”**

---

## ▶️ How to Run

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
pip install -r requirements.txt
jupyter notebook