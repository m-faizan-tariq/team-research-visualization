# Team Research Visualization

## Overview

This project analyzes historical Bitcoin price data from 2019 to 2022 to investigate the relationship between opening and closing prices. The main objective is to determine whether there is a statistically significant correlation between these two variables using exploratory data analysis, visualization, and non parametric statistical tests.

## My Contribution

My contributions focused on data cleaning and preparation, which were critical for ensuring data integrity and reliable analysis. I identified missing values in the key columns Open and Close, standardized them by replacing inconsistent entries with NA, and then used the zoo package and the na.approx function to perform linear interpolation based on adjacent values. This preserved the continuity of the time series while minimizing potential bias.

After imputation, I re checked the dataset to confirm that no null values remained and generated summary statistics to understand the updated distribution of the cleaned data. These steps provided a robust foundation for the teams subsequent visualization and modelling work.

My work complemented the efforts of the rest of the team. Muhammad Awais led the exploratory data analysis, Muhammad Ahmed handled environment setup and dataset validation, Udyanraje Bhosale developed visualizations including histograms and exponential decay curves, and Muhammad Hasnain investigated the relationship between Open and Close prices through scatter plots, regression, and correlation analysis.

## Methodology

The project followed these main steps:

- Load the historical Bitcoin dataset into R.
- Inspect and clean the data, focusing on missing values in Open and Close.
- Standardize missing values to NA and apply linear interpolation using the zoo package.
- Verify data completeness and generate descriptive statistics for key variables.
- Explore distributions using histograms and other plots.
- Model the distribution of prices using an exponential decay curve.
- Visualize the relationship between Open and Close prices with scatter plots and a fitted regression line.
- Use Spearman rank correlation to quantify the strength and direction of the relationship between Open and Close.

## Results

Key results from the analysis include:

- The dataset spans approximately three years of daily Bitcoin trading data from 2019 to 2022.
- After cleaning and interpolation, the data showed no remaining missing values in the Open and Close columns.
- Visual inspection of the scatter plot suggested a strong positive association between opening and closing prices.
- Because the closing price was not normally distributed, Spearman rank correlation was used instead of Pearson correlation.
- The Spearman correlation coefficient was very high and the associated p value was effectively zero, providing strong evidence of a statistically significant positive relationship between Open and Close prices.
- These findings indicate that the closing price tends to move in line with the opening price, which is relevant for understanding short term Bitcoin price behaviour.

## Tech Stack

- R
- zoo package for time series interpolation
- Base R graphics for visualizations

## Files

- `teamResearch.R` – Main R script containing data loading, cleaning, analysis, and visualization code.
- `Final report.pdf` – Full project report with background, methodology, analysis, and conclusions.
- `Muhammad Faizan Tariq Contributions.pdf` – Detailed summary of my individual contribution to the project.
- `Bitcoin CZ.csv` – Historical Bitcoin price dataset used in the analysis.

## Author

Muhammad Faizan Tariq  

- GitHub: https://github.com/m-faizan-tariq  
- Portfolio: https://m-faizan-tariq.github.io/faizan-portfolio/
