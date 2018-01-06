# Course Projects for 500, Spring 2018

## Introduction

As a substantial part of your course grade, you will complete a small observational study comparing two exposures on at least two outcome(s) in time to generate an abstract, give a presentation, and complete a thorough written discussion using R Markdown.

"It is hard to learn statistics (or anything else) passively; concurrent theory and application are essential."

Though hardly an original idea in general, this particular phrasing is stolen from Harry Roberts, as are several of the bulleted points to follow, originally prepared for his courses at the University of Chicago. I am also grateful to Doug Zahn, for several helpful suggestions swiped from his work at Florida State University, and to Dave Hildebrand, for many things, not least his excellent example at Wharton. 

There is more to a statistical application than the analysis of a canned data set, even a good canned data set. George Box noted that "statistics has no reason for existence except as the catalyst for investigation and discovery." Expert clinical researchers and statisticians repeatedly emphasize how important it is that people be able to write well, present clearly, work to solve problems, and show initiative. This project assignment is designed to help you develop your abilities and have a memorable experience.

## Three Deliverables and their Deadlines

I want you to establish relevant and interesting research questions related to a problem of interest, procure data to help answer the questions and pose others, and communicate your results to an audience of your peers. You will be responsible for the following elements of a project, described in detail in the rest of this document. All materials for the project should be submitted through canvas.case.edu

1. A **proposal** which you will submit for my approval in February. Here you will be identifying an observational study of interest and writing a detailed proposal, which you will revise, as needed, in reaction to my comments, until a final version is complete not later than March 1, so your initial submission should be submitted at least a couple of weeks prior to that date.

2. An **update** verifying that you have the data and are proceeding appropriately, due April 1.

3. A final 20-minute **presentation** to the class about your results, due April 19, although some presentations will be given on April 26. In addition to building presentation slides using Markdown or some other strategy (like Powerpoint), you will produce a formal abstract of the study, and a paired R Markdown and HTML file set that describes all of your analytic and data management work.

**Please don't be shy about asking for help sooner, rather than later. Options narrow as an investigation progresses. The earlier I hear about a problem, the more likely I will be able to help solve it.**

## Task 1: The Proposal, which can be submitted in February, and must be approved by March 1.

Your proposal will be a summary (moving towards an abstract) of your proposed study, and must include:

1. A good, interesting title. You will work hard on this: please don't call it "Observational Studies Project."  A vast majority of your intended audience will never get past the title and abstract of the final report. Get off to a good start. Avoid deadwood like "The Study of..." or "An Analysis of..."
2. Your name and the names of any co-investigators (in which case you should indicate their role in this work.)
3. No more than a paragraph (and, perhaps, one figure) of background information, meant to help me understand the study's objective. Use words I know.
4. An objective or list of study objectives, which leads directly to the research question.
    - Be sure you specify the population, key outcome(s), and exposure/treatment (as well as, perhaps, some of the covariates of interest) in developing your objective.
    - This is a **SMALL** study. Do not boil the ocean.
5. A careful statement of the research question(s), with indications about anticipated directions for any hypotheses. 
    - Please state research questions as questions.
6. A classification of the type of research design (i.e. prospective cohort, etc.)
7. A description of the setting in which the data were collected (i.e. MHMC burn unit)
8. A brief description of the participants, including key inclusion or exclusion criteria, as well as the size and style of the sample (i.e. 200 consecutive male patients between November and May with burns over more than 15% of their bodies)
9. A brief description of the intervention or exposure of interest
10. A description of the exposure's method of allocation to participants
11. A listing of primary outcome measures, which should be clearly linked to the objectives.
    - Be sure to indicate clearly why these outcome measures are important. Do not assume that I know.
    - Also, please indicate clearly how these outcome measures will be obtained and (one hopes) validated.
12. A paragraph or two describing the available data set, and confirming that you either have it or describing why you will certainly be able to get it well before the April 1 deadline.
13. A paragraph or two describing your planned statistical methodology for answering your research questions. Obviously, you won't have developed a complete tool set here, but do the best you can. Here is a sample recipe for this last piece:
    - Statistical Methods: Appropriate graphical and numerical data summaries across *the exposure groups*, followed by propensity score matching and weighting methods to address selection bias. For outcomes analysis, our primary tool will be *primary tool* on propensity-matched pairs, as well as unadjusted and propensity-weighted comparisons of *the exposure groups* on *our primary outcome*.
    - Note that you'll need to insert the information *in italics* yourself, including the specific exposure groups you're comparing and your primary outcome measure. In most cases your primary tool is determined by the type of outcome you are working with, as follows:
        - If your primary outcome is continuous, your primary tool will usually be linear regression.
        - If your primary outcome is binary (yes/no), your primary tool will usually be logistic regression. 
        - If your primary outcome is time-to-event, your primary tool will usually be Cox regression.

That should be sufficient for this first draft. You'll need to fill in additional details by the time you submit the revised abstract later in the semester. If you've written three pages or more, go back and edit until you're down to about two pages. Your eventual abstract will also include results and conclusions, but we're not there yet. All materials for the project should be submitted through canvas.case.edu

### Frequently Asked Questions about the Proposal

