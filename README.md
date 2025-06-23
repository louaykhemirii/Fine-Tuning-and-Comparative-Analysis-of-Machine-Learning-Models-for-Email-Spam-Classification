# 📧 Spam Email Classification with Machine Learning

This project presents a comprehensive sensitivity analysis of multiple supervised learning models applied to the task of **classifying emails as spam or not spam** using the high-dimensional `spam.dat` dataset.

The main focus is to **minimize false negatives (missed spam)** while keeping **false positives under 0.5%**, in line with strict classification constraints.

---

## 🧪 Project Summary

**Dataset:** [`spam.dat`](https://spamassassin.apache.org/)  
**Target:** `yes` (spam), `no` (not spam)  
**Instances:** 4,789 emails  
**Features:** 462 binary features (SpamAssassin rules)

---

## 🔍 Sensitivity Studies Performed

| Study | Description |
|-------|-------------|
| ✅ Classifier Comparison | Logistic Regression, SVM, Decision Tree, Random Forest, MLP, k-NN, Naive Bayes, AdaBoost |
| ✅ Hyperparameter Tuning | `C`, `max_depth`, `n_neighbors`, etc. using `GridSearchCV` |
| ✅ Feature Selection | Recursive Feature Elimination (RFE) |
| ✅ Dimensionality Reduction | Principal Component Analysis (PCA) |
| ✅ Class Imbalance Handling | Random Oversampling, SMOTE |
| ✅ Cost-Sensitive Training | `class_weight` adjustment for false negative penalties |
| ✅ Ensemble Learning | AdaBoost |

---

## 📊 Key Evaluation Metrics

- **False Negative Rate (FNR)**  
- **False Positive Rate (FPR)**  
- **ROC AUC Score**  
- **Confusion Matrix**

---

## 🏆 Best Performing Model

- **Model:** Logistic Regression with SMOTE  
- **FNR:** 2.72%  
- **FPR:** 0.17% ✅ meets constraint  
- **AUC:** 0.9988

---

## 📈 Visual Results

- Model comparison chart of FNR, FPR, and AUC
- Top 10 most influential features (Logistic Regression)

---

## 📁 Repository Structure

├── spam.dat # Dataset
├── Louay Khemiri.ipynb # Main Jupyter Notebook
├── README.md # This file
└── assets/ # (Optional) plots/images for GitHub rendering


---

## 🧑‍💻 Author

**Louay Khemiri**  
MSc Student — Supervised by Maciej Nikodem  
*Comparative Analysis of Radio Propagation Models for Short-Range Radio Networks*

---

## 📜 License

This project is for academic and educational use only.

