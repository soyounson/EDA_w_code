# 🦈 Global Shark Attacks data

Before modeling, data understand is the key part. Thus, we are going to do Exploratory Data Analysis (EDA) and trying to understand data fully. That is the main scope of the work. Let's follow the steps. 

For fun, the global shark attacks dataset has been considered in this work. 


<p align="center">
<img src="/images/shark.gif" width="450">
</p>



-----------------------------------------------------------------------

### ☾ Table of contents
- [x] Data acquisition
- [x] Dataset
- [ ] Preprocessing
- [ ] Data mining : EDA, correaltion matrix, visualization 
- [ ] Features engineering
-----------------------------------------------------------------------

### ☺︎ Data acquisition 

download data set from the kaggle link below 

🦆 [Kaggle data](https://www.kaggle.com/datasets/teajay/global-shark-attacks)
[Global shark attacks file](https://www.sharkattackfile.net/index.htm)


### ☺︎ Dataset

First, you read csv file and check all variables. 

```
df0 = pd.read_csv("attacks.csv",encoding = "ISO-8859-1")

#..... describe dataset 
print('================================================')
print(df0.describe)
print('================================================')
print('total size :',df0.shape)
```

#### ☻ Variables 

Total size of data is **25723 rows** and **24 columns**.




| Case Number |    Date    | Year |    Type    | country |   Area  | Location | Activity | Name | Sex | Age |        Injury       | Fatal (Y/N) | 
| ----------- | ---------- | ---- | ---------- | ------- | ------- | -------- | -------- | ---- | --- | --- | ------------------- | ----------- |
| 2018.05.26.a| 26-May-2018| 2018 | Unproviked |   USA   | Florida | Daytona  | Standing | male |  M  |  12 | Minor injury to foot|      N      |


| Time | Species | Investigator or Source| pdf | href formula | href | Case Number.1 | Case Number.2 | original order | Unnamed: 22 | Unnamed: 23 |       
| ---- | ------- | --------------------- | --- | ------------ | ---- | ------------- | ------------- | -------------- | ----------- | ----------- |
| 14h00|   nan   | K. McMurray, Tracking Sharks.com |2018.05.26.a-DaytonaBeach.pdf | http://sharkattackfile.net/spreadsheets/pdf_directory/2018.05.26.a-DaytonaBeach.pdf | http://sharkattackfile.net/spreadsheets/pdf_directory/2018.05.26.a-DaytonaBeach.pdf | 2018.05.26.a  | 2018.05.26.a | 6294 | nan | nan |


In details, it is necessary to understand all columns, contents, and values whether numerical or categorical.
       
- `Case Number` :  Date 
- `Date` : LITR, date when incident happended. 
- `Year` : LITR, year 
- `Type` : provoke, unprovoked, ... 
- `Country` 
- `Area` : area, espeically states in the USA 
- `Location` : exact location
- `Activity` : what kinda activities when they were attacked by sharks
- [delete] `Name` : name of victims 
- `Sex` : LITR, sex. Male or Female 
- `Age` : LITR, age 
- `Injury` : wounded parts in the attack
- `Fatal (Y/N)` : seriousness
- `Time` : Exact time or a time slot 
- `Species` : what kinda sharks 
- [delete] `Investigator or Source` : name who invested the incident 
- [delete] `pdf` : title of the investing file 
- [delete] `href formula` : directory of file 
- [delete, duplicate] `href` : same w/ href formula
- `Case Number.1` : Casenumber, same w/ date 
- [delete, duplicate] `Case Number.2` : same w/ Case Number.1
- [delete, duplicate]`original order` : order of incidents
- [delete] `Unnamed: 22` : all nan
- [delete] `Unnamed: 23`  : all nan


#### ☻ Issues 

There are several erors including missing values, duplication, noise, categorical values, mixing values etc. Thus, data cleaning and preprocessing are strongly required. Different approaches should be considered for data analysis.   

<p align="center">
<img src="/images/shark_Data_error.png" width="800">
</p>


-------------------------------------------------
### ☺︎ Preprocessing 

Before moving to EDA, preprocessing is required due to several issues 

#### ☻ Data cleaning 

#### ☻ Encoding 

categorical data -> numerical data 

### ☺︎ Data mining 


#### ☻ Data visualization 



#### ☻ Features correlation 



-----------------------------------------------------------------------

### ☻ Reference



### ☻ image sources
1. [Giphy](https://giphy.com/search/sesame-street)
