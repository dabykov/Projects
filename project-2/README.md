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

## Feature engineering

## Model building
