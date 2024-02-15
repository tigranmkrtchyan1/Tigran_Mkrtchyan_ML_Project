# Tigran_Mkrtchyan_ML_Project
This project encompasses a range of machine learning techniques and applications. From predictive analytics to deep learning, we aim to explore various facets of machine learning and their practical implications. Our focus lies in not only advancing the field of AI but also in applying these advancements to make a tangible impact.

#Project Desctiption
The Fraud Detection in Payments project aims to develop and implement an advanced system capable of identifying and preventing fraudulent activities in payment transactions. Leveraging machine learning algorithms and data analytics techniques, the system will analyze various transaction parameters and patterns to detect anomalous behavior indicative of fraud. By continuously learning from historical data and adapting to evolving fraud tactics, the system seeks to enhance security and minimize financial losses for businesses and consumers alike.

**Goals**
The primary goal of the  project is to develop a robust machine learning algorithm capable of accurately detecting fraudulent transactions in payment datasets. The algorithm should minimize false positives (legitimate transactions misclassified as fraud) and false negatives (fraudulent transactions not detected), ensuring reliability and trust in the system. By automating fraud detection, the project aims to enhance the efficiency and security of financial operations, saving time and reducing losses due to fraud.

**Data**
The dataset that was provided appears to contain transactional information with 100,000 rows, each representing a payment transaction. The data includes the following attributes:

**step**: presumably a time indicator of the transaction.
**type**: the type of transaction (e.g., PAYMENT, TRANSFER, CASH_OUT).
**amount**: the amount of money involved in the transaction.
**nameOrig**: the identifier for the origin account.
**oldbalanceOrg** and newbalanceOrig: the original account balance before and after the transaction.
**nameDest**: the identifier for the destination account.
**oldbalanceDest** and newbalanceDest: the destination account balance before and after the transaction.
**isFraud**: a label indicating whether the transaction is fraudulent.
**isFlaggedFraud**: a flag that indicates whether the transaction was marked as fraudulent.
This data will be essential in training and testing the machine learning model to recognize patterns and anomalies that may indicate fraudulent activities.

**Analysis**
The analysis will involve several stages using machine learning methodologies:

1. **Data Preprocessing**: Cleaning the data, handling missing values, encoding categorical variables (like type), and normalizing numerical features.
2. **Feature Engineering**: Creating new features that may help in detecting fraud, such as discrepancies in balance before and after a transaction, or the frequency of transactions in a certain period.
3. **Model Selection**: Choosing appropriate machine learning models for classification. This could include algorithms like Decision Trees, Random Forest, Gradient Boosting Machines, or Neural Networks.
4. **Model Training and Validation**: Using a portion of the data to train the models and a separate portion to validate their performance. Techniques like cross-validation may be used to ensure that the model generalizes well to unseen data.
5. **Performance Evaluation**: Evaluating the model using appropriate metrics, such as precision, recall, F1-score, and the ROC-AUC curve. Since the cost of false negatives (missed frauds) is usually higher than false positives, you might prioritize recall or use a cost-sensitive learning algorithm.

**Summary**

We began by cleaning a dataset involving financial transactions, addressing missing values and correcting data types. Post-cleaning, we prepared the data for machine learning by selecting features, encoding categorical variables, scaling numerical data, and splitting it into training and testing sets.

We then implemented and evaluated three machine learning models: Logistic Regression, K-Nearest Neighbors (KNN), and Decision Trees, focusing on detecting fraud (binary classification).

Logistic Regression: Achieved approximately 99.96% accuracy. While it showed high precision, its recall for fraud cases was notably low, indicating a significant number of missed fraud detections.

K-Nearest Neighbors: Also achieved high accuracy around 99.96%. It demonstrated a slightly better balance between precision and recall for fraud cases compared to logistic regression, but still underperformed in correctly identifying a significant portion of fraud cases.

Decision Trees: This model showed an accuracy of about 99.94%. It offered a better balance between precision and recall for fraud cases than the previous models, but still faced challenges in effectively identifying fraud cases.

In all models, the high accuracy was somewhat misleading due to the dataset's imbalanced nature, with a far greater number of non-fraud cases. The primary challenge was improving the recall for fraud cases without substantially reducing precision. The models were more effective in identifying non-fraud transactions but struggled with accurately detecting fraud cases, a common issue in imbalanced datasets. Future improvements could include more advanced resampling techniques, parameter tuning, or trying different algorithms to enhance fraud detection accuracy.




