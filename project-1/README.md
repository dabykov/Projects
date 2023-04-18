# Data Collection and Analysis: Project Overview
For this project, I scraped a Wikipedia page in order to build a dataset that contains general information regarding major old Hollywood figures. The objective of the project is to showcase the skills related to data collection, data preprocessing, exploratory data analysis, and feature engineering.

## Code and Resources Used
**Python version**: 3.10.9 <br>
**Packages**: numpy, pandas, matplotlib, seaborn, warning, bs4, re, requests, json, csv, copy. <br>
**Dataset Source**: https://en.wikipedia.org/wiki/Classical_Hollywood_cinema <br>
**Web Scraping article**: https://realpython.com/beautiful-soup-web-scraper-python/

## Web Scraping
In order to collect the necessary data, I used BeautifulSoup library that helps to handle HTML code. The steps were the following:
1. First, I scraped the information contained in the infobox of a single random figure from the list. It also included building functions that perform initial clean up of the data.
2. I built a function for standardized infobox extraction.
3. I scraped through all the figures' infoboxes and created a list with the cquired information.

## Data Cleaning
Next step was to clean up the data so it was usable for oexploratory analysis. I made the following changes:
* Dropped unnecessary columns
* Engineered features and augmented data
* Normalized some columns
* Parsed and split up long strings
* Parsed and cleaned up extra commas and whitespaces
* Converted dates into datetime objects

## Dataset Characteristics
Initially, the dataset that I scraped from Wikipedia contained 196 rows and 84 columns, where the majority is almost fully empty. After data cleaning and feature engineering, it now contains 196 rows and 14 columns:

 1. Name       
 2. Full Birth Name      
 3. Birth Date
 4. Place of Birth       
 5. Died
 6. Death Place       
 7. Resting place        
 8. Children       
 9. Spouse/Spouses       
 10. Occupation/Occupations      
 11. Start career         
 12. End career       
 13. Birth Year        
 14. Death Year

## EDA
In order to gain some insights into the dataset, I performed exploratory data analysis, and namely:
* Examined numerical and categorical features
* Posed questions that seemed interesting to me and answered them
* Visualized some variables to look at proportions and distributions of the data, values counts and proportions. Here are few highlights from EDA:

![](https://github.com/dabykov/Projects/blob/main/project-2/Dashboard%202.png?raw=true)
