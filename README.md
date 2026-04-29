Hospital readmissions within 30 days


Hospital readmissions within 30 days after discharge are a critical concern for healthcare systems, as they increase costs, decrease the quality of care, and contribute to overcrowded hospitals. Predicting patients at high risk of readmission allows hospitals to intervene proactively and implement preventive measures, which in turn can improve patient outcomes and reduce unnecessary costs.

Data Science Problem Framing: The task at hand is a classification problem, where the goal is to predict whether a patient will be readmitted within 30 days after discharge based on various factors such as patient demographics, medical history, and treatment data. This problem can be approached as a binary classification, where the target variable is: 1 if the patient is readmitted within 30 days 0 if the patient is not readmitted

Success Metrics: Accuracy: Percentage of correct predictions (both true positives and true negatives). AUC (Area Under the ROC Curve): Measures the ability of the model to distinguish between the classes. Precision and Recall: Balances the trade-off between false positives and false negatives, especially important in healthcare contexts. F1-Score: A harmonic mean of Precision and Recall to provide a balanced measure. Cost Savings: The reduction in costs due to fewer readmissions, which could be tied to preventive interventions and better resource management. Business KPIs: Cost Savings: A reduction in the costs associated with unnecessary hospital readmissions. Uplift in Patient Outcomes: The improvement in patient health outcomes through targeted interventions and preventive care. Operational Efficiency: The ability of the hospital to better allocate resources based on predictions, improving overall healthcare delivery. Capstone Linkage: The outputs from this step will guide the subsequent steps (Capstone Steps 1–3), where the data will be explored, preprocessed, and modeled to build a predictive framework for readmissions.



Dataset

Source: https://www.kaggle.com/datasets/algozee/hospital-readmission-risk-prediction-2026?resource=download
~18,000 transactions
Cleaned 5209 records 
Features include 
 0   Age                             18000 non-null  int64  
 1   Gender                          18000 non-null  object 
 2   Insurance_Type                  18000 non-null  object 
 3   Socioeconomic_Risk_Score        18000 non-null  int64  
 4   Previous_Admissions_6M          18000 non-null  int64  
 5   Previous_Readmissions_1Y        18000 non-null  int64  
 6   Time_Since_Last_Discharge       18000 non-null  int64  
 7   Length_of_Stay                  18000 non-null  int64  
 8   Admission_Type                  18000 non-null  object 
 9   Primary_Diagnosis_Group         18000 non-null  object 
 10  Comorbidity_Index               18000 non-null  int64  
 11  Chronic_Disease_Count           18000 non-null  int64  
 12  ICU_Stay_Flag                   18000 non-null  int64  
 13  Severity_Score                  18000 non-null  int64  
 14  HbA1c_Level                     18000 non-null  float64
 15  Creatinine_Level                18000 non-null  float64
 16  Hemoglobin_Level                18000 non-null  float64
 17  Average_Systolic_BP             18000 non-null  int64  
 18  Number_of_Medications           18000 non-null  int64  
 19  Medication_Change_Count         18000 non-null  int64  
 20  High_Risk_Medication_Flag       18000 non-null  int64  
 21  Followup_Appointment_Scheduled  18000 non-null  int64  
 22  Discharge_Disposition           18000 non-null  object 
 23  Medication_Adherence_Score      18000 non-null  float64
 24  Readmitted_Within_30_Days       18000 non-null  int64  


How to Run

Clone the repository
Install dependencies: pip install -r requirements.txt

Run notebooks:
run Hospital Readmission Analysis.ipynb in google colab or JupyterLab

make sure data is included hospital_readmission_risk_dataset_2026_v1_18000rows.csv