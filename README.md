# Heart-Disease-Prediction
Heart Disease Prediction System


# PROBLEM STATEMENT
* Cardiovascular diseases (CVDs) are the leading cause of death worldwide, responsible for an estimated 17.9 million deaths every year, accounting for 31% of all global deaths. Eight out of ten CVD-related deaths are caused by heart attacks and strokes, and a significant portion of these deaths occur prematurely in individuals under the age of 70.

* Early detection plays a critical role in preventing life-threatening events. People at high cardiovascular risk—due to conditions like hypertension, diabetes, high cholesterol, or previously diagnosed heart disease—require timely assessment and intervention.

* This project aims to build a machine learning model that can accurately predict the presence of heart disease using 11 clinical and demographic features. Such a predictive system can support healthcare professionals by enabling early diagnosis, risk stratification, and improved patient outcomes.

  
📌 Project Description

Heart Disease Prediction is a Machine Learning project that predicts whether a patient is likely to have heart disease based on various medical attributes such as age, blood pressure, cholesterol level, chest pain type, heart rate, and other clinical parameters.

The objective of this project is to assist healthcare professionals in identifying high-risk patients at an early stage, enabling timely diagnosis and treatment. By leveraging machine learning algorithms, the system analyzes patient health records and predicts the presence of heart disease with high accuracy.

📊 Dataset Information

The dataset contains 180 patient records with 15 features.

Features
Feature	Description
patient_id	Unique patient identifier
slope_of_peak_exercise_st_segment	Slope of exercise ST segment
thal	Thalassemia test result
resting_blood_pressure	Resting blood pressure (mm Hg)
chest_pain_type	Type of chest pain
num_major_vessels	Number of major vessels colored by fluoroscopy
fasting_blood_sugar_gt_120_mg_per_dl	Fasting blood sugar > 120 mg/dl
resting_ekg_results	Resting ECG results
serum_cholesterol_mg_per_dl	Cholesterol level
oldpeak_eq_st_depression	ST depression induced by exercise
sex	Gender
age	Age of patient
max_heart_rate_achieved	Maximum heart rate achieved
exercise_induced_angina	Exercise-induced angina
heart_disease_present	Target variable (0 = No Disease, 1 = Disease)
Target Variable

heart_disease_present

0 → No Heart Disease
1 → Heart Disease Present
🎯 Project Objective

Develop a machine learning model capable of:

Predicting heart disease risk.
Assisting healthcare decision-making.
Reducing diagnosis time.
Improving preventive healthcare measures.
🛠 Technologies Used
Programming Language
Python
Libraries
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Machine Learning Algorithms
Logistic Regression
Random Forest Classifier
Decision Tree Classifier
XGBoost Classifier (Optional)
Development Environment
Jupyter Notebook
Google Colab
VS Code
🔧 Tools Used
Tool	Purpose
Jupyter Notebook	Model Development
Google Colab	Cloud-based Training
GitHub	Version Control
Python	Programming
Scikit-learn	Machine Learning
Pandas	Data Processing
Matplotlib & Seaborn	Visualization
📈 Project Workflow
1. Data Collection
Load the heart disease dataset.
Understand feature descriptions.
Check dataset dimensions and data types.
2. Data Preprocessing
Remove unnecessary columns (patient_id).
Handle missing values.
Encode categorical features:
thal
chest_pain_type
Feature scaling if required.
3. Exploratory Data Analysis (EDA)
Analyze feature distributions.
Correlation analysis.
Visualize relationships between features and target variable.
Detect class imbalance.
4. Feature Engineering
Select important features.
Convert categorical variables into numerical format.
Normalize numerical features.
5. Model Building

Train multiple models:

Logistic Regression
Decision Tree
Random Forest
XGBoost
6. Model Evaluation

Evaluate using:

Accuracy Score
Precision
Recall
F1-Score
Confusion Matrix
ROC-AUC Score
7. Model Selection
Compare all models.
Choose the best-performing model based on evaluation metrics.
8. Prediction

The trained model predicts:

Heart Disease Present
No Heart Disease

for new patient records.

📊 Exploratory Data Analysis

Key analyses performed:

Age Distribution
Cholesterol Distribution
Blood Pressure Analysis
Heart Disease Frequency
Correlation Heatmap
Feature Importance Analysis

Example Insights:

Higher cholesterol levels may increase heart disease risk.
Older patients tend to show higher disease prevalence.
Exercise-induced angina is strongly associated with heart disease.

#⚠️ Important
The dataset was very small (180 rows) and imbalanced, which increases the chance of overfitting and reduces model generalization.

The data contained outliers, so Winsorization (capping) was used to reduce their impact while preserving important medical information.

After One-Hot Encoding, feature count increased, so SelectKBest was applied to choose the top 10 important features for better model performance.
# Model comparision Report 

Using K-Nearest Neighbors (KNN), we achieved the highest overall performance with 92% accuracy and the best F1 Score (0.909), making it the most effective model for predicting heart disease in this dataset.

SVM and XGBoost also achieved 92% accuracy with strong recall (1.0), but KNN outperformed them in precision and F1 Score, giving a better balance between false positives and false negatives.

Before tuning, Logistic Regression, SVM, and Decision Tree showed strong baseline performance (all around 92%), indicating the dataset is suitable for linear and non-linear models.

After tuning, KNN showed the most stable improvement across all metrics, demonstrating strong generalization on the small dataset.

Therefore, KNN was finalized as the best model for heart disease prediction due to its balanced accuracy, high recall, and superior F1 Score compared to other models.
## images 

<img src="Dashboard 1.png" width="800">
<img src="Dashboard 2.png" width="800">

## Result 
The machine learning model successfully predicts heart disease presence using patient medical records.

Achievements
Accurate classification of heart disease risk.
Identification of important health indicators.
Improved predictive healthcare analytics.
Supports early diagnosis and preventive treatment.

| Metric    | Value     |
| --------- | --------- |
| Accuracy  | 80% – 95% |
| Precision | High      |
| Recall    | High      |
| F1 Score  | Balanced  |

## 🚀 Future Improvements
Hyperparameter tuning using GridSearchCV.
Deploy using Flask or Streamlit.
Real-time patient prediction dashboard.
Integration with hospital management systems.
Deep Learning implementation using TensorFlow/Keras.
