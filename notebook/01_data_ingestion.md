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
- SeniorCitizen (int) (Note: the original data info is int64, and only include 2 values ie, 0 and 1. Should concider as categorical)
- tenure (int) (Note: original data info is int64, and include 73 unique values. Should concider as categorical)
- MonthlyCharges (float)
- TotalCharges (object) (Note: original object as String type, but need to convert to float. There's some missing data as value ' ' (blank space))

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

 - tenure 	:
	 - 1: 613, percentage: 0.09
	 - 34: 65, percentage: 0.01
	 - 2: 238, percentage: 0.03
	 - 45: 61, percentage: 0.01
	 - 8: 123, percentage: 0.02
	 - 22: 90, percentage: 0.01
	 - 10: 116, percentage: 0.02
	 - 28: 57, percentage: 0.01
	 - 62: 70, percentage: 0.01
	 - 13: 109, percentage: 0.02
	 - 16: 80, percentage: 0.01
	 - 58: 67, percentage: 0.01
	 - 49: 66, percentage: 0.01
	 - 25: 79, percentage: 0.01
	 - 69: 95, percentage: 0.01
	 - 52: 80, percentage: 0.01
	 - 71: 170, percentage: 0.02
	 - 21: 63, percentage: 0.01
	 - 12: 117, percentage: 0.02
	 - 30: 72, percentage: 0.01
	 - 47: 68, percentage: 0.01
	 - 72: 362, percentage: 0.05
	 - 17: 87, percentage: 0.01
	 - 27: 72, percentage: 0.01
	 - 5: 133, percentage: 0.02
	 - 46: 74, percentage: 0.01
	 - 11: 99, percentage: 0.01
	 - 70: 119, percentage: 0.02
	 - 63: 72, percentage: 0.01
	 - 43: 65, percentage: 0.01
	 - 15: 99, percentage: 0.01
	 - 60: 76, percentage: 0.01
	 - 18: 97, percentage: 0.01
	 - 66: 89, percentage: 0.01
	 - 9: 119, percentage: 0.02
	 - 3: 200, percentage: 0.03
	 - 31: 65, percentage: 0.01
	 - 50: 68, percentage: 0.01
	 - 64: 80, percentage: 0.01
	 - 56: 80, percentage: 0.01
	 - 7: 131, percentage: 0.02
	 - 42: 65, percentage: 0.01
	 - 35: 88, percentage: 0.01
	 - 48: 64, percentage: 0.01
	 - 29: 72, percentage: 0.01
	 - 65: 76, percentage: 0.01
	 - 38: 59, percentage: 0.01
	 - 68: 100, percentage: 0.01
	 - 32: 69, percentage: 0.01
	 - 55: 64, percentage: 0.01
	 - 37: 65, percentage: 0.01
	 - 36: 50, percentage: 0.01
	 - 41: 70, percentage: 0.01
	 - 6: 110, percentage: 0.02
	 - 4: 176, percentage: 0.02
	 - 33: 64, percentage: 0.01
	 - 67: 98, percentage: 0.01
	 - 23: 85, percentage: 0.01
	 - 57: 65, percentage: 0.01
	 - 61: 76, percentage: 0.01
	 - 14: 76, percentage: 0.01
	 - 20: 71, percentage: 0.01
	 - 53: 70, percentage: 0.01
	 - 40: 64, percentage: 0.01
	 - 59: 60, percentage: 0.01
	 - 24: 94, percentage: 0.01
	 - 44: 51, percentage: 0.01
	 - 19: 73, percentage: 0.01
	 - 54: 68, percentage: 0.01
	 - 51: 68, percentage: 0.01
	 - 26: 79, percentage: 0.01
	 - 0: 11, percentage: 0.0
	 - 39: 56, percentage: 0.01
