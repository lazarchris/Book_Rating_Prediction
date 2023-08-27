<**Book Rating Prediction Project**

This repository contains a project focused on predicting the average rating of books based on various features present in the dataset. The goal of this study is to build models that can accurately predict book ratings using the provided attributes. The project involves data preprocessing, feature selection, regression and classification modeling, and an exploration of results.

**Table of Contents**
1. [Introduction](#introduction)
2. [Data Preprocessing](#data-preprocessing)
3. [Feature Selection](#feature-selection)
4. [Data Distribution and Imbalance](#data-distribution-and-imbalance)
5. [Data Augmentation with SMOGN](#data-augmentation-with-smogn)
6. [Regression and Classification Approaches](#regression-and-classification-approaches)
7. [Model Evaluation](#model-evaluation)
8. [Conclusion](#conclusion)
9. [Future Steps](#future-steps)
10. [GitHub Repository](#github-repository)

### Introduction
The main objective of this project is to predict the average rating of books using a dataset with 12 attributes, ranging from authors to publishers. The dataset was preprocessed to handle outliers, missing values, and categorical features.

### Data Preprocessing
Outliers and suspicious data points were removed, including instances with zero average ratings, unknown publication dates, and extreme values in attributes like number of pages and rating count. Categorical features were label encoded for model compatibility.

### Feature Selection
Exploratory data analysis revealed limited correlations between the features and the target variable. The highest observed correlation was just 0.17, indicating that feature selection and engineering were necessary. Some redundant features were dropped to improve model efficiency.

### Data Distribution and Imbalance
The distribution of average ratings exhibited a Gaussian pattern, with a concentration between ratings 3 and 4. This distribution imbalance could affect model performance by favoring the majority class.

### Data Augmentation with SMOGN
To address the class imbalance issue, Synthetic Minority Over-sampling Technique (SMOGN) was employed to augment the minority class. This aimed to enhance the learning of the algorithm on the less represented class.

### Regression and Classification Approaches
Both regression and classification approaches were explored. For regression, metrics like Mean Squared Error (MSE), Mean Absolute Percentage Error (MAPE), and R-squared were used. The classification task involved binning ratings into categories like bad, good, and excellent.

### Model Evaluation
Despite the low correlation observed between features and the target variable, models were built and evaluated. The results indicated moderate performance. Regression models showed low MSE and MAPE due to the limited rating range (0 to 5), but R-squared was notably low. Classification achieved better results, with an accuracy score of 0.603 using the Random Forest Classifier.

### Conclusion
In this project, we addressed the challenge of predicting book ratings by approaching it as both a regression and classification problem. Although the feature-target correlation was limited, the models showed promising results. Classification outperformed regression, which suggests that incorporating additional features like book price and sales could lead to better predictions.

### Future Steps
To enhance prediction accuracy, several avenues can be explored:
- Incorporate additional features like book price, sales data, and user reviews.
- Experiment with different regression and classification algorithms.
- Utilize more advanced techniques for feature selection and engineering.
- Investigate ensemble methods to combine predictions from multiple models.

### GitHub Repository
The code and materials related to this project can be found in the [GitHub repository](https://github.com/lazarchris/Book_Rating_Prediction.git). Feel free to explore the code, datasets, and results.

For any questions or collaborations, please reach out to:
- Christy Lazar: [GitHub Profile](https://github.com/lazarchris)
- Shawna Roseaulin: [GitHub Profile](#)
- Neelam Patkar: [GitHub Profile](#)
- Chin Vergara: [GitHub Profile](#)
