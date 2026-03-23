# AI-ML
Heart Disease Prediction using Machine Learning
This project builds a machine learning model to predict the likelihood of heart disease using patient medical data. The model is trained using a Random Forest Classifier with proper preprocessing and hyperparameter tuning.
Problem Statement
Heart disease is one of the leading causes of death worldwide. Early detection can significantly improve treatment outcomes. However, manual diagnosis can be time-consuming and prone to error.
This project aims to:
Predict whether a patient has heart disease or not
Assist in early detection using data-driven insights
Reduce dependency on manual analysis
Solution Approach
The solution uses a complete machine learning pipeline:
Data preprocessing (scaling and encoding)
Feature engineering
Model training using Random Forest
Hyperparameter tuning using GridSearchCV
Model evaluation using multiple metrics
Dataset
The dataset contains 918 records with 12 features, including:
Age
Sex
Chest Pain Type
Resting Blood Pressure
Cholesterol
Fasting Blood Sugar
Resting ECG
Max Heart Rate
Exercise-Induced Angina
Oldpeak
ST Slope
Target: HeartDisease (0 = No, 1 = Yes)
Technologies Used
Python
Pandas
NumPy
Scikit-learn
Jupyter Notebook / Google Colab
Machine Learning Pipeline
1. Preprocessing
Numerical features are scaled using StandardScaler
Categorical features are encoded using OneHotEncoder
Combined using ColumnTransformer
2. Model
RandomForestClassifier with class balancing
3. Hyperparameter Tuning
GridSearchCV with 5-fold cross-validation
Optimized for ROC-AUC score
Best Parameters:
max_depth = 10
min_samples_leaf = 2
n_estimators = 100
Model Performance
Accuracy: 89%
ROC-AUC Score: 0.93
Classification Report
Precision: approximately 0.88–0.90
Recall: approximately 0.84–0.92
F1 Score: approximately 0.87–0.90
Confusion Matrix
[[69 13]
 [ 8 94]]
Feature Importance
Top contributing features:
ST_Slope
ChestPainType
Oldpeak
Cholesterol
MaxHR
These features have the highest impact on prediction.
Model Saving
The trained model is saved using pickle:
heart_failure_model.pkl
This model can be loaded and used for predictions in real-world applications.
Future Improvements
Deploy as a web application using Flask or Streamlit
Integrate with real-time hospital data
Use advanced models for improved accuracy
Add explainability tools such as SHAP or LIME
Use Cases
Hospitals and clinics
Health monitoring systems
Preventive healthcare tools
Medical research
Key Learnings
Building end-to-end machine learning pipelines
Handling mixed data types
Model tuning and evaluation
Applying machine learning to real-world problems
Conclusion
This project demonstrates how machine learning can assist in early detection of heart disease, helping healthcare professionals make faster and more accurate decisions.
