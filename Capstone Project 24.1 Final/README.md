# Capstone Project 24.1 Final Report

### Problem Statement
Diabetes is among the most prevalent chronic diseases in around the world, impacting millions of people each year and exerting a significant financial burden on the economy. Early diagnosis can lead to lifestyle changes and more effective treatment, making predictive models for diabetes risk important tools for public and public health officials. ###### (I am not only the promoter of solution but also a client as I am diabetic)

2.	# Model Outcomes or Predictions:
	
### Supervised Learning Models used
1) Random Forest  up to 84% achieved
2) Logsitical Regression up to 74% achieved
3) k-Nearest Neighbors (k-NN) up to ~~ 84% achieved (but slightly lesser compare to Random Forest)
   
### Unsupervised Learning Models used
   Dimensionality Reduction Models:
   Principal Component Analysis (PCA)

   Used combionation of Supervised with Unsupervised learning models
   Random Forest + PCA
   Logsitical Regression + PCA
   k-Nearest Neighbors (k-NN) + PCA

### Data Acquisition
I tried to get data from medical instiions but first I was required to have myself reguistered with instituin but as the same time it required a degree in medical field which was major challenge, therefore, I end up using Kaggle dataset. I used below

### Diabetes Health Indicators
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset

Dataset has columns (total 22 columns):
Dataset rows Count: 578,052

Below are importance features which are useful for classification between diabetic versus Non-diabetic person
     GenHlth 	- General health
     Age   
     BMI     	- Body Mass Index
     HighBP  	- High Blood pressure
     HighChol  - High Cholestrol

Data columns (total 22 columns):
Rows Count: 578,052

  
![image](https://github.com/user-attachments/assets/98f1f310-6b3a-48cd-ac51-fcbc269f1e77)

![image.png](attachment:4a01d6ee-abe8-4100-9a20-2154453dfb14.png)

8.	Data Preprocessing/Preparation: For this deliverable, you are tasked with detailing how you cleaned the data for your notebook.
9.	
a.	What techniques did you use to ensure your data was free of missing values, and inconsistencies? 
b.	How did you split the data into training and test sets?
c.	Please include any necessary analysis and encoding steps you took as well.
10.	Modeling: For this deliverable, please document your selection of machine learning algorithms that you selected for your problem statement from the first deliverable.
11.	Model Evaluation: Share your model evaluation here. What types of models did you consider for your problem (classification, regression, unsupervised)?  Articulate the evaluation metrics you used and how you determined which model was most optimal for your problem.


### Business understanding of the problem

Diabetes is among the most prevalent chronic diseases in the United States, impacting millions of Americans each year and exerting a significant financial burden on the economy. The scale of this problem is also important to recognize. The Centers for Disease Control and Prevention has indicated that as of 2018, 34.2 million Americans have diabetes and 88 million have prediabetes. Diabetes also places a massive burden on the economy, with diagnosed diabetes costs of roughly $327 billion dollars and total costs with undiagnosed diabetes and prediabetes approaching $400 billion dollars annually.

### Context

Diabetes is a serious chronic disease in which individuals lose the ability to effectively regulate levels of glucose in the blood, and can lead to reduced quality of life and life expectancy. After different foods are broken down into sugars during digestion, the sugars are then released into the bloodstream. This signals the pancreas to release insulin. Insulin helps enable cells within the body to use those sugars in the bloodstream for energy. Diabetes is generally characterized by either the body not making enough insulin or being unable to use the insulin that is made as effectively as needed. Complications like heart disease, vision loss, lower-limb amputation, and kidney disease are associated with chronically high levels of sugar remaining in the bloodstream for those with diabetes. While there is no cure for diabetes, strategies like losing weight, eating healthily, being active, and receiving medical treatments can mitigate the harms of this disease in many patients. Early diagnosis can lead to lifestyle changes and more effective treatment, making predictive models for diabetes risk important tools for public and public health officials. Furthermore, the CDC estimates that 1 in 5 diabetics, and roughly 8 in 10 prediabetics are unaware of their risk. While there are different types of diabetes, type II diabetes is the most common form and its prevalence varies by age, education, income, location, race, and other social determinants of health. Much of the burden of the disease falls on those of lower socioeconomic status as well.

### Content

The Behavioral Risk Factor Surveillance System (BRFSS) is a health-related telephone survey that is collected annually by the CDC. Each year, the survey collects responses from over 400,000 Americans on health-related risk behaviors, chronic health conditions, and the use of preventative services. It has been conducted every year since 1984. For this project, a csv of the dataset available on Kaggle for the year 2015 was used. This original dataset contains responses from 441,455 individuals and has 330 features. These features are either questions directly asked of participants, or calculated variables based on individual participant responses.

##### This dataset contains 3 files:

###### diabetes _ 012 _ health _ indicators _ BRFSS2015.csv 
Dataset of 253,680 survey responses to the CDC's BRFSS2015. The target variable Diabetes_012 has 3 classes. 0 is for no diabetes or only during pregnancy, 1 is for prediabetes, and 2 is for diabetes. There is class imbalance in this dataset. This dataset has 21 feature variables

###### diabetes _ binary _ 5050split _ health _ indicators _ BRFSS2015.csv
Dataset of 70,692 survey responses to the CDC's BRFSS2015. It has an equal 50-50 split of respondents with no diabetes and with either prediabetes or diabetes. The target variable Diabetes_binary has 2 classes. 0 is for no diabetes, and 1 is for prediabetes or diabetes. This dataset has 21 feature variables and is balanced.

###### diabetes _ binary _ health _ indicators _ BRFSS2015.csv
Dataset of 253,680 survey responses to the CDC's BRFSS2015. The target variable Diabetes_binary has 2 classes. 0 is for no diabetes, and 1 is for prediabetes or diabetes. This dataset has 21 feature variables and is not balanced.

###### BMI (Body Mass Index)
Below 18.5 Underweight 18.5 – 24.9 Normal weight 25.0 – 29.9 Overweight 30.0 and above Obese

###### GenHlth (General Health)
1: Excellent 2: Very Good 3: Good 4: Fair 5: Poor

###### HighBP (High Blood Pressure) & HighChol (Hiogh Cholestrol)
Majority of class 1 (diabetic cases) has high blood pressure & High choletrol



