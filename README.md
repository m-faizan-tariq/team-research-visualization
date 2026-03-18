# Team Research Visualization

## Overview

This project analyzes historical Bitcoin price data from 2019 to 2022 to investigate whether there is a significant correlation between opening and closing prices. The research addresses this question using statistical analysis and visualization techniques on cryptocurrency market data.

The study tests the null hypothesis that Bitcoin opening and closing prices are independent against the alternative hypothesis that a significant correlation exists between them.

## My Contribution

My contributions focused on data cleaning, which was a critical step to ensure data integrity and analysis reliability. I began by identifying null values in the key columns (Open and Close) and standardized their representation by replacing them with NA. Using the zoo package, I applied the na.approx() function for linear interpolation, filling missing values based on adjacent entries. This approach preserved the dataset continuity while minimizing potential biases. I re-verified the dataset after imputation to confirm no null values remained. I also calculated and shared summary statistics for the cleaned data to provide insights into its updated distribution.

My work complemented the efforts of the team. Muhammad Awais conducted detailed exploratory analysis, Muhammad Ahmed ensured environment setup and dataset validation, Udyanraje Bhosale created histograms and exponential decay curves, and Muhammad Hasnain explored relationships through scatter plots and regression.

## Methodology

The research followed these key steps:

- Data loading and preprocessing using R
- Null value identification and standardization to NA format
- Linear interpolation using zoo package to fill missing values
- Verification of data completeness after imputation
- Descriptive statistical analysis of opening and closing prices
- Distribution analysis using histogram visualization
- Exponential decay curve fitting to model price distribution
- Scatter plot analysis to examine Open vs Close relationship
- Spearman correlation testing to measure monotonic relationship

## Results

Key findings from the analysis:

- The dataset covers 3 years of historical Bitcoin price data from 2019 to 2022
- The research tested whether there is a significant correlation between Open and Close prices
- Histogram visualization revealed the distribution of closing prices
- Exponential decay curve was fitted to understand price spread patterns
- Spearman correlation was used as the statistical test due to non-normal distribution

## Tech Stack

- R
- zoo package for time series interpolation
- Base R graphics for visualization

## Files

- `teamResearch.R` - Main R script containing all data loading, preprocessing, analysis, and visualization code
- `Final report.pdf` - Complete project report with introduction, methodology, analysis, and conclusions
- `Muhammad Faizan Tariq Contributions.pdf` - Individual contribution summary
- `Bitcoin CZ.csv` - Dataset containing historical Bitcoin price data

## Author

Muhammad Faizan Tariq

- GitHub: https://github.com/m-faizan-tariq
- Portfolio: https://m-faizan-tariq.github.io/faizan-portfolio/
