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

![Customer segmentation](https://github.com/shaimaa122/Customer_segment/blob/main/Customer_segmintation.png =100x20 )

## Process(Steps):
## 1- Exploratory Data Analysis(EDA):
Exploratory data analysis step is to data cleaning, explore data type, visualize the data, find the relation between the features and Segmentation(target), data distribution, mean and standard deviation, and etc, i figured:
   - Most of the customers are in D segmentation, Least of the customers are in B segmentation, The customers in A and C segmentations are close to each other.
   - Most of the customers are Male,The D segmentation contains the most Males & Female and the B segmentation contains the least Males & Female because the numbers of    Customers in D is more than in B
   - The most of customers have 1 year experience, and few customers have more than 10 years.
   - Most of the customers are Married, The `D` segmentation contains the most of unmarried customer, and the other segmentations (`A`,`B`,`C`) contains most of married special `C`.
   - The most Profession is Artist and the least Profession is Homemaker, The C , A and Bsegmentations contains most of the Artist, but The D segmentation contains most of the Healthcare.
   - The A and B segmentations that contains least of the Marketing, but The C and D segmentations contains least of the HomeMaker.
   - The most range of Customers between 20 - 45,The D The most range of Customers between 20 - 30, So contains the most of unmarried, The A The most range of Customers between 27 - 40, The B The most range of Customers between 30 - 50, The C The most range of Customers between 40 - 50, So contains the most of married.
   - Most of the customers have one year experience, and least of customers have more than 10 years experience.
   - Most of customers spending Low score and least of customers spending high, Most of D segmentation is spending Low, because their ages less than 30, Most of C segmentation is spending Average, , because their ages more than 40.
   - Most customers have Family size of 2 , Most of customers have  Family size of 9
   - The most of Customers Cat_6, The least of Customers in Cat_5 and Cat_1
 
  ![age by segmentation](https://github.com/shaimaa122/Customer_segment/blob/main/EDA/age%20by%20segmintaions.png)

**At the end of EDA:**
The A Segmentation:
contain the most of married Customers and spnding score is Low becouse thair age is less than 40 , and the Profession is Artists.
The B Segmentation:
contain the less number of customers and thair age more than 30 and less than 50, So most of customer is married.
The c Segmentation:
contain the most of married Customers and spnding score is Average becouse thair age is more than 45 , and the Profession is Artists.
The D Segmentation:
contain the most of unmarried Customers and spnding score is low Customers becouse thair age is less than 30 , and the Profession is Homemaker.

## 2- Extract Featuures:
   - Categorical Features: 
      - Convert the binary columns into 0,1
      - Convert categorical variable into dummy/indicator variables.
   - Derived Features:
      - Add new Features to improve the score:
        `Age_range` - Classify the customers based on their age ( less than 30, less than 45, less than 60, more than 60)
        
        
## 3- Modelling:
   In this project, I split data then I use classfications models: `Baseline Model` ,`Logistic Regression`,`Decision Tree Classifier`,
   `Random Forest Classifier `,  ` KNN Classifier`,  `SGD Classifier`, `Stacking Classifier`
### Compare Models
![Compare Models](https://github.com/shaimaa122/Customer_segment/blob/main/compare%20models%20with%20grid.png)

- To compare these models with the `Baseline Model`, I noticed that. Baseline showed the lowest accuracy with 0.28606.
- The classfications models with accuracy score : `Logistic Regression` is 0.50656,`Decision Tree Classifier` is 0.43505,
   `Random Forest Classifier ` is 0.4889,  ` KNN Classifier` is 0.47552,  `SGD Classifier` is 0.47663, `Stacking Classifier `is 0.5217, The best score compared by baseline is **Stacking model**
   
- At the end, The Stacking model after using GridSearchCV with best params is 0.52888 the acurrcy is increased.
  
 
 
         
