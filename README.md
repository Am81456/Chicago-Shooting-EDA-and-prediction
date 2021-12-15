# Chicago-Shooting-EDA-and-prediction

PRESENTATION LINK - https://youtu.be/iPWfWE0zIL4



## an abstract/introduction

Gun violence and shooting has been a pressing issue in the United States for a while and has been happening more frequently. for this project, we will be using the Chicago open data source to do a program traning and have a better understanding of the factors in the Cities of Chicago. 

 
## exploratory data analysis
Index(['CASE_NUMBER', 'DATE', 'BLOCK', 'PRIMARY_TYPE', 'UNIQUE_ID', 'ZIP_CODE',
       'WARD', 'COMMUNITY_AREA', 'STREET OUTREACH ORGANIZATION', 'AREA',
       'DISTRICT', 'BEAT', 'AGE', 'SEX', 'RACE', 'FBI_CD', 'FBI_DESCR',
       'IUCR_CD', 'IUCR_SECONDARY', 'MONTH', 'DAY_OF_WEEK', 'HOUR', 'LATITUDE',
       'LONGITUDE', 'LOCATION'],
      dtype='object')
      
The Number of distinct crimes in City: 3

The Distinct Crimes are :
 ['FATAL SHOOTING' 'NON-FATAL SHOOTING' 'NON-SHOOTING HOMICIDE']
 

## data cleaning and feature engineering

Handling Missing Values
There are unknown values for many variables in the Data set. There are many ways to handle missing data.

Imbalanced Data set 
how to deal with the imbalanced data set I used Synthetic Minority Oversampling Technique to deal with class imbalance smote = SMOTE() 
source:https://www.analyticsvidhya.com/blog/2020/07/10-techniques-to-deal-with-class-imbalance-in-machine-learning/ 
Which helped with the fitting the  predictor and target variable x_smote, y_smote = smote.fit_resample(X, Y) and Stratifying  target variable 
  

## modeling
for this dataset, we will be using the random forest model and ADA Boost and compare which one has a higher accuracy and precision rate. 



## results and discussion

According to the EDA it shows that 2017 - 2019 had the highest crime activity in the five-year period. Throughout the 2016 - 2021 period, January & February had the highest crime activity and most recently November 2021. The months in 2020 with the highest crime activity are June & July.Throughout the 5-year period, these months recorded the highest crime activity


## conclusion/next steps 
Based on the analysis shown on the slides before, it shows that the random forest has a better result than ADA boost with both accuracy and precision 




references
** The source of the dataset is Data is extracted from the Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system.  Violence Reduction - Victims of Homicides and Non-Fatal ShootingsPublic from the Chicago Data portal
Source dataset link: https://data.cityofchicago.org/resource/gumc-mgzr.csv
** To deal with the imbalanced data set I used Synthetic Minority Oversampling Technique to deal with class imbalance smote = SMOTE() 
source:https://www.analyticsvidhya.com/blog/2020/07/10-techniques-to-deal-with-class-imbalance-in-machine-learning/. [Which helped with the fitting the  predictor and target variable x_smote, y_smote = smote.fit_resample(X, Y)



