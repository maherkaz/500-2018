# Homework 1 for 500 - 2018

## Get access to the DIG training data

Visit https://biolincc.nhlbi.nih.gov/teaching/ and request copies of the DIG "teaching" data set.

## Build and evaluate a logistic regression model using DIG data

Use R, R Studio and R Markdown to execute a logistic regression model on the `dig1.csv` data to predict the probability that a patient in the study will die, based on their assigned treatment (digoxin or placebo), their age at randomization, their race, their sex, their ejection fraction (percent), their NYHA functional class, whether or not they currently have angina, and their calculated body mass index. Be sure to treat the categorical variables (including NYHA class, angina status, race and sex) appropriately as factors (ideally with meaningful names), and account for missingness deliberately in an appropriate way. Your model should be fitted to a random training sample of 5,000 subjects (be sure to specify the seed you used to select that sample) and then tested on the remaining 1,800 subjects, but you'll probably want to check for and deal with missingness in the entire sample before splitting into training and test groups. Your final results should include:
    - a R Markdown file containing all of your code
    - an HTML file with the results from your Markdown
    - your sample preparation work including dealing with missingness and partitioning
    - your fitted logistic regression model (to your sample of 5,000 subjects)
    - the results of your test on the remaining 1,800 subjects, which is best accomplished as a graph which shows the distribution of your model probability estimates in the "actually died" and "actually survived" groups within your test sample of 1,800 subjects.

## Build a mock proposal for a DIG observational study

Review the documentation available to you on the BIOLINCC page, and also included above, and complete a **mock proposal** not to exceed 2 pages for an observational study based on the available DIG data, based on that information. A list of questions you should address follows below. Above you'll find 
    - a PDF of the DIG data description 
    - a .csv file of the DIG data set you will obtain from NIH
    - the original 1997 publication in *NEJM*  by the Digitalis Investigation Group

### Questions to be addressed in the Mock Proposals

1. What comparison do you want to make? (Select a comparison different than the one made in the original DIG paper)
    + Did patients receiving "EXPOSURE A" have lower rates of "BAD OUTCOME" than those who received "EXPOSURE B"?
2. Why is this of interest?
    + "OUTCOME" is important because ...
    + "EXPOSURE" (A or B) is important because ...
    + (*Be sure to clearly indicate what you hypothesize the effect of EXPOSURE on OUTCOME to be.*)
3. What are the key measures - specifically, the exposure/treatment, the primary outcome, and important covariates that are available in the data to help address your question of interest?
    + Exposure/Treatment = A or B, and be sure to specify the way in which you will know which exposure someone receives, and whether the exposure / treatment is applied using a randomized approach, or not.
    + Outcome = ..., and be sure to specify the variables you will use to determine the outcome, as well as the *type* of outcome, be it continuous, categorical (and if categorical, binary or multi-categorical) or survival (and if survival, is censoring involved?) 
    + Covariates of interest: We'd be interested in anything related to treatment choice or to outcome. You should provide a list of such variables of interest. Remember to include **ONLY** things which are measured prior to the exposure/treatment of interest, or which are not possibly changed by it.
