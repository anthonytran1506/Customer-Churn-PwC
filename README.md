# Telecom Customer Churn Prediction

This project focuses on building and evaluating machine learning models to predict customer churn for a telecom company. The aim is to identify key churn drivers and propose data-driven strategies to improve customer retention.

---

## 📊 Project Overview
- **Business Problem:** High customer churn rate affecting profitability.
- **Objective:** Analyze churn patterns, build predictive models, and recommend retention strategies.
- **Dataset:** Telecom customer data, including demographics, service usage, billing, and technical support history.

---

## 🔄 Data Processing
- **Data Cleaning:** Handled missing values, inconsistent data types, and irrelevant features.
- **Feature Engineering:**
  - Created features like `Support_Ticket_Ratio`, `Month_Used`, and `tenure_group`.
  - Categorized contract types and payment methods.
- **Encoding & Scaling:** Applied necessary transformations for model compatibility.

---

## 📊 Exploratory Data Analysis (EDA)
- Identified key churn indicators like tenure, payment method, and contract type.
- Visualized relationships between features and churn to uncover trends.

---

## 🎨 Models and Evaluation

### 1. **Logistic Regression**
- **Accuracy:** 0.85  
- **Precision (Churn):** 0.73  
- **Recall (Churn):** 0.68  
- **F1-Score:** 0.70  
- **AUC-ROC:** 0.79

### 2. **Tuned Decision Tree**
- **Accuracy:** 0.83  
- **Precision (Churn):** 0.71  
- **Recall (Churn):** 0.61  
- **F1-Score:** 0.66  
- **AUC-ROC:** 0.76

### 3. **Tuned Random Forest**
- **Accuracy:** 0.85  
- **Precision (Churn):** 0.74  
- **Recall (Churn):** 0.66  
- **F1-Score:** 0.70  
- **AUC-ROC:** 0.79

### 4. **Support Vector Machine (SVM)**
- **Accuracy:** 0.84  
- **Precision (Churn):** 0.72  
- **Recall (Churn):** 0.66  
- **F1-Score:** 0.69  
- **AUC-ROC:** 0.78

### 📊 **Best Performing Model:**
- The **Tuned Random Forest** offers the best precision for churn detection, balanced recall, and strong feature interpretability.

---

## 🔗 Key Findings & Retention Strategies

- **Technical Issues Drive Churn:** Focus on reducing support ticket ratios and resolution times.
- **Contract Type Matters:** Promote long-term contracts with incentives.
- **Pricing Impacts Churn:** Introduce payment plans for customers with higher charges.
- **Payment Method Influence:** Encourage stable payment methods over electronic checks.
- **Service Quality:** Regular audits for fiber optic services to ensure reliability.

---

## 💡 Next Steps
- **Deploy the Random Forest model** for live churn prediction.
- Integrate churn predictions with CRM systems for targeted retention strategies.
- Continuously monitor and retrain the model for improved accuracy.

---

## ⚙️ Installation & Usage
1. Clone this repository:
```bash
git clone https://github.com/yourusername/telecom-churn-prediction.git
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the model:
```bash
python churn_model.py
```

---

## 📧 Contact
For questions or feedback, feel free to reach out to [Your Name](mailto:your.email@example.com).

---

## 📅 License
This project is licensed under the MIT License.

