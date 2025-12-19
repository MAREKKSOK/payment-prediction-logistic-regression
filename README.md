# payment-prediction-logistic-regression
Built a logistic regression model to predict 90-day payment probability and support debt collection prioritization using behavioral and financial data.

1.	Bussiness problem:
  •	MAIN GOAL:  Select customers who will make a payment within the next 90 days.
  •	SECONDARY GOAL: Find the most important features related to payment.
  This can help make better decisions when selecting cases for collection actions.

2.	5 the most important features impact with payment or not payment result:
  •	POSITIVE FEATURES:
    1)	Previous payment sum
    2)	Product type telco
    3)	Product type utilities
    4)	Payment promises
    5)	Previous payment count
  •	NEGATIVE FEATURES:
    1)	Income level low
    2)	Risk segment D
    3)	Employment status unemployment
    4)	Risk segment C
    5)	Employment status retired
  SUMMARISE:
    The strongest positive features related to payment are previous payment behavior and customer engagement.
    Customers who made payments in the past or promised payments are more likely to pay again.
    On the other hand, low income level, high risk segments (C and D), and unemployment significantly reduce the probability of payment.
    This confirms that both behavioral and financial features are important for repayment prediction.

3.	Business recommendation
  •	Cases with the highest probability of payment  
    o	Customers with previous payment history and fewer overdue days should be prioritized. The model shows that these features have the strongest impact on payment within the next 90 days.

  •	Cases to deprioritize  
    o	Customers with low income level, especially unemployed and retired individuals, have a lower probability of payment.
      For these cases, intensive collection actions are less likely to be effective.

  •	Model usage
    o	The model can be used to rank customers by probability of payment. Customers with higher probability can be contacted first using soft collection actions. Customers with very low probability can be deprioritized.

IMPORTANT
The model should be used as a decision-support tool, not as a final decision maker.
