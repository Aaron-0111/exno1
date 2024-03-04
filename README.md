
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
## Data cleaning
### 1) Read and display DataFrame
```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/345c6c64-d291-49c0-810c-cab4f1fbf6b2)
### 2) Display head
```
df.head(4)
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/72282f14-3cb8-4576-a7fe-e8d9a2cc4188)
### 3) Display tail
```
df.tail(4)
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/596ccf54-d333-4b8f-bafc-f421949d2629)
### 4) Info of datafram
```
df.info(3)
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/ce5d2704-5a62-4442-baa7-9892873ee27f)
### 5) Describe about the dataframe
```
df.describe()
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/7eeb79dc-0974-431d-981b-03054525d64f)
### 6) Shape of the datafram
```
df.shape
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/7b143f48-594e-4724-8eeb-265f33f80135)
### 7) Checking tha NUll values
```
df.isnull().sum()
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/cbe916b2-bf76-4627-853d-0117cb26dc3b)
### 8) Drop the Null values
```
df.nunique()
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/c7b4ef70-687a-4aed-a6cf-f0fe1d98feec)
### 9) Finding the mean value
```
mn=df.TOTAL.mean()
mn
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/75712668-518a-4b4e-9207-1f92aeccd2a5)
### 10) Fill Null value with Mean value
```
df.TOTAL.fillna(mn,inplace=True)
df
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/253f8cbf-66f3-4d0e-ac71-7581e49e00b0)
### 11) Finding minimum value
```
mn=df.M4.min()
mn
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/54bdbddb-2245-4a66-91fb-619bc5d4dde8)
### 12) Printing only Date of Birth
```
df['cd']=pd.to_datetime(df['DOB'])
df['cd']
```
![image](https://github.com/Aaron-0111/exno1/assets/149347631/cb00101d-617b-4699-b5aa-f972aa72a3f8)
## Result:
Thus the program for data cleaning using python has executed successfully.
