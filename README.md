## Module 20 Challenge - Credit Risk Classification

In this assignment, we first split the lending data into training and testing sets, then trained a logistic regression model on the original data to predict loan statuses. 

After evaluating its performance, we proceeded to address class imbalance by oversampling the training data using RandomOverSampler. 
We trained another logistic regression model on the oversampled data and evaluated its performance. The oversampled model demonstrated improved predictive capabilities for both healthy and high-risk loans compared to the model trained on the original data.

This assignment I found relatively complicated at first, but was able to start feeling more comfortable with the concepts as the assignment went on. I have struggled the most with the machine learning portion of this bootcamp, so that isn't much of a surprise to me, but it is fun to overcome the challenges.


Overview
    The analysis aimed to assess credit risk using machine learning models. Data comprised financial information on loans, and the goal was to predict loan statuses. The loan_status variable had imbalanced classes, with more healthy loans (0) than high-risk loans (1). We employed logistic regression models and resampling techniques to address class imbalance.

Results
Model 1:
    Balanced Accuracy: 0.9679899
    Precision and Recall Scores: 
                0       1.00 precision     0.99 recall `0` healthy loan
                1       0.84 precision     0.94 recall `1` high-risk loan
Model 2:
    Balanced Accuracy: 0.993599
    Precision and Recall Scores:
                0       1.00 precision     0.99 recall `0` healthy loan
                1       0.84 precision     0.99 recall `1` high-risk loan

Summary
    The performance of both models varied. Model 2, trained on oversampled data, generally exhibited better accuracy, precision, and recall compared to Model 1. The choice of model depends on the priority of prediction targets. While Model 2 demonstrated overall improvement, it is crucial to consider specific goals, such as prioritizing accurate predictions for high-risk loans `1` or healthy loans `0`. Further analysis may be necessary to determine the most suitable model for specific business needs.


Material referenced for the completion of this assignment includes the recorded lectures from class, notes taken during class, as well as supplemental content provided by the instructor.