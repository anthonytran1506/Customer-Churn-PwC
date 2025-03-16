# Telecom Customer Churn Prediction

This project, conducted by PwC’s Data & Analytics Consulting Division, focuses on identifying and mitigating customer churn for a leading telecom company. The analysis involves exploratory data analysis (EDA) and developing machine learning models to predict churn, offering data-driven strategies for improving retention and profitability.

---

## 📊 Project Overview
- **Objective:** Analyse customer behaviour, identify key churn drivers, and develop strategies to improve retention.
- **Dataset:** Telecom customer data including demographics, services, billing, and support history.
- **Methodology:** EDA, feature engineering, machine learning model training and evaluation, and strategic recommendations.

---

## 🎭 Key Findings
- **Churn Rate:** Over 25% of customers are churning, with higher rates among newer customers (<5 months tenure).
  ![image](https://github.com/user-attachments/assets/e41c7377-f443-4498-929b-a6696044a178)
  Figure 1. Churn Distribution

- **High-Risk Factors:**
  - **Frequent Technical Issues:** Customers with higher number of technical ticket are more likely to churn.
    ![image](https://github.com/user-attachments/assets/69c76cd6-dc2d-4d21-8e18-ac9c5401dee1)
    Figure 2. Churn Rate by Number of Technical Tickets

  - **Contract Type:** Month-to-month contracts exhibit higher churn risk.
    ![image](https://github.com/user-attachments/assets/73feb817-4e03-448a-89ac-0d983f412f0d)

Figure 3. Churn Rate by Contract Type

  - **Billing Methods:** Customers using electronic checks and paperless billing show increased churn rates.
     ![image](https://github.com/user-attachments/assets/5bc8f6ed-494f-4fae-b0a9-dd016788ad0e)

Figure 4. Churn Rate by Billing Methods (Paperless Billing)

    
![image](https://github.com/user-attachments/assets/8cc2c2c3-d682-426e-9fa9-46ddb51f6225)

    
  Figure 5. Churn Rate by Payment Method

  - **Higher Costs:** Customers with higher monthly and total charges are more likely to churn.
    ![image](https://github.com/user-attachments/assets/fb06a6b5-8395-46af-a321-797b07c19979)

Figure 6. Churn by Monthly Charge

![image](https://github.com/user-attachments/assets/795fca4e-d12c-4267-bb1a-fdf9d5866a17)


Figure 7. Churn by Total Charge

---

## 🔄 Feature Engineering
- **Support Ticket Ratio:** Ratio of technical to administrative tickets, highlighting technical issues' impact on churn.
  ![image](https://github.com/user-attachments/assets/cf05c878-4b6f-4f6d-83de-2ec3da4ddce0)
  Figure 8. Churn vs Support Ticket Ratio

---

## 🎨 Model Training & Evaluation
Four machine learning models were evaluated using accuracy, precision, recall, F1-score, and AUC-ROC.

| **Model**                  | **Accuracy** | **Precision** | **Recall** | **F1-Score** | **AUC-ROC** |
|----------------------------|--------------|--------------|-----------|-------------|-------------|
| Logistic Regression        | 0.85         | 0.73         | 0.68      | 0.70        | 0.79        |
| Tuned Decision Tree        | 0.83         | 0.71         | 0.61      | 0.66        | 0.76        |
| **Tuned Random Forest**    | **0.85**     | **0.74**     | **0.66**  | **0.70**    | **0.79**    |
| Support Vector Machine     | 0.84         | 0.72         | 0.66      | 0.69        | 0.78        |

- **Best Model:** The **Tuned Random Forest** offers the highest precision and robust performance, making it the optimal choice for churn prediction.
  ![image](https://github.com/user-attachments/assets/d1dab195-a4fa-40bc-afe8-d9ecf22cac2a)

Figure 9. Tuned Random Forest - Confusion Matrix

- **Feature Importance:**
  - Top predictors include **Support Ticket Ratio, numTechTickets, tenure, contract type,** and **total charges.**
    ![image](https://github.com/user-attachments/assets/83987391-92a0-4e9f-9988-d803c76f1af2)
    Figure 10. Feature Importance

---

## 🌐 Retention Strategies

### Customer Retention Programmes
- Offer **loyalty discounts** for long-tenure customers.
- Provide **incentives for bundled packages**, enhancing engagement for services like TechSupport and Streaming.
- Introduce **reward programs** for exclusive perks.

### Billing and Payment Flexibility
- Promote **stable payment methods** like bank transfers or credit cards over electronic checks.
- Offer **payment-splitting plans** for higher charges.
- Enable **flexible switching** between payment methods.

### Service Quality Improvements
- Prioritise **fast resolution** for technical issues.
- Conduct **regular audits** for fiber optic services.
- Implement **proactive issue detection** using analytics.
- Gather and act on **customer feedback** to address recurring issues.

### Proactive Customer Engagement
- Use the **churn prediction model** to identify high-risk customers.
- Offer **personalised discounts** and upgrades.
- Conduct **regular check-ins** with customers on month-to-month contracts or those with frequent technical issues.

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

## 👋 Contact
For questions or feedback, please reach out to [Nguyen Khanh Toan (Andrew) Tran](mailto:toantran2005.work@gmail.com).

---

## 📅 License
This project is licensed under the MIT License.

