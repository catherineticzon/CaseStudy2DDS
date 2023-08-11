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

## Prediction Models  
### Predicting Attrition with knn 
To predict attrition, I used a knn model that had a sensitity of 62.27% and specificity of 60.98%. The model used the variables: years in current role, years since last promotion, age, and job level. When applied to the Attriton Competition dataset, the model predicted that 290 employees would **not** attrit and 10 employees **would attrit.**  
The code for this model can be found in the Rmarkdown file of this repository (ines 780-816) and the dataset with the predicted attrition as well ("Case2PredictionsTiczon_Attrition.csv"). 


### Predicting Salary 


