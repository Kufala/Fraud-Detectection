# 🛡️ Credit Card Fraud Detection  
A machine learning project for detecting fraudulent credit card transactions using Logistic Regression, Random Forest, and XGBoost.

---

## 🚀 Project Overview
Credit card fraud is rare but costly. This project uses anonymized PCA-transformed features to build predictive models that distinguish fraud from legitimate transactions.

### Key Highlights
- Highly imbalanced dataset (fraud ≈ 0.17%)
- SMOTE + Class Weight balancing strategies
- Logistic Regression, Random Forest, XGBoost
- Comprehensive EDA & preprocessing pipeline
- Modular, production-style source code

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection
pip install -r requirements.txt
```

---

## 📊 Dataset Description

- `Time`: Seconds since first transaction  
- `V1`–`V28`: PCA-anonymized features  
- `Amount`: Transaction value  
- `Class`: 0 = normal, 1 = fraud  

---

## 🔧 Preprocessing Pipeline

1. Load raw data  
2. Handle missing values  
3. Scale `Amount` & `Time`  
4. Save processed dataset to `data/processed/`  

Run:
```bash
python src/preprocess.py
```

---

## 🤖 Model Training

Trains Logistic Regression, Random Forest, and XGBoost.

Run:
```bash
python src/train.py
```

Trained model saved in `/models`.

---

## 📈 Model Evaluation

Generates classification metrics + ROC-AUC.

Run:
```bash
python src/evaluate.py
```

---

## 📚 Notebook

A full notebook combining EDA, preprocessing, modeling:

```
notebooks/EDA_and_Modeling.ipynb
```

---

## 🛠️ Technologies Used
- Python
- NumPy, Pandas
- Scikit-learn
- XGBoost
- Imbalanced-learn
- Matplotlib, Seaborn

---

## 🏁 Future Improvements
- Neural network model
- More advanced anomaly detection
- Model deployment via API
- Streamlit dashboard

---

## 📬 Contact
For questions or contributions, open an issue or pull request.

