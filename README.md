# 📊 Binary Classification with Machine Learning | Titanic Survival Prediction

This project compares multiple supervised learning algorithms for binary classification using the Titanic dataset. It covers **data preprocessing**, **model training**, **evaluation**, and **cross-validation**, all implemented in Python within Google Colab.

--- 

## 🛠️ Tech Stack
- **Language:** Python 3
- **Libraries:** scikit-learn, pandas, numpy, seaborn, matplotlib  
- **Platform:** Google Colab  

---

## 📂 Project Structure
| File | Description |
|------|-------------|
| `Clasification.ipynb` | Core notebook containing data preprocessing, model training, evaluation, and cross-validation |
| `README.md` | Project overview and documentation |

---

## 🔄 Workflow Overview

### **1. Data Preprocessing**
- Loaded Titanic dataset from `seaborn`
- Dropped irrelevant columns: `deck`, `embark_town`, `alive`, `class`, `who`, `adult_male`
- Handled missing values:
  - Filled `age` with mean
  - Dropped rows with missing `embarked`
- Encoded categorical variables (`sex`, `embarked`) using **Label Encoding**
- Converted all features to integers for model compatibility
- Applied **StandardScaler** for feature scaling (required for KNN, SVM, Decision Tree)

---

### **2. Models Implemented**
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Gaussian Naive Bayes (GNB)  
- Decision Tree Classifier  
- Support Vector Machine (SVM - Linear Kernel)  

---

### **3. Model Training & Evaluation**
- **Train-Test Split:** 80% training, 20% testing  
- Evaluation Metrics:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-Score)

---

### **4. Cross-Validation**
- Applied **5-fold Cross-Validation** for:
  - SVM (Linear Kernel)
  - KNN
- Reported mean accuracy from cross-validation

---

## 📈 Results Summary

| Model                  | Accuracy | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) |
|------------------------|----------|---------------------|------------------|--------------------|
| Logistic Regression    | 0.803    | 0.74                 | 0.77             | 0.75               |
| KNN                    | 0.792    | 0.72                 | 0.75             | 0.74               |
| Gaussian Naive Bayes   | 0.803    | 0.74                 | 0.77             | 0.75               |
| Decision Tree          | 0.803    | 0.74                 | 0.77             | 0.75               |
| SVM (Linear Kernel)    | 0.803    | 0.74                 | 0.77             | 0.75               |

**Cross-Validation Mean Accuracy:**
- SVM: ~0.787  
- KNN: ~0.799  



