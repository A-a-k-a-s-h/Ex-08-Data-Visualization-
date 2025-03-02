# Ex-07-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.

# CODE
```
/* 
Name : Aakash H
Register Number : 212220040002
**Data Visualization - Superstore.csv**
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sbn
df=pd.read_csv("/content/Superstore.csv", encoding = 'windows-1252')
df.head()
df.info()
df.isnull().sum()
sbn.countplot(x=df['Segment'],data=df)
plt.title("Number of Sales in Segment")
sbn.barplot(df['City'],df['Profit'])
plt.title("Number of Profit in Cities")
sbn.countplot(x=df['Ship Mode'],data=df)
plt.title("Number of profits in Ship Mode")
sbn.boxplot(df['Region'], df['Sales'])
plt.title("Sales of Product based on Region")
sbn.scatterplot(x=df['Sales'], y=df['Profit'])
sbn.scatterplot(df['Sales'],df['Profit'],hue=df['Segment'])
sbn.scatterplot(df['Sales'],df['City'],hue=df['Profit'])
sbn.scatterplot(df['Sales'],df['Profit'],hue=df['Ship Mode'])
sbn.scatterplot(df['Sales'],df['Profit'],hue=df['Region'])
*/
```
# OUPUT
## Data Visualization - Superstore.csv
![Data_Visualization](/images/img.png) 
![Data_Visualization](/images/img2.png)
![Data_Visualization](/images/img3.png)
![Data_Visualization](/images/img4.png)
![Data_Visualization](/images/img5.png)
![Data_Visualization](/images/img6.png)
![Data_Visualization](/images/img7.png)
![Data_Visualization](/images/img8.png)


# RESULT
Thus the Data Visualization for the given dataset had been executed successfully.
