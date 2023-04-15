# Airbnb Price Prediciton Model: Project Overview
For this project, I built a predictive regression model that estimates Airbnb prices in New York City. The objective of the project is to showcase the skills related to data preprocessing, exploratory data analysis and multiple regression model building and tuning.

## Code and Resources Used
**Python version**: 3.10.9 <br>
**Packages**: numpy, pandas, matplotlib, sklearn, seaborn, warning, scipy. <br>
**Dataset Source**: http://insideairbnb.com/get-the-data

## Dataset Characteristics
The dataset that I downloaded from the Inside Airbnb website contains information regarding various details and metrics of a Airbnb listings in New Yowk City. After converting it to a Pandas data frame, it contains 42 931 rows and 18 columns:
1. id
2. name
3. host_id
4. host_name
5. neighbourhood_group
6. neighbourhood
7. latitude
8. longitude
9. room_type 
10. **price**
11. minimum_nights 
12. number_of_reviews
13. last_review
14. reviews_per_month
15. calculated_host_listings_count
16. availability_365
17. number_of_reviews_ltm 
18. license

## Data Cleaning
First step was to clean up the data so it was usable for our model. I made the following changes:
*	Dropped unnecessary columns
*	Removed the NaN values from the dataset
*	Removed all '0' values from the 'price' column
*	Removed outliers from the target variable using logarithm transformation

## EDA
In order to gain insights into the variables, I performed exploratory data analysis, and namely:
* Examined correlation between numerical variables
* Examined values counts for the categrical variables
* Performed analysis of variance (ANOVA)
* Visualized variables to look at distribution of the data, values counts and proportions

Below are a few highlights from EDA:
![alt text](https://github.com/dabykov/Projects/blob/main/project-2/neighbourhoods.png "Neighbourhood")
![alt text](https://github.com/dabykov/Projects/blob/main/project-2/neighbourhood_groups_map.png "Neighbourhood Groups")
![alt text](https://github.com/dabykov/Projects/blob/main/project-2/price%20distribution.png "Price Distribution")
![alt text](https://github.com/dabykov/Projects/blob/main/project-2/room%20type.png "Room Type")

## Feature engineering
After thoroughly analyzing the variables, I changed and engineered some features making a few changes, namely:
* Dropped the columns that didn't affect the target variable
* One-hot encoded the 'neighbourhood' variable and then applied PCA
* Scaled some features

## Model building
I tried three different models and evaluated them using Root Mean Squared Error and R-squared metrics. I chose RMSE because it is relatively easy and intuitive to interpret, and it punishes large prediction errors.

*	**Random Forest Regression** – Because it deals great with sparse data from categorical variables and also is able to capture non-linear relationships between input features and output variable
*	**Gradient Boosting Regression** – Because of the same reasons as for RFR, but it uses different (sequential) approach.
*	**KNN regression** – Because it is easy to interpret and it works well with a low-dimensional data.

## Model performance
The Random Forest model far outperformed the other approaches on the test and validation sets. 
*	**Random Forest regression** : R-squared = 99.9%
*	**Gradient Boosting Regression**: R-squared = 99.9%
*	**KNN Regression**: R-squared = 94.3%
