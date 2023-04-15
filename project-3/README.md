# Airbnb Price Prediciton Model: Project Overview
For this project, I built a predictive classification model that estimates whether a certain bank customer is likely to churn. The objective of the project is to showcase the skills related to data preprocessing, exploratory data analysis, feature engineering and classification model building and tuning.

## Code and Resources Used
**Python version**: 3.10.9 <br>
**Packages**: numpy, pandas, matplotlib, sklearn, seaborn, warning, scipy, imblearn, copy. <br>
**Dataset Source**: https://www.kaggle.com/datasets/muratcakmak/churn-modelling-bank-customer

## Dataset Characteristics
The dataset that I downloaded from Kaggle (author: MURAT ÇAKMAK) contains open-source (or mock) bank customers data that can help predict the customers churn. After converting it to a Pandas data frame, it contains 10 000 rows and 14 columns:
 1. CustomerId
 2. Surname
 3. CreditScore
 4. Geography
 5. Gender
 6. Age
 7. Tenure
 8. Balance
 9. NumOfProducts
 10. HasCrCard
 11. IsActiveMember
 12. EstimatedSalary
 13. Exited
 14. RowNumber

## Data Cleaning
First step was to clean up the data so it was usable for our model. I made the following changes:
*	Dropped unnecessary columns
*	Label encoded the 'Gender' column

## EDA
In order to gain insights into the variables, I performed exploratory data analysis, and namely:
* Examined correlation between numerical variables
* Examined categorical variables
* Performed analysis of variance (ANOVA)
* Visualized variables to look at distribution of the data, values counts and proportions. Below are a few highlights from EDA:
![alt text](https://github.com/dabykov/Projects/blob/main/project-3/Correlation.png "Correlation")
![alt text](https://github.com/dabykov/Projects/blob/main/project-3/Age.png "Age Distribution")
![alt text](https://github.com/dabykov/Projects/blob/main/project-3/Country.png "Customers by Country")
![alt text](https://github.com/dabykov/Projects/blob/main/project-3/Exited.png "Exited Proprtion")

## Feature engineering
After thoroughly analyzing the variables, I changed and engineered some features making a few changes, namely:
* Dropped the columns that didn't affect the target variable
* One-hot encoded the categorical variable
* Scaled some features

## Model building
I tried seven different models and evaluated them using standard accuracy metric classification report. The models include:
*	**Logistic Regression** - Baseline model
*	**Random Forest Classifier**
*	**Gradient Boosting Classifier**
*	**KNN Classifier**
*	**Support Vector Machine Classifier**
*	**Gaussian Naive Bayes**
*	**Adaptive Boosting Classifier**

## Model performance
The three best performing models that were fed into the ensemble model are: 
* **Random Forest Classifier**: Accuracy on the testing set = 82.5%
* **KNN Classifier**: Accuracy = 81.1%
* **Gradient Boosting Classifier**: Accuracy = 82.4%

The **Ensemble Model** accuracy metric is 82.7%
