# payment-prediction-logistic-regression
Built a logistic regression model to predict 90-day payment probability and support debt collection prioritization using behavioral and financial data.

## 1. Business problem

**Main goal**  
Select customers who are most likely to make a payment within the next **90 days**.

**Secondary goal**  
Identify the most important features related to payment behavior.  
This helps make better decisions when selecting cases for debt collection actions.

---

## 2. Most important features impacting payment result

### Positive features
1. Previous payment sum  
2. Product type: telco  
3. Product type: utilities  
4. Payment promises  
5. Previous payment count  

### Negative features
1. Low income level  
2. Risk segment D  
3. Employment status: unemployed  
4. Risk segment C  
5. Employment status: retired  

### Summary
The strongest positive features related to payment are **previous payment behavior** and **customer engagement**.

Customers who made payments in the past or promised payments are more likely to pay again.

On the other hand, **low income level**, **high risk segments (C and D)**, and **unemployment** significantly reduce the probability of payment.

This confirms that both **behavioral** and **financial** features are important for repayment prediction.

---

## 3. Business recommendations

### Cases with the highest probability of payment
- Customers with previous payment history  
- Customers with fewer overdue days  

These cases should be **prioritized**, as the model shows they have the strongest impact on payment within the next 90 days.

---

### Cases to deprioritize
- Customers with low income level  
- Unemployed and retired customers  
- High risk segments  

For these cases, intensive collection actions are less likely to be effective.

---

### Model usage
- The model can be used to **rank customers by probability of payment**  
- Customers with higher probability should be contacted first using **soft collection actions**  
- Customers with very low probability can be **deprioritized**

---

### Important note
The model should be used as a **decision-support tool**, not as a final decision maker.
