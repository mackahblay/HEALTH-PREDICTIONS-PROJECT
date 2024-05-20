# Healthcare-Project-w-Linear-Regresion

Date: 2024-04-29
Author: Melchizedek Ackah-Blay

## Overview
This project investigates the prediction of individual medical costs billed by health insurance using a multiple linear regression model. The study aims to identify key predictors of medical costs and quantify their impact on healthcare expenditure. This analysis is crucial for stakeholders such as health insurers, employers, policymakers, and healthcare providers who seek to manage and predict healthcare costs effectively.
Key Tasks and Activities

## Data Exploration and Cleaning:
- Data Import: Loaded a dataset consisting of 1338 observations and 7 variables from a CSV file.
- Data Cleaning: Ensured that the dataset was clean and prepared for analysis. Variables such as the number of children were treated as categorical to facilitate meaningful insights.

## Exploratory Data Analysis (EDA):
- Categorical Variables Analysis:
            Identified dominant trends, such as the prevalence of non-smokers (79.5%) and the distribution of individuals across different regions, with the Northwest and Southwest regions having the highest representation (24.3% each).
- Continuous Variables Analysis:
            Calculated key statistics such as the mean age (39.2 years) and mean BMI (30.66), highlighting the variability within the dataset.
            Analyzed medical costs, which had a mean of $13,270.42 with a significant standard deviation of $12,110.01, indicating a wide range of expenses.

## Data Visualization:
- Created boxplots and scatterplots to visualize relationships between variables and individual medical costs.
- Number of Children vs Medical Costs: Households with 0 and 4 children had higher median costs, while those with 5 children had the lowest costs.
- Smoking Status vs Medical Costs: Smokers incurred substantially higher medical costs compared to non-smokers.
- Region vs Medical Costs: The Northeast region had the highest median medical costs.
- Age vs Medical Costs: Positive correlation, indicating that costs increase with age.
- BMI vs Medical Costs: No clear correlation, but individuals with BMI over 30 showed greater variability in medical costs.

## Multiple Linear Regression Analysis:
- Developed a multiple linear regression model to predict medical costs based on variables such as age, BMI, sex, smoking status, number of children, and region.
  ### Model Results:
  Age: Each additional year increases medical costs by $256.9.
  BMI: Each unit increase in BMI increases costs by $339.2.
  Sex (Male): Being male is associated with a $131.3 decrease in costs compared to being female.
  Smoking: Smokers incur $23,848.5 more in costs compared to non-smokers.
  Number of Children: Each additional child increases costs by $475.5.
  Region: Compared to the Northeast, the Northwest, Southeast, and Southwest regions have lower costs by $353.0, $1035.0, and $960.0 respectively.

## Assessment of Regression Assumptions:
- Linearity: Residuals vs Fitted plot showed no clear pattern, suggesting the linearity assumption holds.
- Normality: Normal Q-Q plot indicated deviations from normality, especially in the upper tail.
- Homoscedasticity: Scale-Location plot suggested heteroscedasticity, indicating a violation of this assumption and potential bias in the model estimates.


## Conclusion

The analysis identified significant predictors of medical costs, such as smoking status, age, and BMI, which have substantial impacts on healthcare expenditures. However, the regression model assumptions, particularly normality and homoscedasticity, were violated, suggesting that further model refinement or alternative approaches might be necessary for more accurate predictions.

Future research could explore additional factors influencing medical costs, such as socioeconomic status and access to healthcare, and consider more sophisticated modeling techniques to address the violations of regression assumptions identified in this study. This could enhance the predictability and reliability of healthcare cost models, ultimately aiding stakeholders in managing healthcare resources more effectively.
