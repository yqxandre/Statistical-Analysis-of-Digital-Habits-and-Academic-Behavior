# Statistical Analysis of Digital Habits and Academic Behavior

## Overview

This project investigates the relationship between students' digital habits, academic behaviours, lifestyle factors, and productivity using a dataset of 20,000 student records.

The initial objective was to examine how digital habits, such as phone usage, social media, and gaming, relate to academic productivity. However, exploratory data analysis revealed unusual distributional patterns and a perfect \(R^2\) in the initial Ordinary Least Squares (OLS) regression model. This prompted a shift in focus towards investigating the dataset's underlying data-generating process and its implications for statistical inference.

## Objectives

- Investigate the relationships between digital habits, lifestyle factors, and student productivity.
- Develop and refine regression models to examine the predictors of productivity.
- Evaluate regression assumptions using model diagnostics.
- Apply regularization and variable selection to identify key predictors.
- Investigate potential synthetic data generation and assess its implications for interpreting statistical results.

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Examined dataset structure, descriptive statistics, and missing values.
- Visualised variable distributions using histograms and boxplots.
- Investigated relationships between variables using correlation analysis.
- Identified unusual distributional patterns that raised concerns about the dataset's underlying structure.

### 2. Ordinary Least Squares (OLS) Regression
- Estimated a baseline multiple regression model to examine the relationships between predictors and productivity score.
- Evaluated variable significance and model fit.
- Refined the model by considering potential reverse causality, endogeneity, and the theoretical relationships between variables.

### 3. Model Diagnostics
- Examined residual plots to assess linearity and homoscedasticity.
- Evaluated residual normality using graphical diagnostics.
- Used Variance Inflation Factors (VIF) to investigate multicollinearity.

### 4. LASSO Regularization
- Applied LASSO regression to perform automated variable selection.
- Used 10-fold cross-validation to select the regularization parameter.
- Compared the selected predictors against the OLS results.

## Key Findings

- **Unusual data structure:** Many predictors exhibited uniform distributions and bounded ranges. Combined with a perfect \(R^2\) in the initial OLS model, these patterns raised concerns that the dataset may have been synthetically generated.
- **Model refinement:** The initial model was refined by considering potential endogeneity and reverse causality, resulting in a more interpretable specification.
- **Key predictors:** LASSO retained six predictors: study hours per day, sleep hours, phone usage hours, stress level, attendance percentage, and focus score.
- **Limited evidence of real-world generalisability:** Although the models identified strong internal relationships, the potential synthetic nature of the dataset limits the conclusions that can be drawn about real-world student behaviour.

## Limitations

- The dataset's potentially synthetic nature limits the generalisability of the findings to real-world student populations.
- Statistical associations do not necessarily establish causal relationships.
- High model fit may reflect the dataset's underlying construction rather than relationships that would hold in real-world settings.

## Tools & Techniques

- **Software:** RStudio
- **Statistical modelling:** Ordinary Least Squares (OLS), LASSO regression
- **Model evaluation:** Residual analysis, normality diagnostics, Variance Inflation Factors (VIF)
- **Validation:** 10-fold cross-validation
- **Data analysis:** Exploratory data analysis and correlation analysis

## Repository Contents

The repository contains the analysis report, source code, and supporting materials used in the project.

## References

Dataset source: [https://www.kaggle.com/code/suyogverma/student-productivity-distraction-tradeoff]

