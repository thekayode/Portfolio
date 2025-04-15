# Portfolio

# 💳 Credit Card Fraud Detection with Logistic Regression

This project focuses on detecting fraudulent transactions in a credit card dataset using logistic regression. Fraudulent transactions are rare compared to legitimate ones, making this a classic example of an imbalanced classification problem.

---

## 📂 Dataset

The dataset used is from Kaggle's [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). It contains transactions made by European cardholders in September 2013.

- **Total records:** 284,807  
- **Features:** 30 anonymized features (V1–V28), `Time`, and `Amount`  
- **Target:** `Class`  
  - `0` → Legitimate transaction  
  - `1` → Fraudulent transaction  

---

## 📊 Exploratory Data Analysis (EDA)

- No missing values in the dataset.
- The dataset is highly imbalanced:
  - Legitimate: 284,315  
  - Fraudulent: 492  

### Observations:
- Fraudulent transactions tend to have:
  - Lower median and mean transaction amounts  
  - Distinctive patterns in certain anonymized features

---

## 🧪 Data Preprocessing

A balanced dataset was created by:

- Randomly sampling 492 legitimate transactions  
- Combining them with all 492 fraudulent transactions  

This new balanced dataset was used to train and evaluate the model to avoid bias due to class imbalance.

---

## 🔍 Model Used

- **Model:** Logistic Regression (from `scikit-learn`)  
- **Evaluation metric:** Accuracy Score  

---

## 🛠️ Tools & Libraries

- Python 3  
- Pandas  
- NumPy  
- Scikit-learn  

---

## 📈 Future Improvements

- Use additional evaluation metrics: precision, recall, F1-score  
- Explore advanced models: Random Forest, XGBoost, Neural Networks  
- Apply sampling techniques like SMOTE  
- Create a full ML pipeline for reproducibility and scalability  

---

## 📁 Usage

```bash
# Clone the repository
git clone https://github.com/yourusername/fraud-detection.git
cd fraud-detection

# Install required libraries
pip install -r requirements.txt

# Run the notebook or script
python fraud_detection.py
🙌 Acknowledgments
Kaggle Credit Card Fraud Dataset

Scikit-learn for machine learning tools
