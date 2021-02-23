# Saudi Digital Academy
# Customer segmentation -  *Shaima Alharbi*  

## Setup:

- Libraries: 
   You will need to have numpy, pandas, seaborn,sklearn and matplotlib.

-  Data:
   the data set is from [Kaggle](https://www.kaggle.com/vetrirah/customer) and can be downloaded from this [repo](https://github.com/shaimaa122/Customer_segment/blob/main/Train.csv). 
   
- [Data Dictionary](https://github.com/shaimaa122/Customer_segment/blob/main/Customer%20Segmentation%20-%20Data%20Dictinory.pdf)

## Overview:
Customer segmentation is the practice of dividing a customer into groups of individuals that are similar As below fig, In this project ,I classify the customers into 4 segmentations(A,B,C,D).
![Customer segmentation](https://github.com/shaimaa122/Customer_segment/blob/main/Customer_segmintation.png)

## Process(Steps):
### 1- Exploratory Data Analysis(EDA):
Exploratory data analysis step is to identify missing data, explore data type, visualize the data before applying any       analysis to it, look at data distribution, mean and standard deviation, and etc.
F

   - The most of numbers of Male Customer 
### 2- Extract Featuures:
   - Categorical Features: 
      - Convert the binary columns into 0,1
      - Convert categorical variable into dummy/indicator variables.
   - Derived Features:
      - Add new Features to improve the score:
        `Age_range` - Classify the customers based on their age ( less than 30, less than 45, less than 60, more than 60)
### 3- Scaler:
        
### 4- Modelling:
   In this project, I split data then I use classfications models:
   - Baseline Model:
   - Logistic Regression:
   - Decision Tree Classifier
   - Random Forest Classifier 
   - KNN Classifier
   - SGD Classifier
   - Stacking Classifier

## Conclusion:
 
         
