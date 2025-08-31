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

## ⚙️ Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
Create a virtual environment (recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows
Install dependencies:

bash
Copy code
pip install -r requirements.txt
🚀 Usage
Place the dataset in your working directory:

bash
Copy code
~/Downloads/creditcard.csv
Run the Jupyter notebooks step by step:

bash
Copy code
jupyter notebook
Notebooks included:

01_exploration.ipynb → Data exploration & preprocessing

02_modeling.ipynb → Training, evaluation, and metrics

📈 Results
Models tested: Logistic Regression, Random Forest, XGBoost

Metrics used: Accuracy, Precision, Recall, F1-score, ROC-AUC

Example results (Random Forest):

Accuracy: ~99%

Precision: High (few false positives)

Recall: Moderate (some fraud cases may be missed)



📌 References
1) Kaggle Dataset
2) Imbalanced Classification techniques
3) scikit-learn documentation

