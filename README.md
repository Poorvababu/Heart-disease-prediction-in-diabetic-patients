The dataset used in this system for the prediction of heart disease using diabetes is created by integrating diabetes and heart disease datasets available in the Kaggle repository. Detailed description of the datasets is provided in Tables A.1, A.2 and A.3 which represents the Diabetes Health Indicators Dataset (DHID), Diabetes Prediction Dataset (DPD), and Logistic Regression to Predict Heart disease Dataset (LRPHD) datasets respectively. DHID is collected by the CDC (The Centres for Disease Control and Prevention) through BRFSS (The Behavioural Risk Factor Surveillance System), which is a telephone survey conducted annually in America. The dataset used has been split equally based on respondents with and without diabetes. It is a balanced dataset with 21 features and 70,692 responses. DPD is a diabetes prediction dataset created by collecting EHRs which contain clinical and demographic information from multiple healthcare providers and aggregating it into a single dataset. The data was collected through medical records, lab tests and surveys making it a dataset with 9 features and about 1 lakh responses. LRPHD is an ongoing cardiovascular study and results are obtained on the residents of Framingham, Massachusetts which contains 15 features and over 4000 responses.
Each feature is a potential demographic and behavioural risk factor. It is observed from these datasets that the attributes leading to diabetes and heart disease are very interrelated. Those features are blood pressure, glucose levels, cholesterol level, heart rate, lifestyle habits etc. From LRPHD, it is observed that Diabetes is an attribute to predict heart disease. Thus, we have curated a custom dataset to predict heart disease using diabetes as a parameter where the attributes common to diabetes and heart disease are retained and additional attributes contributing to diabetes are included in the dataset. Attributes retained from DHID dataset are DPD,HbA1c_level. Attributes such as blood and glucose level are the two parameters that are not present in DHID. So these two parameters are integrated to the DHID dataset along with other attributes such as age, sex, diabetes and, hypertension values. Similarly, the feature values contributing to the heart disease prediction from LRPHD dataset were analyzed and modified DHID such that the HeartDiseaseorAttack feature is used as the class label. Initially, DHID was evenly balanced for the class label diabetes with 50:50 ratio and the heart disease feature within the dataset was in the ratio 85 (no value):15(yes value). In addition, LRPHD to predict heart disease had the same ratios. So, the custom dataset is generated with 46 (no value):54 (yes value) ratio of diabetes feature to predict the heart disease with the samples of ratio 85 (no value): 15 (yes value) heart disease.

Custom dataset

Total	number	of instances in the dataset	70692 records
Number of features	19
After Feature selection	15
Class label balance	85% no heart disease, 15% heart disease

Following Datasets from Kaggle repository are merged as discused above:

https://www.kaggle.com/datasets/prosperchuks/health-dataset

https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

https://www.kaggle.com/datasets/dileep070/heart-disease-prediction-using-logistic-regression
