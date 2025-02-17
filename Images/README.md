### Final Results:
- #### PCE Logistic Regression Model:
  - `PCE_metrics.png` - Table including model performance metrics `(F1 score, Accuracy, Sensitivity and Specificity)` for our logistic regression model using only the **pooled cohort equation (PCE)** variables.
  - `PCE_regression_coeffs.png` - Significant coefficient results from our logistic regression model using only **PCE** variables, indicating which feature variables which were significant in predicting our target variable: cardiovascular health outcomes. Almost all were found to be significant, except those related to taking blood pressure medication and diabetes status. 
  - `ROC_PCE.png` - ROC curve demonstrating model performance and optimal threshold for model using only the existing **PCE** variables. The area under the curve (AUC) is 0.814. Optimal threshold optimizing both sensitivity and specificity is identified to be 0.672.

- #### SDOH Logistic Regression Model:
  - `SDOH_metrics.png` - Table including model performance metrics `(F1 score, Accuracy, Sensitivity and Specificity)` for our logistic regression model using only **SDOH** variables.
  - `SDOH_regression_coeffs.png` - Significant coefficient results from our logistic regression model using **SDOH** variables, indicating which feature variables which were significant in predicting our target variable: cardiovascular health outcomes.
  - `SDOH_regression_coeffs_2.png` - Significant coefficient results from our logistic regression model using **SDOH** variables, indicating which feature variables which were significant in predicting our target variable: cardiovascular health outcomes. We found `Poverty Ratio` and `Food Security` to be significant coefficients. 
  - `SDOH_regression_coeffs_3.png` - Significant coefficient results from our logistic regression model using **SDOH** variables, indicating which feature variables which were significant in predicting our target variable: cardiovascular health outcomes. We found `Poverty Ratio` and `Food Security` to be significant coefficients.
  - `ROC_SDOH.png` - ROC curve demonstrating model performance and optimal threshold for model also using **SDOH** variables. The area under the curve (AUC) is 0.831, indicating our overall model performance is good and better than that of a random classifier. Interestingly, the area under the curve for this model is actually better than that of the model using only the existing PCE variables, which would indicate a more accurate model--but this is not 100 percent true when considering the other metrics.


### Box and Bar Plots by CVD Outcome/ASCVD Score for Various Feature Variables:
- `CVD_byAge.png` - Box plot demonstrating how **Age** distribution varies across our two cardiovascular health outcomes: `negative = 1` vs. `non-negative = 0`. Note that those who experienced a negative CVD event are generally older and above 60. The plot caps at 80 because that was the age limit in our dataset.
- `CVD_byPovertyRatio.png` - Box plot demonstrating how **Poverty Ratio** distribution varies across our two cardiovascular health outcomes: `negative = 1` vs. `non-negative = 0`. Note that our interquartile ranges and standard errors for median poverty ratio are overall lower for those who experienced a negative cardiovascular event (``yes category in blue``) than for those who didn't (``no category in red``). Poverty ratio is defined as the total family income divided by the poverty threshold. A lower poverty ratio usually indicates a higher likelihood that a household with that given income is living in poverty.
- `ASCVD_byIncome.png` - Bar plot demonstrating how `ASCVD` scores vary for those of different **Income** brackets. Lower income categories have higher ASCVD risk scores on average than those in higher income categories.
- `ASCVD_byRace.png` - Bar plot demonstrating how `ASCVD` scores vary for those of different **Races**. Non-hispanic Black has the highest ASCVD risk score on average compared to those of different race categories. Other categories show no error-bar overlap, indicating they also have statistically significant differences among each other. 
- `ASCVD_example.png` - Example score demonstrating the variables used in the [current ASCVD Risk Estimator Calculator](https://tools.acc.org/ascvd-risk-estimator-plus/#!/calculate/estimate/) using the ACC/AHA PCE to compute  ASCVD risk scores for a 55 year-old white male.
- `ASCVD_vs_CVDoutcomes.png` - Violin plot demonstrating how the ASCVD score distribution varies between our two cardiovascular health outcomes: `negative = 1` vs. `non-negative = 0`.

### Exploratory Analysis:
- `NAs.png` - Bar plot demonstrating how many NAs were in each of our feature variable categories before imputation was applied.
- `cvd_events_barplot.png` - Bar graph demonstrating the imbalance in our dataset pertaining to our target variable: cardiovascular health outcomes: `negative = 1` vs. `non-negative = 0`.
- `table1_cat.png` - Table 1 for all our categorical values, providing us a holistic understanding of the distribution of our data for each feature variable as it relates to our target variable: CVD outcomes. It provides the percentage breakdown of each ``Yes/No" category for both types of CVD outcomes for each of our  categorical variables.
- `table1_cont.png` - Table 1 for all our continuous values, providing us a holistic understanding of the distribution of our data for each feature variable as it relates to our target variable: CVD outcomes. It provides us the min/max values, median, mean and number of NAs for both types of CVD outcomes for each of our continuous variables. 

### Project Design: 
- `Flow_Chart.png` - Flowchart representing the above described methodology, highlighting both the existing and new feature variables that will be used to train our models in predicting CVD outcomes in adult patients.
- `machine_learning_pipeline.png` - Machine Learning pipeline representing the various steps required to build a predictive machine learning model.





