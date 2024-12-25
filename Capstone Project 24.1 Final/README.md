# Capstone Project 24.1 Final Report

#### Problem Statement
Diabetes is among the most prevalent chronic diseases in around the world, impacting millions of people each year and exerting a significant financial burden on the economy. Early diagnosis can lead to lifestyle changes and more effective treatment, making predictive models for diabetes risk important tools for public and public health officials. (I am not only the promoter of solution but also a client as I am also diabetic)

#### Data Acquisition
I tried to get data from medical instiions but first I was required to have myself reguistered with institution but as the same time it required a degree in medical field which was major challenge, therefore, I end up using Kaggle dataset. I used below

#### Diabetes Health Indicators

Has three data files. 

https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset

Dataset has columns (total 22 columns):
Dataset rows Count: 578,052 (consolidated data of three files)

Below are importance features which are useful for classification between diabetic versus Non-diabetic person
     GenHlth 	- General health
     Age   
     BMI     	- Body Mass Index
     HighBP  	- High Blood pressure
     HighChol  	- High Cholestrol

Data columns (total 22 columns):
Rows Count: 578,052

![image](https://github.com/user-attachments/assets/98f1f310-6b3a-48cd-ac51-fcbc269f1e77)

### Model Outcomes or Predictions:
	
#### Supervised Learning Models used

#### Evaluation:
1) Random Forest  up to 84% achieved
2) Logsitical Regression up to 74% achieved
3) k-Nearest Neighbors (k-NN) up to ~~ 84% achieved (but slightly lesser compare to Random Forest)

#### Data Preprocessing/Preparation:

- Combined all three files
  
- Ensured all three files same column name. Renamned After analysis of file "diabetes_012_health_indicators_BRFSS2015.csv" with three categories 0 = nondiabetec, 1 
  = Prediabetic 2 = Diabetic of column "'Diabetes_012".  it came out that prediabteic data didn't improved predict/classification, therfore, the decision made to 
  merging both categories  1 = Prediabetic & 2 = Diabetic
  
- Modified data of column `Diabetes_012`of file "diabetes_012_health_indicators_BRFSS2015.csv" to 0 = Non-diabetic and 1 = Diabetic
  
- Ensured all three files have same column names.

- Combined all three files

- Converted all columns data from float to Integer as Integers use less computer memory

- Dropped columns Income & Education as those doesn't contribute to classification of diabetic and non-

- Ensure duplicaplicate data is removed

- Balanced manority data
  
  Prior balance below were percentage 
	0    80.909992
	1    19.090008

  After balance below were percentage 
	0    50.0
	1    50.0

- Perform Standardization to ensure features uses same scale and mean and devaition
  
- Selected sample a manageable subset for analysis 10K sampels for faster process

  
#### Split of data for modeling

- Removed the column "Diabetic_binary" (Target column) from data to use for training data & Test data
- Split input feature data into Training and Test dataset ( two sets)
  Split output target data into Training and Test dataset ( two sets)

#### Reduce features by using PCA (Principal Component Analysis)

- Reduces input features in to 10 PCA

#### Run model

- Apply data with PCA into model

#### Data analysis and setting to optimization

- Analyze data with graphs
![image](https://github.com/user-attachments/assets/660a62f1-f040-4e8a-89ed-ea43dbc16c61)

#### Best model for the dataset

- Best model is Random Forest which gave up to 84% accuracy

#### Next step

- Need to root cuase and fix the issue which has been introduced after code optimzation which has resulted results down
