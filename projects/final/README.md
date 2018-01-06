# Final Materials for 500 Projects

## Submission Details

You will submit this in two parts.

1. Your pre-presentation version of your abstract and slides, due at 11 PM on April 18.
2. Your final version of your abstract, slides, R Markdown file, HTML document, data set, and anything else, due at noon on May 1.

## The Abstract

Your abstract should be no longer than 2 pages (perhaps 4,000 characters at the most) and contains much of your approved proposal (perhaps more succinctly summarizing some of the background, data set, and methodological details to meet the character limit.) To this, you will add (still within the character limit) brief Results and Conclusions sections. Unlike our previous versions of this task, this version of the Abstract should be divided into four sections, as indicated below:

- a **Background** section, to include basic descriptive information about the problem of interest and its clinical relevance, leading to a study objective, and concluding with a careful statement of the main research question, or hypothesis.
- a **Methods** section, to include the classification of the type of research design, a description of the setting and participants, the specific details on the intervention or exposure of interest, and how it is allocated to participants, along with a listing of primary outcome measures and a description of the data set. You'll also need to specify (in general terms) the covariates used in building your propensity score. This should then be followed by a paragraph or two describing the statistical methodology used for both developing the balanced covariate information through (in one analysis) matching on the propensity score and (in another analysis) some other method involving propensity weighting, as well as specifying the actual method of comparing outcomes after propensity scores have been used.
- a **Results** section, to include the results for your primary outcome, and any secondary outcomes, probably described using point estimates and confidence intervals, rather than *p* values, and also describing the effectiveness of the propensity score work you did in improving covariate balance across your exposure groups. Any sensitivity analyses should also be reported here, though in a manuscript, they might make the discussion section instead of the Results.
- a **Conclusions** section, to include a brief summary of the key conclusions, related directly to the research questions posed in the Background section, along with some indication of plans for future work.

The version of your Abstract that you submit on April 18 should be complete. If you decide to make changes as a result of comments made in the course of your Presentation, then the version you submit on May 1 should reflect that. 

## The Presentation

After all of the project proposals have been approved, we will settle on a schedule for the presentations (some will be on April 19, some on April 26.) Your slides must be submitted prior to the presentation (by 11 PM on April 18) in either PDF or Powerpoint format.

Broadly, your slides will include an introduction which provides a foundation by motivating and clearly stating the research questions you studied, a main section which summarizes your pre-data collection beliefs, the key models and analytical results, and the critical findings of the study, and a conclusion, which provides insight into how your knowledge of the problem you studied has changed as a result of the project, as well as highlighting what you believe to be the key takeaways (both statistical and study-specific) for your audience. These sections should be keyed to slides, smoothing transitions, and forcing you to "tell us what you're going to tell us, tell us, then tell us what you told us."  Plan for 25 minutes of total time, which should include about 18 minutes of slides, allowing 3-4 minutes for asking and answering questions during the talk, and 3-4 minutes after the talk.

### Some Suggestions and a Potential Outline for Your Presentation

Don't use more than 24 slides (in fact, 20 is sufficient), including a title slide containing the project title, and your name, email and affiliation(s). Use large, extremely readable fonts. Class slides provide insight into what I think works well. 

Here's how I might outline such a talk. Do not feel obligated to follow this outline precisely, but I thought it might help to see what I'm thinking about when I say 20 slides is sufficient.

- Slide 1: Meaningful Title, with your contact details, affiliations, and the date. 
- Slides 2-4: Background slides (if you don't need three slides, use 2 or even 1) - Include a VERY small amount of background material – just enough to let us understand the major clinical issues involved well enough to evaluate your results. Most students err here on the side of providing too much information. This project presentation should focus on the methodological issues. This shouldn't be more than 2-3 minutes.
- Slide 5: A slide for the research question and population of interest
- Slide 6: A slide for data source, exposure and outcome definitions – the slides should clearly state the source of data (perhaps with the description of the population), the definition of the exposure and any key outcomes (with details as needed so we understand what we're looking at) and specifically including the number of patients in each exposure group prior to matching
- Slide 7: A slide to list the covariates in groups, explaining why you chose what you did, without reading a long list to us. You should be able to explain each of the measures involved if asked, but don't read the list to us – just have it, and be able to tell us how many variables were in your propensity model. It's helpful to group the covariates by type rather than, say, alphabetically. You should also be able to indicate which variables (if any) you had to impute, and what approaches of those I provided (or others, if applicable) that you used to do that imputation.
- Slide 8: A slide to describe the analyses you did – matching (including how many matches you made, and whether you did anything other than 1:1 greedy matching) and then your second analysis – as discussed earlier.
- Slide 9: A slide to indicate how you fit the propensity score (i.e. propensity to be in which group?) and its results – specifically, how many covariates did you include, what was the minimum and maximum propensity score within each exposure group (so we can see that they're not too close to 0 or 1), and perhaps a density plot to compare the propensity scores.
- Slide 10: A Love plot to describe covariate balance in terms of standardized differences before and after matching.
- Slide 11: An assessment/table of Rubin's Rules before and after matching. No need to show the Rubin's Rule 3 plot or the variance ratio plot – you can just summarize important details.
- Slide 12: As necessary, a slide to describe any methodological or data problems seen during the matching. This might come earlier in the talk or be eliminated altogether.
- Slide 13: A slide describing the primary outcome result after matching – showing the estimated causal effect (perhaps an odds ratio, hazard rate or risk difference, or whatever) properly labeled, explained in detail, and accompanied by a 95\% confidence interval, and a comparison to the original (unadjusted) estimate and confidence interval.
- Slides 14-15: 1-2 slides to describe what sort of weighted analysis you did and how it worked out in terms of improving covariate balance and reducing selection bias (if this is weighting alone, for instance, highlights of an assessment of balance after weighting would probably just take one slide)
- Slide 16: A slide describing the primary outcome result after your second propensity-based analysis – showing the estimated causal effect (perhaps an odds ratio, hazard rate or risk difference, or whatever) properly labeled, explained in detail, and accompanied by a 95% confidence interval, and a comparison to both the matched and the original (unadjusted) estimates and confidence intervals. You should be prepared to indicate which analysis is more appropriate in your view, on the basis of the quality of balance achieved, mostly.
- Slide 17: If your 1:1 matched analysis was statistically significant, you should present a sensitivity analysis, with a gamma estimate, in terms of an actual sentence or two in English. If it wasn't, you should present some thoughts on potential stability analyses.
- Slide 18: Description of results for secondary outcomes (if needed)
- Slide 19: A slide with clinical conclusions, focusing on the primary outcome.
- Slide 20: A slide with statistical conclusions – additional methodological considerations. What do you know now that you wish you knew at the beginning, or that you think might be useful to others, or that you think might be useful to you after much of the class has faded into memory?

