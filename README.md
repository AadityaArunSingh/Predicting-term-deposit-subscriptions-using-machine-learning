# Bank Marketing – Term Deposit Subscription Prediction

This project was developed as part of **COMM053 – Practical Business Analytics** at the University of Surrey.

The objective is to predict whether a customer will subscribe to a term deposit **before** a marketing call is made, enabling more efficient and cost-effective campaign targeting.

---

## 📊 Dataset
- Source: UCI Bank Marketing Dataset
- Target variable: `y` (term deposit subscription: yes / no)
- Strong class imbalance reflecting real-world telemarketing outcomes

---

## ⚙️ Data Preprocessing
- Removed leakage features (e.g. `duration`)
- Handled high proportion of `"unknown"` values
- Feature engineering:
  - Binary variable for prior contact
- One-hot encoding for categorical variables
- Feature scaling where required (model-dependent)

---

## 🤖 Models Implemented
- Logistic Regression (baseline & enhanced)
- Decision Tree
- K-Nearest Neighbors (KNN)
- Support Vector Machine (RBF Kernel)
- Cost-sensitive / threshold-tuned models

Each model was evaluated with business-relevant metrics beyond accuracy.

---

## 📈 Evaluation Metrics
- Recall (priority due to business cost of missed subscribers)
- Precision
- F1-score
- ROC-AUC
- Confusion Matrix
- Precision–Recall Curve

---

## 💡 Business Insight
The models demonstrate clear trade-offs between:
- **Aggressive strategies** (high recall, lower precision)
- **Conservative strategies** (higher precision, fewer wasted calls)

This enables flexible deployment depending on campaign cost and channel.

---

## 🧑‍🎓 Author
**Aaditya Singh**  
MSc Data Science  
University of Surrey
