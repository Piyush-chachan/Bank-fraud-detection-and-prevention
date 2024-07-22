 # Bank fraud detection and prediction


## Overview 
Our approach to combating fraud involves utilizing advanced machine learning models to predict and prevent fraudulent transactions. By harnessing historical data and predictive analytics, we focus on delivering accurate fraud detection without extensive development work. Our ML model is designed to identify suspicious patterns and anomalies in transaction data, providing actionable insights to enhance fraud prevention efforts. This method allows for proactive intervention and timely alerts, ensuring a robust defense against emerging threats. Our solution aims to balance security with customer satisfaction, offering reliable fraud detection that supports seamless and uninterrupted transaction experiences.


# Data Description : Fraud Detection on Bank Payments
Fraud and detecting it
Fraudulent behavior can be seen across many different fields such as e-commerce, healthcare, payment and banking systems. Fraud is a billion-dollar business and it is increasing every year. The PwC global economic crime survey of 2018 [1] found that half (49 percent) of the 7,200 companies they surveyed had experienced fraud of some kind.

Even if fraud seems to be scary for businesses it can be detected using intelligent systems such as rules engines or machine learning. Most people here in Kaggle are familier with machine learning but for rule engines here is a quick information. A rules engine is a software system that executes one or more business rules in a runtime production environment. These rules are generally written by domain experts for transferring the knowledge of the problem to the rules engine and from there to production. Two rules examples for fraud detection would be limiting the number of transactions in a time period (velocity rules), denying the transactions which come from previously known fraudulent IP's and/or domains.

Rules are great for detecting some type of frauds but they can fire a lot of false positives or false negatives in some cases because they have predefined threshold values. For example let's think of a rule for denying a transaction which has an amount that is bigger than 10000 dollars for a specific user. If this user is an experienced fraudster, he/she may be aware of the fact that the system would have a threshold and he/she can just make a transaction just below the threshold value (9999 dollars).

For these type of problems ML comes for help and reduce the risk of frauds and the risk of business to lose money.With the combination of rules and machine learning, detection of the fraud would be more precise and confident.

Banksim dataset
We detect the fraudulent transactions from the Banksim dataset. This synthetically generated dataset consists of payments from various customers made in different time periods and with different amounts.


# Novelty & Impact: 
Our project stands out for its innovative combination of machine learning and financial incentives, offering a unique selling proposition where financial institutions can earn commissions on each confirmed and prevented fraud. This dual approach not only enhances security but also provides a financial benefit, making it highly attractive to the market. The impact is significant, as it improves fraud detection accuracy, reduces false positives, and supports regulatory compliance, thereby protecting customers and bolstering institutional trust.


# Feasibility: 
The feasibility of our fraud detection project is high, leveraging advanced machine learning models and comprehensive datasets to identify fraudulent transactions effectively. With scalable integration into financial systems, it meets strong market demand for fraud prevention. The unique selling proposition of earning commissions on saved frauds enhances its attractiveness. Regulatory support for advanced fraud detection further boosts its feasibility, ensuring a secure and financially beneficial solution for financial institutions.


# Market Readiness / Practical Applicability
Our fraud detection project is market-ready and practically applicable due to several factors. The advanced machine learning models have been trained and tested on real-world datasets, demonstrating their effectiveness in identifying fraudulent transactions. The scalability of the solution allows seamless integration into existing financial systems, making it adaptable for various financial institutions. The unique selling proposition of earning commissions on confirmed and saved frauds provides a clear financial incentive for adoption, aligning with market demands for innovative fraud prevention methods. Additionally, the solution supports regulatory compliance, further enhancing its attractiveness to financial institutions. With strong market demand for effective fraud detection and prevention solutions, our project is well-positioned for successful deployment and wide-scale adoption, offering enhanced security and financial benefits to institutions and their customers.


# Conclusion:

* Overall Best Model: The Stacking Classifier achieved the highest accuracy (0.99610) and F1 score (0.99610), demonstrating superior performance in both detecting fraud and legitimate transactions.

* Precision and Recall: All models exhibited high precision and recall, with Random Forest and XGBoost showing particularly strong results. The precision and recall values indicate that the models are effectively distinguishing between fraud and legitimate transactions.

* ROC AUC Scores: The ROC AUC scores are very high for all models, suggesting excellent discriminatory power between fraud and non-fraud transactions. The Random Forest model had the highest ROC AUC score (0.9998).

* Bagging Classifier Performance: The Bagging Classifier demonstrated a strong performance with an accuracy of 0.99510 and an F1 score of 0.99512. Its precision of 0.99269 indicates a high rate of correctly identified legitimate transactions and an effective detection of fraud.

* Model Performance: While the Random Forest and Stacking Classifier models performed exceptionally well, the choice of model may depend on the specific needs of the application, such as interpretability or computational efficiency.

* Comparison with Other Models: While the Bagging Classifier performed exceptionally well, achieving high accuracy and F1 scores, the Stacking Classifier slightly outperformed it in terms of accuracy (0.99610) and F1 score (0.99610). However, the Bagging Classifier still represents a robust choice with very competitive metrics.


# Output Description:

The models were evaluated on a dataset consisting of 7,200 fraud transactions and 587,443 legitimate transactions. The metrics provided demonstrate the effectiveness of each model in accurately predicting fraud and legitimate transactions, with the Stacking Classifier emerging as the top performer. All models exhibit robust performance with high accuracy, F1 scores, and AUC scores, reflecting their ability to effectively handle the imbalanced nature of the dataset and deliver reliable fraud detection.
