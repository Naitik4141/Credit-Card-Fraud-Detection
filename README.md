# Credit-Card-Fraud-Detection
Credit Card Fraud Detection
# 💳 Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using a supervised machine learning approach. The dataset is highly imbalanced, with very few fraud cases, making it a challenging real-world problem for classification.

---

## 📂 Dataset

The dataset is publicly available on [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud) and contains:

- 284,807 transactions
- 492 fraud cases (~0.17%)
- Features are anonymized via PCA (`V1` to `V28`)
- `Amount` and `Time` features included
- `Class`: Target variable (0 = normal, 1 = fraud)

---

## 🧠 Problem Statement

Credit card fraud detection is critical for banks and financial institutions to prevent unauthorized transactions. This project builds a machine learning model to classify transactions as **fraud** or **non-fraud**, and evaluates the model using various metrics due to the data imbalance.

---

## 🛠️ Tools & Technologies

- Python 🐍
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 🚀 Workflow

1. **Data Preprocessing**
   - Drop irrelevant columns (e.g., `Time`)
   - Split data into train/test with class stratification

2. **Modeling**
   - Train a `RandomForestClassifier` with `class_weight='balanced'`

3. **Evaluation**
   - Generate a confusion matrix heatmap
   - Calculate Accuracy, Precision, and Recall

---

## 📊 Results

Sample Output (varies by run):


Confusion Matrix:

| Actual / Predicted | Not Fraud | Fraud |
|--------------------|-----------|-------|
| **Not Fraud**      | 56863     | 32    |
| **Fraud**          | 4         | 103   |

---

## 📁 Project Structure


---

## 🧪 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
