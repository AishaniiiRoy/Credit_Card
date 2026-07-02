# Credit Card Default Risk Prediction using Logistic Regression

This repository contains an end-to-end statistical analysis and predictive modeling framework designed to identify high-risk credit applicants. Using **Logistic Regression**, we isolate the demographic and behavioral characteristics that mathematically impact a borrower's likelihood of default (`status`).

## 📊 Core Model Discoveries

By evaluating feature significance using a standard threshold of $\alpha = 0.05$, the model reveals distinct indicators for risk mitigation and risk escalation:

### 🔹 Strong Protective Factors (Reduces Default Risk)
* **Checking Account Status (`checkin_acc_A14`, `checkin_acc_A13`):** Having a robust checking account balance ($\ge 200$ DM) or not having an account open at all correlates strongly with lower default rates.
* **Credit History (`credit_history_A34`):** A history of clean, duly paid-back credits serves as a powerful indicator of reliability.
* **Demographics (`age`):** Older individuals exhibit a statistically significant reduction in overall default probability.

### 🔸 High Risk Drivers (Increases Default Risk)
* **Financial Strain (`inst_rate`):** High installment rates relative to an applicant's disposable income significantly spike default risk.
* **Loan Terms (`duration`, `amount`):** Prolonged loan durations and exceptionally high credit amounts are statistically tied to higher default probabilities.
