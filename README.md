# Customer Churn Prediction Project: Random Forest vs. Neural Network

This project aimed to develop a robust predictive model for customer churn, specifically within a credit card services context. The primary objective was to accurately identify customers at risk of attrition, enabling proactive retention strategies. The project involved a comprehensive workflow encompassing data cleaning, exploratory data analysis (EDA), feature engineering, model development, and performance evaluation.

## Data Preparation and EDA:
The initial phase focused on rigorous data cleaning and transformation. This involved handling missing values, addressing data inconsistencies, and standardizing data formats. Feature engineering was performed to derive meaningful insights from the raw data. Subsequently, EDA was carried out to understand the underlying patterns and relationships within the dataset. This included visualizing feature distributions, identifying correlations, and exploring the impact of various attributes on customer churn. The EDA revealed an imbalanced dataset, with significantly more non-churned customers than churned customers, necessitating careful consideration during model development.

## Model Development and Comparison: 
Two distinct machine learning methodologies were employed for churn prediction: Random Forest and a Neural Network.

Random Forest: This ensemble learning method constructs multiple decision trees and aggregates their predictions, offering robust performance and interpretability.
Neural Network: A deep learning approach capable of capturing complex, non-linear relationships within the data.
Both models were trained and evaluated using appropriate metrics, including accuracy, precision, recall, F1-score, and ROC-AUC.

## Results and Conclusion:

The comparative analysis of the Random Forest and Neural Network models revealed a clear performance advantage for the Random Forest in predicting customer churn. The Random Forest model achieved a higher accuracy of 96.20% compared to the Neural Network's 94.08%, demonstrating its superior ability to correctly classify customers. Notably, for the churn class, the Random Forest exhibited better precision, recall, and F1-score, with a precision of 0.88 and an F1-score of 0.88, surpassing the Neural Network's respective values of 0.80 and 0.82. Furthermore, the Random Forest's ROC-AUC score of 0.9888 was significantly higher than the Neural Network's 0.9730, indicating a greater capacity to distinguish between churned and non-churned customers. The confusion matrices further solidified this conclusion, showing fewer false positives and false negatives for the Random Forest model, implying more accurate classifications. These results strongly suggest that the Random Forest model is more reliable and effective for churn prediction in this context. The model highlighted the importance of 'total transaction amount' and 'total transaction count' in predicting churn. Strategies focused around these metrics would be highly effective for customer retention. Conversely, the Neural Network's lower performance was likely attributed to potential overfitting, suboptimal hyperparameter tuning, challenges in handling the imbalanced dataset, or insufficient training data.

## Further Research and Recommendations:

A key planned development is the creation of a user-friendly front-end interface. This interface will allow users to input customer data and receive a real-time prediction of the customer's churn probability, expressed as a percentage. This functionality will enable businesses to:

Segment Customers: Group customers based on their predicted churn risk, facilitating targeted interventions.
Personalized Strategies: Develop and implement personalized retention strategies tailored to specific customer segments, maximizing the effectiveness of retention efforts.
Proactive Intervention: Allow customer service and retention teams to act quickly on customers who have a high churn probability.
