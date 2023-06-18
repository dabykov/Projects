# UFC Fighters Segmentation using K-means: Project Overview
For this project, I performed a clustering analysis breaking UFC fighters into different groups based on the characteristics available (besides the standard weight and gender grouping). The objective of this project is to showcase the skills related to unlabeled data preprocessing, exploratory data analysis, and applying unsupervised learning algorithms in order to perform data segmentation. 

## Code and Resources Used
**Python version**: 3.10.9 <br>
**Packages**: numpy, pandas, matplotlib, sklearn, seaborn, warning. <br>
**Dataset Source**: https://www.kaggle.com/datasets/axeltorbenson/ufc-roster-datastatistics

## Dataset Characteristics
The dataset that I downloaded from Kaggle (author:  Axel Torbenson) contains data related to the UFC fighter roster along with the official rankings of each fighter, general physical information (age, weight, and height), their UFC record, and total MMA record. The original data was gathered from Wikipedia and the UFC website. After converting it to a Pandas data frame, it contains 617 rows and 14 columns:
1. Ranking
2. Name
3. Age
4. Weight
5. Gender
6. Height
7. Ufc_wins
8. Ufc_loses
9. Ufc_draws
10. Ufc_no_contests
11. Mma_wins
12. Mma_loses
13. Mma_draws
14. Mma_no_contests

## Data Cleaning
The first step was to clean up the data so it was usable for our analysis. I made the following changes:
*	Inspected data
* Selected features
*	Handled NaN values

## EDA
In order to gain insights into the variables, I performed exploratory data analysis, namely:
* Examined the basic descriptive statistics
* Visualized frequency distributions of the chosen features
* Examined correlation between continuous numerical variables
* Performed analysis of variance (ANOVA)

## Preprocessing features
After analyzing the variables, I preprocessed and transformed some features, namely:
* Scaled and standardized features
* Performed principal component dimensionality reduction
* Defined the optimal number of clusters using the Elbow method.

## Model building
In order to form clusters from the preprocessed data, I applied an unsupervised machine learning algorithm K-means. Below are a few highlights from the clustering analysis:
![](https://github.com/dabykov/Projects/blob/main/project-4/Dashboard%204.png?raw=true)


## Profiling
Lastly, I evaluated the results and conducted the following cluster profiling:

#### Cluster 1:
- Young fighters
- UFC newcomers
- Mostly middle-weight, heavy-weight categories
- Tall fighters

#### Cluster 2:
- Highly experienced both in UFC and MMA
- Mostly fighters of mature age
- Weight categories vary significantly
- Mostly tall fighters

#### Cluster 3:
- Young fighters
- UFC newcomers
- Mostly light-weight, middle-weight categories
- Fighters of smaller height

#### Cluster 4:
- Very experienced in MMA, decent experience in UFC
- Mostly mature fighters
- Weight categories vary significantly
- Middle-height fighters
