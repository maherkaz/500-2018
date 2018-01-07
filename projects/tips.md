# A Few Tips Regarding the Project

I expect you to do (and present) two analyses using propensity scores. You will eventually be submitting a single R Markdown file that takes your original (perhaps after cleaning) data, and produces all of the analyses you will do. You will perform a first analysis that uses matching and a second analysis that uses weighting. 

For the matched analysis, you can use any form of propensity score matching: in most cases this will probably be just 1:1 greedy matching without replacement. You are welcome to consider alternative matching strategies as part of your first analysis. 

My strong preference in a second analysis is that you use propensity score weighting (ATT approach) along with the linear propensity score included as an adjustor in the final outcome model after weighting – we'll call this a ``doubly robust'' analysis. Should that not be feasible for some reason, you may instead consider ATT weighting on the propensity score without the additional adjustment.

## Checking to See if Your Propensity Scores are Too Close to Zero or One

We will worry if a propensity score value is below 0.01 or above 0.99. If that happens to you, contact me, quickly. If just one or two subjects fall in that range, we may wind up just dropping them from the study. If more fall in that range, we will have to look for variables included in your covariate list that either alone or in combination with other covariates, determine the treatment group perfectly.

The simplest check is to get a summary of the bottom few and top few propensity score values within each treatment group, perhaps with the `describe` function in the `Hmisc` package. 

## Squared Terms or Product Terms in a Propensity or Outcome Model

Suppose you decide you want to include Age as a covariate in your propensity or outcome model, and also account for the notion that Age might have a non-linear relationship with what you're trying to predict, or just for the notion that Age is an especially important continuous covariate to balance well. So you decide, as a result to include Age and Age squared in your model. Try this...

1. Find the average `age` for all subjects. If some subjects don't have an `age`, impute first.
2. Subtract that average `age` from each subject's `age` to create a new variable, called centered age. If the overall average age was 50, and the first subject's age was 53, then that subject's centered age would be 3. If the second subject was 44, then centered age would be -6.
3. Create a new variable containing the square of the centered age for each subject.
4. Include the centered age (I usually call this `age.c`) and its square (`age.c2`) in your outcome model or propensity model, in place of the original ages.

If you're including an interaction between a binary indicator and a continuous variable in a model for the purposes of the project, I would simply create a product term and include that. Include a product term if you have reason to believe there is a meaningful interaction between the variables.

