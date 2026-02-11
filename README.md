**Objective**

The objective of this project is to predict whether a customer will churn (Yes/No) using the Telco Customer Churn dataset.



**Dataset: Telco Customer Churn (Kaggle)**



The dataset contains customer demographic details, account information, service usage, and churn status.



 **Data Preprocessing**



Handled missing values



Encoded categorical variables



Removed unnecessary columns (e.g., customerID)



Converted target variable (Churn) into binary format



Train-test split performed using:



train\_test\_split(test\_size=0.2, random\_state=42, stratify=y)





Stratified split was used to preserve churn class distribution.



**Exploratory Data Analysis (EDA)**



Churn distribution analysis



Boxplots for numerical features



Correlation analysis



Outlier inspection



**Key observation:**

Customers with higher monthly charges and shorter tenure are more likely to churn.



 **Models Used**

&nbsp;Logistic Regression (Baseline Model)

Random Forest Classifier (Improved Model)



**Evaluation Metrics**



The following metrics were used:



Accuracy



Precision



Recall



F1-Score



**Confusion Matrix**



**Best Result**

&nbsp;Model                Accuracy  Recall (Churn=1)  F1 Score (Churn=1) 

&nbsp;Logistic Regression  0.81      0.56              0.61               

&nbsp;Random Forest        0.77      0.73              0.63               



Best model selected based on higher recall for churn class, since detecting churners is more important from a business perspective.



**Business Insight**

Although Random Forest had slightly lower overall accuracy, it achieved higher recall for churned customers. In a business context, identifying customers at risk of churn is more valuable than maximizing overall accuracy.



 **Conclusion**

Random Forest was selected as the final model due to its better performance in identifying churned customers.



