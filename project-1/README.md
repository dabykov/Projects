# Dataset Building by scraping Wikipedia: Project Overview
For this project, I . The objective of the project is to showcase the skills related to data collection, dataset building, data preprocessing, exploratory data analysis, and feature engineering.

## Code and Resources Used
**Python version**: 3.10.9 <br>
**Packages**: numpy, pandas, matplotlib, seaborn, warning, bs4, re, requests, json, csv, copy. <br>
**Dataset Source**: https://en.wikipedia.org/wiki/Classical_Hollywood_cinema
** Web Scraping article**: https://realpython.com/beautiful-soup-web-scraper-python/

## Dataset Characteristics
Initially, the dataset that I scraped from Wikipedia contained 194 rows and 84 columns, where the majority is almost fully empty. After data cleaning ans feature engineering, it now contains 194 rows and  columns:
 1. 
 2. 
 3. 
 4. 
 5. 
 6. 
 7. 
 8. 
 9. 
 10. 
 11. 
 12. 
 13. 
 14. 

## Data Cleaning
First step was to clean up the data so it was usable for our model. I made the following changes:
*	Dropped unnecessary columns
*	Label encoded the 'Gender' column

## EDA
In order to gain insights into the variables, I performed exploratory data analysis, and namely:
* Examined correlation between numerical variables
* Examined categorical variables
* Visualized variables to look at distribution of the data, values counts and proportions. Below are a few highlights from EDA:
![alt text]()
![alt text]()
![alt text]()
![alt text]()
