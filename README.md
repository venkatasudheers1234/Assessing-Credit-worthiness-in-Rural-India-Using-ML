Assessing Credit worthiness in Rural India Using Machine Learning
# Problem Statement
Banks typically rely on credit scores to assess the creditworthiness of loan applicants. However, individuals who have never taken a loan lack a credit score, making it difficult for banks to evaluate their loan eligibility. This issue is particularly prevalent in rural India, where formal credit histories are often absent.
    
# Objective: 
The objective of the project is to develop a machine learning model that predicts the eligible loan amount for individuals without a prior credit score and to perform a descriptive analysis of the data features to understand the maximum repayment capability of customers, enabling banks to grant them the desired loan amount.

# Dataset
The dataset, sourced from Kaggle, contains various attributes including:
•   Personal Details: city, age, gender, social_class
•   Financial Details: primary_business, secondary_business, annual_income, monthly_expenses, old_dependents, young_dependents
•   House Details: home_ownership, type_of_house, occupants_count, house_area, sanitary_availability, water_availability
•   Loan Details: loan_purpose, loan_tenure, loan_installments, loan_amount (these contain loan details of loans that have been previously given, and which have been repaid)

# Solution Approach
Steps Followed for Building Machine Learning Model:

Step 1: Data Collection:
 Sourced the dataset from Kaggle containing personal, financial, and loan details of individuals from rural India.

Step 2:Data Preprocessing:

•	Handled missing values using mode for categorical features and mean for numerical features.
•	Performed one-hot encoding on categorical features (gender, type_of_house).
•	Transformed loan_purpose into binary features by encoding the top 10 most frequent categories, assigning 0 to less frequent categories.

Step 3: Descriptive Analysis:

•	Summarized the data using statistical measures such as mean, median, mode, standard deviation, and range.
•	Visualized distributions and relationships using histograms, bar charts, box plots, and correlation heatmaps.
•	Conducted feature analysis to detect outliers, analyze missing values, and understand correlations.

Step 4:Model Building and Evaluation:

•	Split the data into training and testing sets.
•	Trained a Random Forest Regressor model.
•	Evaluated model performance using metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).
 
 
# Code Execution Steps:
•   Two python scripts files are present: EDA and Model creation.ipynb and ModelCreation_properCoding_documentation.py.
•   EDA and Model creation.ipynb files has all EDA and Model creation scripts.
•   ModelCreation_properCoding_documentation.py: I have followed object oriented programming approach for creating model.For this usecase,Random Forest gives best accuracy as 86.6%.
