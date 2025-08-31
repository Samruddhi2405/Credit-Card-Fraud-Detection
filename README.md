# 💳 Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset is highly imbalanced, with very few fraud cases compared to non-fraud transactions, making it a challenging classification problem.

---

## 📊 Dataset
- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Size**: ~285,000 transactions, 31 features  
- **Target Variable**:  
  - `0` → Legitimate transaction  
  - `1` → Fraudulent transaction  

⚠️ **Note:** The dataset is not included in this repository. Download it from Kaggle and place it in your working directory (e.g., `Downloads/creditcard.csv`).

---

# 💳 Credit Card Fraud Detection

This project implements a **Machine Learning model** to detect fraudulent credit card transactions using the [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud).  
It demonstrates **data preprocessing, model training, evaluation, and visualization** of fraud detection performance.

---

## 📂 Project Structure
Credit-Card-Fraud-Detection/
│── dataset/ # (keep empty, dataset is large, not uploaded to GitHub)
│── notebooks/
│ └── fraud_detection.ipynb # Jupyter Notebook with code
│── README.md # Project documentation

markdown
Copy code

---

## 📊 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Description**:
  - Contains transactions made by European cardholders in September 2013.
  - 284,807 transactions in total.
  - Only **492 frauds** → dataset is **highly imbalanced**.
  - Features are **numerical** after PCA transformation for confidentiality.
  - Includes:
    - `Time`, `Amount`
    - `V1` … `V28` (anonymized features)
    - `Class` → `1` = Fraud, `0` = Normal transaction

⚠️ **Note:** Dataset is not uploaded to this repo (file size >100MB).  
Please download it manually from Kaggle and place it in your system (e.g., `Downloads/creditcard.csv`).

---

## ⚙️ Installation & Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/Samruddhi2405/Credit-Card-Fraud-Detection.git
   cd Credit-Card-Fraud-Detection
Create a virtual environment (optional but recommended):

python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)
Install dependencies:


pip install -r requirements.txt
(If you don’t have requirements.txt, manually install common libraries: numpy pandas scikit-learn matplotlib seaborn jupyter)

Open Jupyter Notebook:

jupyter notebook
Navigate to notebooks/fraud_detection.ipynb and run the cells.

🚀 Workflow
Load Dataset

python

data = pd.read_csv("C:/Users/<YourName>/Downloads/creditcard.csv")
Data Preprocessing

Handle class imbalance

Normalize Amount and Time

Model Training

Logistic Regression

Random Forest

XGBoost (optional)

Evaluation Metrics

Confusion Matrix

Precision, Recall, F1-score

ROC-AUC Curve

📈 Results
Due to class imbalance, accuracy alone is not reliable.

Models are evaluated using Precision, Recall, F1-score, and AUC.

Random Forest and XGBoost generally perform better in fraud detection.
