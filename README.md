# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file


# CODE

import pandas as pd
df=pd.read_csv("/content/Data_set.csv")
print(df)
df.head(10) 
df.info()
df.isnull() 
df.isnull().sum() 
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0]) 
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df['original_network']=df['original_network'].fillna(df['original_network'].mode()[0])
df.head() 
df['rating']=df['rating'].fillna(df['rating'].mean()) 
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()
df['watchers']=df['watchers'].fillna(df['watchers'].median()) 
df.head()
df.info() 
df.isnull().sum() import pandas as pd df=pd.read_csv("/content/Loan_data.csv") 
print(df)
df.head(10) 
df.info() 
df.isnull()
df.isnull().sum() 
df['Gender']=df['Gender'].fillna(df['Gender'].mode()[0]) 
df['Married']=df['Married'].fillna(df['Married'].mode()[0])
df['Education']=df['Education'].fillna(df['Education'].mode()[0]) df['Self_Employed']=df['Self_Employed'].fillna(df['Self_Employed'].mode()[0]) df['Property_Area']=df['Property_Area'].fillna(df['Property_Area'].mode()[0]) 
df['Loan_ID']=df['Loan_ID'].fillna(df['Loan_ID'].mode()[0]) df['Dependents']=df['Dependents'].fillna(df['Dependents'].mode()[0]) 
df.head() 
df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean()) df['CoapplicantIncome']=df['CoapplicantIncome'].fillna(df['CoapplicantIncome'].mean()) 
df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean()) df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean()) df.head() 
df['Credit_History']=df['Credit_History'].fillna(df['Credit_History'].median()) 
df.head() 
df.info() 
df.isnull().sum()

# OUPUT

[Expt1-Datascience.pdf](https://github.com/vijivini/Ex-01-Data-Cleaning/files/11147613/Expt1-Datascience.pdf)
