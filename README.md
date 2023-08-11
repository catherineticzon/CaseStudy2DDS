# Executive Summary of Case Study 2 

## Introduction  
The purpose of the case study is to:
  * Identify top 3 factors contributing to turnover
  * Explore and highlight any job-specific trends
  * Create a model to predict employee attrition
  * Create a model to predict employee monthly salary

In this repository, you will find:
  * A Rmd file with all the models, analysis, and supporting code
  * A presentation slide deck of the findings
  * A CSV file with the predicted employee attrition
  * A CSV file with the predicted employee monthly salary

Click <a href="http://catherineticzon.github.io">here</a> to find my GitHub webpage and navigate to the Projects tab to see my **projects and Rshiny apps.**   

## High-Level Trends 
Given the sample of 870 employees where attrition is known, the following trends were discovered during an exploratory data analysis:  

**Department**  
 * Sales department has a disproportionately higher percentage of attrition compared to the entire sample; sales makes up 42.1% of attrition cases but only 31.4% of entire sample 

**Job Roles**
  * Sales Representatives have a disproportionately higher attrition rate (17.1% but make up only 6.1% of total sample)
  * Research Directors and Manufacturing Directors have proportionately lower numbers of attrition when compared to the total sample

**Job Level**
 * Employees with job level = 1 make up the majority of attrition cases; 61.4% of attrition was of job level 1 employees, though job level 1 only makes up around 38% of the entire sample

**Environment Satisfaction**
 * Employees who had a value of 1 in environment satisfaction disproportionately made up the attrition cases; 20% of the entire sample had environment satisfaction = 1 but 30% of attrition had environment satisfaction = 1 


## Prediction Models  
### Predicting Attrition with knn 
To predict attrition, I used a knn model that had a sensitity of 62.27% and specificity of 60.98%. The model used the variables: years in current role, years since last promotion, age, and job level. When applied to the Attriton Competition dataset, the model predicted that 290 employees would **not** attrit and 10 employees **would attrit.**  The code for this model can be found in the Rmarkdown file of this repository (lines 780-816) and the dataset with the predicted attrition as well ("Case2PredictionsTiczon_Attrition.csv"). 


### Predicting Salary with linear regression 
To predict monthly income, I used a linear regression model that had an RMSE of 1414.96. The outcome variable used was monthly income and the predictor variable was job level. When I applied this model to the Salary Competition data set, the model predicted the monthly income of each of the 300 employees. The code for this model can be found in the Rmarkdown file of this repository (lines 869-900) and the dataset with the predicted monthly income as well ("Case2PredictionsTiczon_Salary.csv").  

