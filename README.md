#  Pf-project
 - [DataSet From](#dataset-from)
 - [Library Used](#library-used)
 - [Functions Used](#function-used)
 - [Graph Types](#graph-types)

# Project About
## 1.Introduction
   - Briefly introduce the Pandas library.
   - Explain its importance in data analysis and manipulation.
   - State the purpose of your project (e.g., showcasing practical use cases of Pandas).
## 2.Overview of Pandas
   - Discuss its key features:
     - DataFrame and Series.
     - Handling missing data.
     - Powerful data wrangling capabilities.

## 3.Project Objectives
  - What do you aim to achieve with this project?
  - Examples:
    - Explore real-world datasets.
    - Data analysis using pandas function.
    - Perform data cleaning and preprocessing.

# DataSet From
## Data set Description
- Source
   - Dataset is sourced from tha Kaggle, a popular platform for datasets, 
     competitions, and machine learning projects.
   - ("Students Performance In Exams") in this way it apears on kaggle
- Link 
   - [Kaggle](https://www.kaggle.com/)
   - [kaggle DataSet](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
## OverView
- The dataset provides information about student performance in exam .<br> 
  It is particularly relevant for understanding students data, behavior, and  performance.
## Stucture Of Data Set
- In DataSet there is 1000 rows and 8 columns. 
## Data Quality
- The dataset had missing values in the Writing score,Maths score  and Reading score,which were handled during<br>  the data cleaning phase. Some duplicates were also identified and removed to ensure the integrity of the analysis.
# Library Used
- Pandas library
    - The Pandas library is widely used in Python for data analysis<br> and manipulation because of its powerful, flexible, and easy-to-use features. 
- For Installing 
    - library we use:  ("%pip install panda")
- PLotting Graph
    - For plotting graph we import:  ("matplotlib.pyplot as plt")
  
# Function used 
- Import library
- Cleaning data
    - Cleaning empty cells
    - Cleanung wrong format 
    - cleaning wrong data
    - Remove duplication
- Pandas Correlation
- Pandas Ploting
  
## Import Library
- For importing library we use two write: ("import pandas as pd") 
## Cleaning Data 
### Cleaning Empty cells 
- For cleaning empth cells we have two functions :
     - **Dropna( )** *( Removing the rows containing the empty or null values )*
     - **Fillna( )**  *( Adding the values in the empty cells )*
     - **inplace = True**   *( We use for showing the new dataset not the copy of the existing one )* 
### Cleaning Wrong Format
- For cleaning the wrong format we have two functions :
     - **pd.to_datetime([ ])** *( This will arrange the date columns into date )*
     -  **df.dropna( subset = 'Column name which have empty values or wrong data ', inpalce = True)** *( This will remove the whole row containing the wrong data or empty values)*
### Cleaning wrong data 
- For cleaning wrong data we have two functins :
    - **df.loc[index,'column name'] = the value we want to replace with** *( This will change the value of the given index )*
- By Applying some codition 
   - Using *if* and *for* 
### Remove Duplication 
- For removing duplication we have  functin :
    - **df.drop_duplicates(inplace = True )** *(This will remove the duplicate from the data set)*
- For finding the duplicate we use :
    - **df.duplicated()** *(This will show you in boolean expression how many dulications you have )*
  
## Pandas Correlation
- Correlation
   - A great aspect of the Pandas module is the **corr()** method.
   - The corr() method calculates the relationship between each column in your data set. 
- Code Run
   -** df.corr()** *( This will tell the cor relation btween two columns )*
- Types 
   - Perfect Correlation:
We can see that "Duration" and "Duration" got the number 1.000000, which makes sense, each column always has a perfect relationship with itself.

   - Good Correlation:
"Duration" and "Calories" got a 0.922721 correlation, which is a very good correlation, and we can predict that the longer you work out, the more calories you burn, and the other way around: if you burned a lot of calories, you probably had a long work out.

   - Bad Correlation:
"Duration" and "Maxpulse" got a 0.009403 correlation, which is a very bad correlation, meaning that we can not predict the max pulse by just looking at the duration of the work out, and vice versa.

# Graph Types
- For runing the code we should first have to import:
    - *import matplotlib.pyplot as plt*
- Kinds of Graph
  - *There are diffrent kinds of graph like :
  - *Hist* (df.plot(kind='hist'))
         plt.show()
  - *bar* (df.plot(kind='bar'))
         plt.show()
  - *line* (df.plot(kind='line'))
         plt.show() 
  - *pie* (df.plot(kind='pie'  y = 'give the column'))
         plt.show()
  - *area* (df.plot(kind='área'))
         plt.show()
  - *scatter* (df.plot(kind='scatter',x ='give the column ' y= 'give the column'))
         plt.show()