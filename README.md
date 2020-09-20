### IDS702 - Modeling And Representation Of Data (Fall 2020)
#### Data Analysis Project 3

This is a data analysis R project I did for the Modeling and Representation of Data course at Duke University. 
The purpose of the analysis is to provide insights to these questions asked below (texts adapted from Professor Akande's course website). 

#### MATERNAL SMOKING AND PRE-TERM BIRTH. 
This question is a continuation of the question on maternal smoking and birth weigths from the last assignment (project2). Remember that the data file contained an indicator variable called Premature (gestational age < 270 days), which is just a recoding of gestational age. For this assignment, use that as your outcome/response variable.

Our questions of interest are very similar to the last assignment as well, except using the new response variable. The questions are as follows:

1. Do mothers who smoke tend to have higher chances of pre-term birth than mothers who do not smoke? What is a likely range for the odds ratio of pre-term birth for smokers and non-smokers?
2. Is there any evidence that the odds ratio of pre-term birth for smokers and non-smokers differs by mother’s race? If so, characterize those differences.
3. Are there other interesting associations with the odds of pre-term birth that are worth mentioning?

First build your model, then do model assessment and validation. You should only proceed to answer the questions when you are satisfied with your final model; you should answer all the questions using that final model.

Analyze the data and investigate these questions using a logistic regression model and include the following in your report:
- the model you ultimately decided to use
- clear model building, that is, justification for the final model (e.g., why you chose certain transformations and why you decided the final model is reasonable to use based on binned residual diagnostics, ROC curves and other metrics for model comparison, such as change in deviance),
- the relevant regression output (includes: a table with coefficients and SEs, and p-values or confidence intervals; and somewhere in the text or table the “area under the curve” for your final model),
- your interpretation of the results in the context of the questions of interest, and
- any potential limitations of the analysis.

The report is organized into sections as follows.

Summary: a few sentences describing the inferential question(s), the method used and the most important results.
Introduction: a short but more in-depth introduction to the inferential question(s) of interest. Here, you are basically writing the experiment and questions of interest given in your own words.
Data: your EDA, interesting features of the data, and how you dealt with missing/erroneous values. Try to include one or two plots of your most interesting EDA findings.
Model: a detailed description of the model used, how you selected the model, how you selected the variables, model assessment, model validation, and presentation of the model results. What are your overall conclusions in context of the inferential problem(s)? Try to include one or two plots that can help drive your point home.
Conclusion: the importance of your findings and potential limitations of the study.
