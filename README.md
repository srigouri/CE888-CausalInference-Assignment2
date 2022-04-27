# CE888-Data Science and Decision Making- Assignment2
# Causal Inference on IHDP and Jobs datasets.

This repository holds  3 files containing python code for Causal Inference model on two different datasets(IHDP data & JOBS data).
Note:IHDP_Causal.ipynb & ihdp_causal.py(1) ,JOBS_Causal.ipynb & jobs_causal(1).py are same.Can use either one according to convenience.

1.Causal Effect on IHDP data - IHDP_causal.py: 

  - This code is to model Random Forest Regression on IHDP Data.

  - A Random Forest Classifier was trained on IHDP_data to predict propensity scores.Based on propensity scores weights were computed and trained the regressor model      using these weights.

  - CATE estimator X-learner from EConML package is trained on IHDP data to predict the effects.

  - Implementation of Evaluation metrics like Absolute Treatment Effect(ATE) and Precision in Estimating the Heterogeneous Treatment Effect(PEHE).The functions to          evaluate the metrics,confidence intervals are called from causalfuncs.py.So,it has to be uploaded in the same directory to execute the metrics without any errors.

  - Visualizations of the effects that are predicted using all the 3 models using Boxplot and scatterplot.

2.Causal Effect on JOBS data - JOBS_causal.py:

- This code is to model Logistic Regression on JOBS Data.

- A Random Forest Classifier was trained on IHDP_data to predict propensity scores.Based on propensity scores weights were computed and trained the regressor model using these weights.

- CATE estimator X-learner from EConML package is also trained on IHDP data to predict the effects.

- Then Evaluation metrics like Absolute Treatment Effect(ATE), Precision in Estimating the Heterogeneous Treatment Effect(PEHE), ATT and policy risk were evaluated and compared.The functions to evaluate the metrics,confidence intervals are called from causalfuncs.py.

- Visualizations of the effects that are predicted using all the 3 models using Boxplot and scatterplot.

3.causalfuncs.py:

This file contains functions to compute evaluation metrics. 
- Absolute Treatment Effect(ATE) 
- Precision in Estimating the Heterogeneous Treatment Effect(PEHE)
- Absolute error for the Average Treatment Effect on the Treated
- risk of the policy defined by predicted effect
- computing weights using classifier and propensity scores
- function to compute confidence intervals.

This file has to be uploaded in the same directory to execute IHDP_Causal.py and JOBS_Causal.py


#References:

- CE-888 Lab4 Causal Inference on sodium and Toys dataset.
- Functions to evaluate metrics: https://github.com/dmachlanski/CE888_2022/blob/main/project/metrics.py

#Source for data : https://github.com/dmachlanski/CE888_2022/tree/main/project/data (Moodle.essex)
