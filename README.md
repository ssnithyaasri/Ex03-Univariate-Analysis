# Ex03-Univariate-Analysis
## AIM
To perform Univariate EDA on the given data set.

Explanation
Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

## ALGORITHM

STEP 1
Import the built libraries required to perform EDA and outlier removal.

STEP 2

Read the given csv file

STEP 3

Convert the file into a dataframe and get information of the data.

STEP 4

Return the objects containing counts of unique values using (value_counts()).

STEP 5

Plot the counts in the form of Histogram or Bar Graph.

STEP 6
Use seaborn the bar graph comparison of data can be viewed.

STEP 7

Save the final data set into the file

## CODE 1

Name : Nithyaa sri S S
Register Number : 212222230100

**Univariate EDA - SuperStore.csv**
import pandas as pd
import numpy as np
import seaborn as snb
df = pd.read_csv('/content/SuperStore.csv')
df.head(10)
df.info()
df.describe()
df.dtypes
df.isnull().sum()
df['Postal Code'] = df["Postal Code"].fillna(df['Postal Code'].mode()[0])
df.isnull().sum()
df['Postal Code'].value_counts()
snb.boxplot(x="Sales",data=df)
snb.countplot(x="Sales",data=df)
snb.distplot(df["Sales"])
snb.histplot(x="Sales",data=df)
df.skew()
df.kurtosis()
snb.histplot(x="Postal Code",data=df)
snb.displot(x="Postal Code",data=df)
snb.boxplot(x="Postal Code",data=df)
snb.boxplot(x="Row ID",data=df)
snb.histplot(x="Ship Mode",data=df)
snb.countplot(x="Category",data=df)

## OUTPUT

EDA - SuperStore.csv

![UNI 1](https://user-images.githubusercontent.com/119122478/228436429-57003182-c474-4578-980c-2363e209d52d.png)

## Displaying information about Dataset

![image](https://user-images.githubusercontent.com/119122478/228436769-8a16f4f0-6d50-4a5c-b2a7-6aa7d56ff488.png)

![image](https://user-images.githubusercontent.com/119122478/228436901-8599b7cf-0ba5-4e8b-beca-cb3c362df634.png)

![image](https://user-images.githubusercontent.com/119122478/228437036-6403fae3-e2a5-424f-bb9f-872bb4226d36.png)

## Finding null values and cleaning it

![image](https://user-images.githubusercontent.com/119122478/228437285-1b879e77-ec6a-4d96-919f-5d5bc2a79989.png)


## Value counts of "Postal Code"

![image](https://user-images.githubusercontent.com/119122478/228437541-b1b069d2-35e7-4c6b-8c74-9dec984f6135.png)

## Distribution of Data

![image](https://user-images.githubusercontent.com/119122478/228437735-26ac46b9-6a67-4319-93d9-69b50e454615.png)
 
 ## Univariate Analysis
 
 ![image](https://user-images.githubusercontent.com/119122478/228438074-a9591548-0fae-4789-b85d-41764e046975.png)
 ![image](https://user-images.githubusercontent.com/119122478/228438211-7a8dadfc-1691-47cc-ae82-4cd3a3441bd7.png)
 ![image](https://user-images.githubusercontent.com/119122478/228443477-6e838fbe-dc39-4523-a4c1-2c20b27e1d43.png)
![image](https://user-images.githubusercontent.com/119122478/228439107-a57ba806-7fe7-415d-8774-53606aa469c0.png)
![image](https://user-images.githubusercontent.com/119122478/228440430-0e554358-0d9b-4603-b5fb-08b4b0dc1b28.png)

## CODE 2

import pandas as pd
import seaborn as sns
df1=pd.read_csv("diabetes.csv")
print(df1)
df1.info()
df1.dtypes
df1.skew()
df1.describe()
sns.boxplot(x='Glucose',data=df1)
sns.countplot(x="Glucose",data=df1)
sns.displot(df1["Glucose"]) 
sns.histplot(x="Glucose",data=df1)
df1.skew()
df1.kurtosis()
sns.boxplot(x="Insulin",data=df1)

## EDA - diabetes.csv

![image](https://user-images.githubusercontent.com/119122478/228440854-fb46a18a-04c7-4c17-ace4-4acbac0eaf37.png)

## Displaying information about Dataset

![image](https://user-images.githubusercontent.com/119122478/228441057-47a66a86-3d87-421a-a733-b42922f65edf.png)
![image](https://user-images.githubusercontent.com/119122478/228441163-d2d4593c-93d3-4eff-a3bd-028fe80eddba.png)
![image](https://user-images.githubusercontent.com/119122478/228441285-1785b768-0e81-400b-9209-e4444ae7c5f5.png)

## Univariate analysis

![image](https://user-images.githubusercontent.com/119122478/228441603-0c3b7cf9-ce59-4743-866e-be08426b971f.png)
![image](https://user-images.githubusercontent.com/119122478/228441797-c7c58d4e-ffb3-495a-9730-87885288eb85.png)
![image](https://user-images.githubusercontent.com/119122478/228441914-10efa759-ca14-4b75-8781-69655b257e38.png)

![image](https://user-images.githubusercontent.com/119122478/228442076-d2eff328-0294-4664-861c-e0c94af68b2c.png)
![image](https://user-images.githubusercontent.com/119122478/228442219-7f98bce6-a74d-47e9-889a-60df6db25248.png)
![image](https://user-images.githubusercontent.com/119122478/228442320-31bf21b2-dd6a-40ac-91c6-cce5e3da071e.png)

## Distribution of data
![image](https://user-images.githubusercontent.com/119122478/228442529-d7f6376e-df38-4752-ab4c-a93f5c6ea2b0.png)
![UNI 25](https://user-images.githubusercontent.com/119122478/228442728-6f843aa2-e931-4cf1-8f1b-90479c8d0bae.png)

## RESULT
Thus the program to perform EDA on the given data set is successfully executed.










 


