**Predicting Heart Disease Using Machine Learning Models**

**Introduction**

Heart disease remains a significant global health concern, requiring advanced methods for accurate prediction and early diagnosis. This study explores the application of various machine learning models for heart disease prediction using clinical data. The primary objective is to identify the most effective model for predicting heart disease based on accuracy and ROC-AUC scores.

**Data Collection and Preprocessing**

The dataset used in this study contains both numerical and categorical features related to heart disease risk factors. To prepare the data for modeling:

Missing values were filled using the mean for numerical columns and the mode for categorical columns.

Categorical variables were converted using one-hot encoding.

Numerical columns were scaled using MinMaxScaler.

**Class Imbalance Handling**

A class imbalance was observed in the target variable, 'Heart Disease Status.' The Synthetic Minority Over-sampling Technique (SMOTE) was applied to balance the classes, ensuring the models received balanced training data.

**Machine Learning Models Applied**

Five machine learning models were implemented and compared:

Logistic Regression

Decision Tree Classifier

Naive Bayes Classifier

Random Forest Classifier

Random Forest with Reduced Features

**Model Evaluation Metrics**

The models were evaluated based on:

Accuracy: Proportion of correctly classified instances.

ROC-AUC Score: Area under the ROC curve, measuring the ability to distinguish between classes.

Confusion Matrix: Visualization of true positive, true negative, false positive, and false negative predictions.

**Results**

Random Forest: Achieved the highest AUC score of 0.88 and was the best-performing model.

Logistic Regression: AUC score of 0.86, indicating strong performance close to Random Forest.

Naive Bayes: Moderate performance with an AUC score of 0.72.

Decision Tree: Performed the worst, with an AUC score of 0.58.

Random Forest with Reduced Features: AUC score dropped to 0.78, indicating slight performance degradation.

Feature Reduction Impact

Feature importance was assessed using the Random Forest model, and features with importance lower than 0.05 were removed. The model's performance slightly decreased after feature reduction, suggesting a need to retain certain variables for optimal performance.

**Conclusion**

Top Performing Models: Random Forest and Logistic Regression.

Weaker Models: Decision Tree performed the poorest, while Naive Bayes showed moderate performance.

Impact of Feature Reduction: Slight performance decline observed with reduced features.

**Recommendations**

Random Forest and Logistic Regression are recommended for heart disease prediction tasks due to their high AUC scores.

Further analysis can explore feature engineering and hyperparameter tuning to improve Decision Tree performance.

Consider explainability when selecting models for clinical use, balancing complexity with interpretability.

**Future Work**

Application of additional feature selection techniques.

Exploring ensemble methods and boosting techniques.

Testing the models on larger and more diverse datasets for generalizability.
