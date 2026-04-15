# 💳 UPI Fraud Detection using Synthetic Data

## 📌 Overview
This project focuses on detecting **fraudulent UPI transactions** using a **Random Forest Classifier** trained on **synthetic data** generated with the `Faker` library.  
It demonstrates how machine learning can be applied to financial fraud detection when real-world data is unavailable.

## 🚀 Features
- Predicts if a UPI transaction is **Legit (0)** or **Fraud (1)**.
- Generates **synthetic UPI transactions** with realistic attributes (amount, banks, locations, time of day).
- Uses **One-Hot Encoding** for categorical features.
- Includes model training, testing, and accuracy evaluation.
- Displays **sample predictions** for quick verification.

## 🛠 Tech Stack
- **Python** 🐍
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Faker** – Synthetic data generation
- **Scikit-learn** – Machine learning models & evaluation

## 📂 Dataset
Since real UPI transaction data is sensitive and private, this project uses synthetic data:
- **Amount** – Transaction value in INR.
- **TimeOfDay** – Morning, Afternoon, Evening, Night.
- **SenderBank / ReceiverBank** – Randomly generated company names.
- **SenderLocation / ReceiverLocation** – Randomly generated city names.
- **Fraud** – 0 = Legit, 1 = Fraud (10% probability for fraud).

## 📊 Model Used
- **Random Forest Classifier** – Chosen for its high accuracy and ability to handle categorical & numerical data.

## 📈 Results
- Accuracy: ~90% (may vary per run due to synthetic randomness)
- Classification report showing precision, recall, and F1-score.

## 📌 How to Run
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/upi-fraud-detection-using-synthetic-data.git
   cd upi-fraud-detection-using-synthetic-data


   
