# MACHINE-LEARNING-PROJECT

## PROJECT TITLE: BANK COSTUMER CHURN PREDICTION
### PROBLEM STATEMENT:- 
As we know, it is much more expensive to sign in a new client than keeping an existing one. It is advantageous for banks to know what leads a client towards the decision to leave the company.

🎯 OBJECTIVE: 🏦🔍

The primary goal of this project is to develop a machine learning model to predict whether a customer will churn (i.e., leave the bank) or stay based on their demographic and financial features and use this model to identify high-risk customers (those most likely to churn) and take proactive measures to retain them, thereby improving customer retention and lowering the amount of money the bank spends to get new customers.


📌 METHODOLOGY: 🔬📊

- We fixed misspelling, missing values, and inconsistencies in the data using appropriate techniques (e.g., filling missing values, standardizing text formats).
Encoded categorical features using label encoding.
- Scaled numerical features using StandardScaler for better model performance. to improve quality.
- Through effective feature selection techniques, we pinpointed the most significant variables contributing to churn, enhancing predictive accuracy and providing valuable insights for customer retention strategies.
  
🏆FINDING THE BEST PERFORMING MODEL:🥇✨  

- Trained multiple models: Logistic Regression, Decision tree, KNeighbor classifier, Naive Bayes, Random Forest, XGBoost, and SVM.
- Compared models using accuracy, precision, recall, F1-score, and AUC-ROC curve.
- Identified XGBoost as the best-performing model with the highest AUC. The ROC curve analysis further supports the findings from the initial evaluation, indicating that the XGBoost model achieves the highest AUC among the tested classifiers.
- This reinforces the conclusion that XGBoost is particularly effective for this dataset, offering superior performance in distinguishing between classes and addresssing class imbalance.
  
🚧 CHALLENGES FACED AND SOLUTION:⚠️🔄   

- challenge was dealing with imbalanced data, which caused biased predictions.
  
**Solution:** We fixed this by removing the 'complain' feature because it was too closely related to the target and affected the results.

- Initially, models showed moderate F1-scores around(40-55%), making it difficult to determine the best one. Accuracy alone was misleading because some models had high accuracy but lower F1-scores.
  
**Solution:** Applied K-Fold Cross-Validation to get a more reliable performance estimate.After K-Fold, XGBoost had the highest F1-score (0.8387) and strong accuracy (0.8497), confirming it as the best model. Random Forest also performed well, but XGBoost showed a slight edge in both accuracy and F1-score.

🔑 KEY TAKEAWAYS: ✅📌  

- Customer churn is influenced by multiple factors such as Age, Geography, Balance, Gender, Number of Products, and Active Membership Status.
- XGBoost performed the best among all models but may require further fine-tuning for optimization.
- Feature selection played a crucial role, improving model accuracy by focusing on the most relevant variables.
  
✅ 💡RECOMMENDATIONS:🏦  

1️⃣ Personalized Banking Offers 🎯 Use customer data (age, balance, product usage) to offer customized interest rates, credit card upgrades, or lower fees.

Example: A high-balance customer might get higher interest rates on savings to encourage retention.

2️⃣ Loyalty & Rewards Programs 🎁 Provide exclusive benefits for long-term customers, such as cashback, bonus points, or VIP services.

Example: Customers who stay for 3+ years receive free premium banking services.

3️⃣ Proactive Engagement & Support 📞 Identify inactive or low-engagement customers (e.g., low transactions, rare logins) and reach out with offers, surveys, or special assistance.

Example: A customer who hasn’t used their account for months receives a personalized discount or call from a banking rep.
