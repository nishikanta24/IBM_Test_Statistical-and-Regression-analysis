# Boston Housing Dataset Analysis

This project aims to explore and analyze the Boston Housing dataset. The analysis includes various descriptive statistics, visualizations, and statistical tests to answer key questions related to the housing market in Boston.

## Objective

**The primary goal of this project is to:**

- **Analyze** the distribution and characteristics of different variables in the dataset.
- **Use statistical tests** to answer questions about the relationships between key factors and the median value of homes.
- **Visualize the dataset** using different charts to gain insights into the variables.

## Dataset Overview

The Boston Housing dataset contains information about various factors influencing home values in Boston. The dataset consists of 506 observations and 14 variables:

- **CRIM**: Per capita crime rate by town
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq.ft.
- **INDUS**: Proportion of non-retail business acres per town
- **CHAS**: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- **NOX**: Nitric oxides concentration (parts per 10 million)
- **RM**: Average number of rooms per dwelling
- **AGE**: Proportion of owner-occupied units built prior to 1940
- **DIS**: Weighted distances to five Boston employment centers
- **RAD**: Index of accessibility to radial highways
- **TAX**: Full-value property-tax rate per $10,000
- **PTRATIO**: Pupil-teacher ratio by town
- **LSTAT**: % lower status of the population
- **MEDV**: Median value of owner-occupied homes in $1000's

## Task 1: Generate Descriptive Statistics and Visualizations

To get familiar with the dataset, we performed the following:

### 1. Boxplot of the Median Value of Homes (MEDV)
- **Objective**: To examine the distribution and potential outliers in the median value of homes.
- **Visualization**:  
  ![Boxplot of MEDV](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20201149.png)

### 2. Bar Plot for the Charles River (CHAS) Variable
- **Objective**: To show the distribution of homes bounded by the Charles River.
- **Visualization**:  
  ![Bar plot of Charles River](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20201357.png)

### 3. Boxplot of MEDV vs AGE (Discretized Age Groups)
- **Objective**: To understand how median home values differ across different age groups.
- **Visualization**:  
  ![Boxplot of MEDV by Age Group](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20210711.png)

### 4. Scatter Plot between NOX (Nitric Oxides) and INDUS (Non-Retail Business Acres)
- **Objective**: To explore the relationship between the concentration of nitrogen oxides and the proportion of non-retail business acres.
- **Visualization**:  
  ![Scatter Plot of NOX vs INDUS](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20210738.png)

- **Interpretation**: There is a positive correlation between the proportion of non-retail business acres and nitric oxides concentration.

### 5. Histogram for the Pupil-Teacher Ratio (PTRATIO)
- **Objective**: To visualize the distribution of the pupil-teacher ratio by town.
- **Visualization**:  
  ![Histogram of PTRATIO](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20210844.png)

## Task 2: Statistical Analysis

For the following questions, statistical tests were applied to derive conclusions:

### Problem Statement 1: **Is there a significant difference in the median value of houses bounded by the Charles River or not?**
- **Method**: T-test for Independent Samples
- **Conclusion**:  
  ![Result Image](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20210907.png)
- **Findings**: There is a significant difference in median house values between areas bounded by the Charles River and those not bounded.

### Problem Statement 2: **Is there a difference in median values of houses (MEDV) for each proportion of owner-occupied units built prior to 1940 (AGE)?**
- **Method**: ANOVA (Analysis of Variance)
- **Conclusion**:  
  ![Result Image](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20210925.png)
- **Findings**: There is a significant difference in median home values between the different age groups of houses.

### Problem Statement 3: **Can we conclude that there is no relationship between Nitric Oxide concentrations and the proportion of non-retail business acres per town?**
- **Method**: Pearson Correlation
- **Conclusion**:  
  ![Result Image](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20211547.png)
- **Findings**: There is a significant positive correlation between nitric oxides and non-retail business acres.

### Problem Statement 4: **What is the impact of an additional weighted distance to the five Boston employment centers on the median value of owner-occupied homes?**
- **Method**: Regression Analysis
- **Conclusion**:  
  ![Result Image](https://github.com/nishikanta24/Statistical-and-Regression-analysis/blob/main/pics/Screenshot%202024-11-09%20211605.png)
- **Findings**: For each additional weighted distance to employment centers, the median value of homes decreases by approximately $1.15k.

## Conclusion

This analysis provides valuable insights into the relationship between various factors and the median value of homes in Boston. Key findings include the significant differences in home values depending on proximity to the Charles River, the age of homes, and the correlation between business land use and pollution. Regression analysis also shows the negative impact of increasing distance from employment centers on home values.
