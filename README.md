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

Summary: a few sentences describing the inferential question(s), the method used and the most important results. <br />
Introduction: a short but more in-depth introduction to the inferential question(s) of interest. Here, you are basically writing the experiment and questions of interest given in your own words. <br />
Data: your EDA, interesting features of the data, and how you dealt with missing/erroneous values. Try to include one or two plots of your most interesting EDA findings. <br />
Model: a detailed description of the model used, how you selected the model, how you selected the variables, model assessment, model validation, and presentation of the model results. What are your overall conclusions in context of the inferential problem(s)? Try to include one or two plots that can help drive your point home. <br />
Conclusion: the importance of your findings and potential limitations of the study.

#### Code Book


Variable:	Description <br />
Id:	id number <br />
birth:	birth date where 1096 = January1, 1961 <br />
gestation:	length of gestation in days <br />
bwt (Response/outcome variable):	birth weight in ounces (999 = unknown) <br />
parity:	total number of previous pregnancies, including fetal deaths and still births. (99=unknown) <br />
mrace:	mother’s race or ethnicity (0-5=white, 6=mexican, 7=black, 8=asian, 9=mix, 99=unknown) <br />
mage:	mother’s age in years at termination of pregnancy <br />
med:	mother’s education (0 = less than 8th grade, 1 = 8th to 12th grade. did not graduate high school, 2 = high school graduate, no other schooling, 3 = high school graduate + trade school, 4 = high school graduate + some college, 5 = college graduate, 6,7 = trade school but unclear if graduated from high school, 9 = unknown <br />
mht:	mother’s height in inches <br />
mpregwt:	mother’s pre-pregnancy weight in pounds <br />
income:	family yearly income in 2500 increments. 0 = under 2500, 1 = 2500-4999, …, 9 = 15000+. 98=unknown, 99=not asked <br />
smoke:	does mother smoke? (0 = never, 1 = smokes now, 2 = until preg, 3 = once did, not now) <br />
Premature:	1 = baby born before gestational age of 270, and 0 = otherwise.
