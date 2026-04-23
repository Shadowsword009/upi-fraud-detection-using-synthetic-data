# 💳 UPI Fraud Detection using Machine Learning

## 🔍 Overview

Digital payments are growing rapidly, and so is fraud. This project demonstrates how machine learning can be used to **identify suspicious UPI transactions** using a **Random Forest Classifier** trained on **synthetically generated data**.

Since real financial datasets are highly restricted, this project simulates realistic transaction patterns using the `Faker` library—making it a practical prototype for fraud detection systems.

---

## ⚙️ Key Features

* 🔐 Detects **fraudulent vs legitimate transactions**
* 🧪 Generates **realistic synthetic UPI data**
* 🧠 Uses **Random Forest Classifier** for prediction
* 🔄 Handles categorical data with **One-Hot Encoding**
* 📊 Provides **accuracy, precision, recall, and F1-score**
* 👀 Shows **sample predictions** for validation

---

## 🧰 Tech Stack

* **Python**
* **Pandas** – Data handling
* **NumPy** – Numerical computation
* **Faker** – Synthetic data generation
* **Scikit-learn** – ML model & evaluation

---

## 📂 Dataset Details

This project uses synthetic data to mimic real-world UPI transactions:

| Feature             | Description                            |
| ------------------- | -------------------------------------- |
| 💰 Amount           | Transaction value (INR)                |
| 🕒 TimeOfDay        | Morning / Afternoon / Evening / Night  |
| 🏦 SenderBank       | Randomly generated bank names          |
| 🏦 ReceiverBank     | Randomly generated bank names          |
| 📍 SenderLocation   | Random city                            |
| 📍 ReceiverLocation | Random city                            |
| 🚨 Fraud            | 0 = Legit, 1 = Fraud (~10% fraud rate) |

---

## 🧠 Model

### Random Forest Classifier

* Handles both **categorical and numerical features**
* Robust against overfitting
* Performs well on structured/tabular data

---

## 📈 Results

* ✅ Accuracy: ~90% *(varies due to randomness)*
* 📊 Includes classification metrics:

  * Precision
  * Recall
  * F1-score

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/upi-fraud-detection-using-synthetic-data.git
cd upi-fraud-detection-using-synthetic-data
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Project

```bash
python main.py
```

---

## 📊 Sample Output

```
Transaction: ₹4500 | Evening | Mumbai → Delhi
Prediction: Legit (0)

Transaction: ₹98000 | Night | Unknown → Unknown
Prediction: Fraud (1)
```

---

## ⚠️ Limitations

* Synthetic data may not fully capture real-world fraud patterns
* Model performance may vary across runs
* Not production-ready without real transaction data

---

## 🔮 Future Improvements

* 🔍 Use **real-world anonymized datasets**
* ⚡ Try advanced models (XGBoost, Neural Networks)
* 🌐 Build a **web dashboard for real-time detection**
* 📉 Handle **class imbalance more effectively (SMOTE, etc.)**

---

## 🤝 Contributing

Pull requests are welcome. If you have ideas for improvement, feel free to fork and contribute!

---

## 📜 License

This project is open-source and available under the MIT License.

---

## ⭐ Support

If you found this useful, consider giving it a ⭐ on GitHub!
