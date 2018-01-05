# Homework 1 for 500 - 2018

## 1. Get access to the DIG training data

Visit https://biolincc.nhlbi.nih.gov/teaching/ and request copies of the DIG "teaching" data set.

## 2. Build a mock proposal for a DIG observational study

Review the documentation available to you on the BIOLINCC page, and complete a **mock proposal** not to exceed 300 words for an observational study based on the available data from the DIG randomized trial. A list of questions you should address follows below. 

To help you build a response, [I have provided](https://github.com/THOMASELOVE/500-2018/tree/master/assignments/homework1): 

- a PDF of the DIG data description from BIOLINCC
- a .csv file (`dig1.csv`) of the DIG data set you will obtain from NIH/BIOLINCC
- the original 1997 publication in the *New England Journal of Medicine*  by the Digitalis Investigation Group

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
    
## 3. Build and evaluate a logistic regression model using DIG data

Use R, R Studio and R Markdown to execute a logistic regression model on the `dig1.csv` data. 

Your model should be fitted to a random training sample of 5,000 subjects (be sure to specify the seed you used to select that sample) and then tested on the remaining 1,800 subjects, but you'll probably want to check for and deal with missingness in the entire sample before splitting into training and test groups. Your model will predict the probability that a subject in the study will die, based on:

- the subject's assigned treatment (digoxin or placebo), 
- age at randomization, 
- race, 
- sex, 
- ejection fraction (percent), 
- NYHA functional class, 
- whether or not they currently have angina, and 
- their calculated body mass index. 

Be sure to treat the categorical variables (including NYHA class, angina status, race and sex) appropriately as factors (ideally with meaningful names), and account for missingness deliberately in an appropriate way. 

Your final results should include:

1. a R Markdown file containing all of your code
2. an HTML file with the results from your Markdown, which describes:
    1. your sample preparation work including dealing with missingness and partitioning the data into training and test samples
    2. your fitted logistic regression model (to your training sample)
    3. the results of your application of your model to your test sample, which is best accomplished as a graph which shows the distribution of your model probability estimates in the "actually died" and "actually survived" groups within your test sample.

