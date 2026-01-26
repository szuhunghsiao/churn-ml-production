## Data Info
Data Source: Telco Customer Churn from Kaggle/IBM Sample data
Download time: 2026-01-11
Label Leakage: since it is from Kaggle for practice, there might be some leakage
Row: 7043  (Each row represents a single customer snapshot)
Col: 21  

## Columns list

Primary Key:  
- customerID  : unique 7043 value should be the primary key and unique for each row. There's no time related columns in the dataset

Numeric:
- SeniorCitizen (int) (Note: the original data info is int64, and only include 2 values ie, 0 and 1. Should concider as categorical. It is a binary indicator rather than a continuous numeric feature, and should be encoded accordingly without normalization.)
- tenure (int) (Note: original data info is int64, and include 73 unique values. However, even the number of unique value is much lower than 7043 (row number), it should still concider as numeric)
- MonthlyCharges (float)
- TotalCharges (object) (Note: original object as String type, but need to convert to float. There's some missing data as value ' ' (blank space). Missing values may correlate with short-tenure customers. This requires careful handling to avoid bias and will be addressed in data validation and feature engineering steps.)

Categorical:  
(Note 1: in multiple columns, they include "No internet servie" might have high relation with InternetService. Should investigate the correlation)  
(Note 2: in MultipleLines, "No phone service" is align with PhoneService's "No" which is not missing value and have strong correlation between those columns)
 - gender 	:
	 - Female: 3488, percentage: 0.5
	 - Male: 3555, percentage: 0.5

 - Partner 	:
	 - Yes: 3402, percentage: 0.48
	 - No: 3641, percentage: 0.52

 - Dependents 	:
	 - No: 4933, percentage: 0.7
	 - Yes: 2110, percentage: 0.3

 - PhoneService 	:
	 - No: 682, percentage: 0.1
	 - Yes: 6361, percentage: 0.9

 - MultipleLines 	: 
	 - No phone service: 682, percentage: 0.1
	 - No: 3390, percentage: 0.48
	 - Yes: 2971, percentage: 0.42

 - InternetService 	:
	 - DSL: 2421, percentage: 0.34
	 - Fiber optic: 3096, percentage: 0.44
	 - No: 1526, percentage: 0.22

 - OnlineSecurity 	:
	 - No: 3498, percentage: 0.5
	 - Yes: 2019, percentage: 0.29
	 - No internet service: 1526, percentage: 0.22

 - OnlineBackup 	:
	 - Yes: 2429, percentage: 0.34
	 - No: 3088, percentage: 0.44
	 - No internet service: 1526, percentage: 0.22

 - DeviceProtection 	:
	 - No: 3095, percentage: 0.44
	 - Yes: 2422, percentage: 0.34
	 - No internet service: 1526, percentage: 0.22

 - TechSupport 	:
	 - No: 3473, percentage: 0.49
	 - Yes: 2044, percentage: 0.29
	 - No internet service: 1526, percentage: 0.22

 - StreamingTV 	:
	 - No: 2810, percentage: 0.4
	 - Yes: 2707, percentage: 0.38
	 - No internet service: 1526, percentage: 0.22

 - StreamingMovies 	:
	 - No: 2785, percentage: 0.4
	 - Yes: 2732, percentage: 0.39
	 - No internet service: 1526, percentage: 0.22

 - Contract 	:
	 - Month-to-month: 3875, percentage: 0.55
	 - One year: 1473, percentage: 0.21
	 - Two year: 1695, percentage: 0.24

 - PaperlessBilling 	:
	 - Yes: 4171, percentage: 0.59
	 - No: 2872, percentage: 0.41

 - PaymentMethod 	:
	 - Electronic check: 2365, percentage: 0.34
	 - Mailed check: 1612, percentage: 0.23
	 - Bank transfer (automatic): 1544, percentage: 0.22
	 - Credit card (automatic): 1522, percentage: 0.22

 - Churn 	:
	 - No: 5174, percentage: 0.73
	 - Yes: 1869, percentage: 0.27

 - SeniorCitizen 	:
	 - 0: 5901, percentage: 0.84
	 - 1: 1142, percentage: 0.16
