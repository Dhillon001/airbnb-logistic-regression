# 📊 Airbnb Superhost Classification using Logistic Regression🏡💰

**Project:** Classify whether an Airbnb host is a **Superhost** using logistic regression.

---

## 🎯 Objective

Given **preprocessed Airbnb data**, build and tune a logistic regression model to predict:

- `host_is_superhost = True` or `False`

---

## 📦 Dataset

- **File**: `data_LR/airbnbData_train.csv`  
- **Preprocessing already applied**:  
  - One-hot encoding of categoricals  
  - Scaling of numerics  
  - Missing-value imputation  

- **Label**: `host_is_superhost` (boolean)  
- **Features**: All remaining columns in the CSV after dropping the label

---

## ⚙️ Workflow

1. Train Logistic Regression with default hyperparameter
2. Tune `C` using GridSearchCV
3. Evaluate using accuracy, confusion matrix, precision-recall, and ROC-AUC
4. Use `SelectKBest` to try feature selection
5. Save best model using `pickle`

---

## 📈 Results

- **Best C** from GridSearch: `1000`
- **Accuracy (best model)**: ~81.16%
- **AUC (best model)**: ~0.8209
- **AUC after feature selection (Top 5 features)**: ~0.7926

---

## 📂 Key Files

- `airbnbData_train.csv`
- `model_best.pkl`
- `README_Lab5_ML_Life_Cycle.md`

---

## 🛠️ Tools & Libraries

- Python 3.9  
- Pandas, NumPy  
- scikit-learn  
- Matplotlib, Seaborn  

---

## ✍️ Author

Harsharandeep Dhillon  

