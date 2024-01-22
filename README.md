# Dry Bean Classification with Machine Learning

## Overview

Dry bean classification is pivotal in the agricultural industry, allowing farmers and researchers to accurately identify and categorize different types of beans. This project employs machine learning to create a robust multi-class classification system for dry beans. The journey involves comprehensive data analysis, feature engineering, and the implementation of machine learning models, including Quadratic Discriminative Analysis, Logistic Regression, and Gaussian Naïve Bayes. The models' performance is rigorously evaluated using metrics such as accuracy, F1 score, precision, and recall.

## Introduction

Dry beans, a fundamental self-pollinated legume consumed by millions worldwide, require efficient grading and classification. Traditional manual sorting is time-intensive, necessitating automated systems. Leveraging machine learning algorithms, especially computer vision systems, enables precise analysis of visual characteristics, contributing to quality control and adherence to international standards.

## Data Description

- **Dataset Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/602/dry+bean+dataset)
- **Attributes:** The dataset comprises 17 attributes, including area, perimeter, major and minor axis lengths, aspect ratio, eccentricity, and more.
- **Classes:** Seven different varieties of dry beans, namely Seker, Barbunya, Bombay, Cali, Dermosan, Horoz, and Sira.

## Methods

The project involves the systematic splitting of data into training and testing sets. The implemented machine learning algorithms encompass:
1. **Naïve Bayes:** Leveraging Gaussian Naïve Bayes for probabilistic classification.
2. **Logistic Regression:** Employing the one-vs-all method for multi-class classification.
3. **Quadratic Discriminative Analysis (QDA):** Utilizing QDA's ability to handle class-specific covariance matrices.

## Exploratory Data Analysis

- **Null Values:** Checked and appropriately handled.
- **Encoding:** Employed one-hot encoding and label encoding for categorical data.
- **Scaling and Normalization:** Ensured numerical feature uniformity through scaling.
- **Skew Distribution:** Analyzed and addressed skewed distributions.
- **Outliers:** Identified and effectively managed.
- **Feature Selection:** Removed columns with high correlation.
- **Visualizations:** Employed bar graphs, box plots, and pair plots for insightful data understanding.

## Results

### Naïve Bayes
- Initial Naïve Bayes: 48.33%
- Naïve Bayes + Dropping Columns: 41.25%
- Naïve Bayes + PCA: 42.28%
- Naïve Bayes + PCA + Dropping Columns: 37.5%

### Logistic Regression
- Logistic Regression: 90.52%

### Quadratic Discriminative Analysis (QDA)
- QDA: 90.76%

## Conclusion

QDA exhibited superior performance with an accuracy of 90.76%, surpassing Logistic Regression (90.52%). Naïve Bayes demonstrated a lower accuracy at 48.33%. The optimal model choice depends on specific problem requirements and evaluation metrics. QDA is preferred for accuracy, while Logistic Regression is suitable when class priors remain constant. The decision should align with the unique characteristics of the problem at hand.

