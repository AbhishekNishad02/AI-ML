Heart Disease Prediction using Machine Learning
This project builds a machine learning model to predict the likelihood of heart disease using patient medical data. The model is trained using a Random Forest Classifier with preprocessing and hyperparameter tuning.
Problem Statement
Heart disease is one of the leading causes of death worldwide. Early detection can improve treatment outcomes. Manual diagnosis can be time-consuming and error-prone. This project helps in predicting whether a patient has heart disease using data-driven techniques.
Solution Approach
The system uses a complete machine learning pipeline including data preprocessing, feature encoding, model training, hyperparameter tuning, and evaluation. Numerical features are scaled and categorical features are encoded before training the model.
Dataset
The dataset contains 918 records with features such as Age, Sex, Chest Pain Type, Resting Blood Pressure, Cholesterol, Fasting Blood Sugar, Resting ECG, Max Heart Rate, Exercise-Induced Angina, Oldpeak, ST Slope, and the target variable HeartDisease.
Technologies Used
Python, Pandas, NumPy, Scikit-learn, Jupyter Notebook or Google Colab.
Model
RandomForestClassifier with class balancing is used. Hyperparameter tuning is performed using GridSearchCV with 5-fold cross-validation. The best parameters are max_depth = 10, min_samples_leaf = 2, and n_estimators = 100.
Model Performance
The model achieves an accuracy of 89 percent and a ROC-AUC score of 0.93. The confusion matrix is [[69 13] [8 94]].
Feature Importance
Important features include ST_Slope, ChestPainType, Oldpeak, Cholesterol, and MaxHR, which have the highest impact on prediction.
Model Saving
The trained model is saved using pickle as heart_failure_model.pkl and can be used for future predictions.
Use Cases
This system can be used in hospitals, clinics, health monitoring systems, preventive healthcare tools, and medical research.
Future Improvements
The model can be improved by deploying it as a web application, integrating real-time data, using advanced models, and adding explainability tools.
Conclusion
This project shows how machine learning can help in early detection of heart disease and support better decision-making in healthcare.