1. I want to run a project idea past you prior to doing a formal proposal. What information do you need to see immediately to understand whether or not a more complete proposal is likely to be successful?
    - There are four things I will need, at a minimum. 
        - What is the exposure - what are the two groups of patients you intend to compare, and how many patients are in each of those groups (it's also helpful to tell me where the patients come from, and how they're selected to be in the study.)
        - What is the primary outcome you wish to compare them on, and how is that variable measured? Hearing about secondary outcomes is also helpful, but you should limit yourself to no more than two outcomes, total, in this study.
        - What is the nature of the covariate information - what variables do you have, specifically, that you propose to include in your Table 1 comparing the two groups, and in the propensity model? Are they all measured PRIOR to the decision to apply or not apply the exposure of interest to patients?
        - Do you have the data in hand? What are the steps that need to happen to get the data in hand? Are there any IRB/HIPAA concerns worth mentioning at this point?
        
2. What are the characteristics of a data set that makes it highly appropriate for this project?
    - You have the data, and can prove to me that you can present it to the class without drawing the ire of any regulatory body or review board.
    - You know how the data were gathered, and can investigate problems in the data yourself. You are capable of cleaning and managing the entire data set that you plan to use, yourself.
    - The data have not previously been analyzed using propensity scores, though it is possible that you have new data and wish to partially replicate an existing study.
    - The data compares two groups of subjects, some of whom received an exposure of interest and some of whom did not (or received an alternative exposure) for reasons that are not directly related to a random allocation.
    - There are multiple covariates which can help explain why the subjects did or did not receive the exposure of interest.
    - There is at least one well-measured outcome of interest, which you believe to be both important to learn about and to potentially be causally linked to the exposure, usually on the basis of both a logical argument, some (biological or other) theory and some prior empirical evidence.
    - You have sufficient numbers of subjects and covariates for propensity score methodology to be plausible. On some level, the more observations you have, the better, but not if you're still collecting or cleaning the data. If you have more than a half-dozen covariates you wish to include in the propensity score, and have at least 100 patients in the smaller of your two exposure groups, I am not likely to be especially concerned about the size of your data set. If you cannot meet these standards with a data set in which you have a serious interest, contact me to discuss the matter, soon.

3. Will you help me find a data set to use?
    - That's your job. I will happily help you decide whether a particular observational study is likely to work well for this project, but I am not going to find data for you.

4. I have multiple outcomes I'm interested in - it's hard to pick a primary one in advance - will I have time to look at multiple outcomes in the presentation?}
    - You'll likely run models looking at multiple outcomes - expect to wind up only presenting some of those outcomes, and perhaps only one in detail, for the class. But there's no reason to settle on which one you'll present in advance if all of the data are easily available. If you have all of the data, you can easily re-run things with a series of different outcomes once you've set up the main propensity analyses.

5. I have some variables which will have missing data. What should I do?
    - It depends, to some degree, on how much missingness you actually have. Let me know about the missingness as soon as you do, and we can discuss it.
    - Specifically for the projects (this isn't to be interpreted as globally accurate advice), I often suggest that the problem is modest in a covariate if the missingness affects less than 20 observations total, and also less than 10\% of the total sample size. Outcome or exposure missingness is a bigger problem, and it is often necessary to drop those cases from the data set. 

6. I have some variables which I could code in several ways - for instance, I could code as "yes/no" for meeting a standard or I could code as "low/middle/high" in terms of severity or I could code as the continuous measured value? Which should I do?
    - Always code everything in the least collapsed way possible at the start of building a data set. 
    - You definitely want to build your data set using the data in the least aggregated (most granular) manner possible. It is always easy to collapse categories (taking low/middle/high to low vs not low, for instance) but it is always hard to expand them (taking low vs. not low to low/middle/high). 
    - If any of your categorical variables are based on a continuous variable that you have also measured, then you should definitely include the continuous variable in your data set either instead of or along with the categorized version. Again, you can always get the categories again if you need them from the continuous results, but you can't go the other way. 

## Task 2: The Update, which can be submitted any time in March, but is due at noon on April 1.

The update should include answers to the following questions:

1. How has your abstract changed from your approved project proposal?
    - Your update should include an edited version of the proposal you got approved initially, with additional materials and edits in reaction to my comments, and in reaction to changes that have occurred (i.e. I hope you will have details now on exactly how many observations you have, what the covariates are, etc.) – this might be as much as 2-3 pages, but is basically just an edited version of what you've already submitted.
    
2. Describe the data - tell me what you have, and what you are still waiting for. 
    - Please provide a one (or more, if you need it) sentence data description statement that says something like the following...
        - I have the data, and I have imported it into R, and I have completed some recoding of variables and preliminary analyses.
        - Assuming the statement I have provided here is true, that's enough for me to see now. If you've done more than this, I don't need the details in this context.
        - If the statement here is not true because you haven't gotten to that point yet, I'm going to want details on where you are and what the problem is, and I'm going to want those details well before April 1, so I can make suggestions about what to do.

3. Describe the biggest problem you're currently having with regard to completing the design and analysis of the study. Feel free to describe multiple problems, especially if I can help. 
    - Write a paragraph (or more, if you need it) describing the major problems you're currently having. 
        - Or, if you have no major problems, tell me that, and describe the minor problems. 
        - Or, if you have no problems at all, tell me that, and tell me what you still plan to do.
        
