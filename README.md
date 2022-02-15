# King County Real Estate Analysis



![from giphy](https://media.giphy.com/media/l0IylQoMkcbZUbtKw/giphy.gif)
By: Andrew Choi, Richard Hinds, and Samira Chatrathi

## Project Overview

For this project, you will use multiple linear regression modeling to analyze house sales in a northwestern county.

### Business Problem
The Real estate market is undoubtedly, one of high volatility. Whether it is rooted in a housing bubble or located within a very concentrated region, housing value is determined by a wide-array of factors outside of an individuals control. We, ultimately, strive as a data science team to see what factors we can encourage our stakeholder to consider when making decisions as to what to prioritize within a home. We are analyzing from the point of view of a homeowner and private flipper in King County, Washington looking to increase the value of their home through efficient rennovations. Our value is defined as the overall price of the home, and our variables are iterated over three models to see how some factors change the overall value. Not only will our modeling and analysis help our stakeholder understand King County specifically, but it well provide inferential understanding to help them decide which aspects of home rennovation can give them the best return on investment.

### The Data

This project uses the King County House Sales dataset. 

It is up to you to decide what data from this dataset to use and how to use it. If you are feeling overwhelmed or behind, we recommend you **ignore** some or all of the following features:

* `date`
* `view`
* `sqft_above`
* `sqft_basement`
* `yr_renovated`
* `zipcode`
* `lat`
* `long`
* `sqft_living15`
* `sqft_lot15`



### Statistical Analysis






### Key Points

* **Your goal in regression modeling is to yield findings to support relevant recommendations. Those findings should include a metric describing overall model performance as well as at least two regression model coefficients.** As you explore the data and refine your stakeholder and business problem definitions, make sure you are also thinking about how a linear regression model adds value to your analysis. "The assignment was to use linear regression" is not an acceptable answer! You can also use additional statistical techniques other than linear regression, so long as you clearly explain why you are using each technique.

* **You should demonstrate an iterative approach to modeling.** This means that you must build multiple models. Begin with a basic model, evaluate it, and then provide justification for and proceed to a new model. After you finish refining your models, you should provide 1-3 paragraphs in the notebook discussing your final model.

* **Data visualization and analysis are no longer explicit project requirements, but they are still very important.** In Phase 1, your project stopped earlier in the CRISP-DM process. Now you are going a step further, to modeling. Data visualization and analysis will help you build better models and tell a better story to your stakeholders.

## Deliverables

There are three deliverables for this project:

* A **non-technical presentation**
* A **Jupyter Notebook**
* A **GitHub repository**

The deliverables requirements are almost the same as in the Phase 1 Project, and you can review those extended descriptions [here](https://github.com/learn-co-curriculum/dsc-phase-1-project-v2-3#deliverables). In general, everything is the same except the "Data Visualization" and "Data Analysis" requirements have been replaced by "Modeling" and "Regression Results" requirements.

### Non-Technical Presentation

Recall that the non-technical presentation is a slide deck presenting your analysis to ***business stakeholders***, and should be presented live as well as submitted in PDF form on Canvas.

We recommend that you follow this structure, although the slide titles should be specific to your project:

1. Beginning
    - Overview
    - Business and Data Understanding
2. Middle
    - **Modeling**
    - **Regression Results**
3. End
    - Recommendations
    - Next Steps
    - Thank you

Make sure that your discussion of modeling and regression results is geared towards a non-technical audience! Assume that their prior knowledge of regression modeling is minimal. You don't need to explain how linear regression works, but you should explain why linear regression is useful for the problem context. Make sure you translate any metrics or coefficients into their plain language implications.

The graded elements for the non-technical presentation are the same as in [Phase 1](https://github.com/learn-co-curriculum/dsc-phase-1-project-v2-3#deliverables).

### Jupyter Notebook

Recall that the Jupyter Notebook is a notebook that uses Python and Markdown to present your analysis to a ***data science audience***. You will submit the notebook in PDF format on Canvas as well as in `.ipynb` format in your GitHub repository.

The graded elements for the Jupyter Notebook are:

* Business Understanding
* Data Understanding
* Data Preparation
* **Modeling**
* **Regression Results**
* Code Quality

### GitHub Repository

Recall that the GitHub repository is the cloud-hosted directory containing all of your project files as well as their version history.

The requirements are the same as in [Phase 1](https://github.com/learn-co-curriculum/dsc-phase-1-project-v2-3#github-repository), except for the required sections in the `README.md`.

For this project, the `README.md` file should contain:

* Overview
* Business and Data Understanding
  * Explain your stakeholder audience here
* **Modeling**
* **Regression Results**
* Conclusion

Just like in Phase 1, the `README.md` file should be the bridge between your non technical presentation and the Jupyter Notebook. It should not contain the code used to develop your analysis, but should provide a more in-depth explanation of your methodology and analysis than what is described in your presentation slides.

## Grading

***To pass this project, you must pass each project rubric objective.*** The project rubric objectives for Phase 2 are:

1. Attention to Detail
2. Statistical Communication
3. Data Preparation Fundamentals
4. Linear Modeling

### Attention to Detail

Just like in Phase 1, this rubric objective is based on your completion of checklist items. ***In Phase 2, you need to complete 70% (7 out of 10) or more of the checklist elements in order to pass the Attention to Detail objective.***

**NOTE THAT THE PASSING BAR IS HIGHER IN PHASE 2 THAN IT WAS IN PHASE 1!**

The standard will increase with each Phase, until you will be required to complete all elements to pass Phase 5 (Capstone).

#### Exceeds Objective

80% or more of the project checklist items are complete

#### Meets Objective (Passing Bar)

70% of the project checklist items are complete

#### Approaching Objective

60% of the project checklist items are complete

#### Does Not Meet Objective

50% or fewer of the project checklist items are complete

### Statistical Communication

Recall that communication is one of the key data science "soft skills". In Phase 2, we are specifically focused on Statistical Communication. We define Statistical Communication as:

> Communicating **results of statistical analyses** to diverse audiences via writing and live presentation

Note that this is the same as in Phase 1, except we are replacing "basic data analysis" with "statistical analyses".

High-quality Statistical Communication includes rationale, results, limitations, and recommendations:

* **Rationale:** Explaining why you are using statistical analyses rather than basic data analysis
  * For example, why are you using regression coefficients rather than just a graph?
  * What about the problem or data is suitable for this form of analysis?
  * For a data science audience, this includes your reasoning for the changes you applied while iterating between models.
* **Results:** Describing the overall model metrics and feature coefficients
  * You need at least one overall model metric (e.g. r-squared or RMSE) and at least two feature coefficients.
  * For a business audience, make sure you connect any metrics to real-world implications. You do not need to get into the details of how linear regression works.
  * For a data science audience, you don't need to explain what a metric is, but make sure you explain why you chose that particular one.
* **Limitations:** Identifying the limitations and/or uncertainty present in your analysis
  * This could include p-values/alpha values, confidence intervals, assumptions of linear regression, missing data, etc.
  * In general, this should be more in-depth for a data science audience and more surface-level for a business audience.
* **Recommendations:** Interpreting the model results and limitations in the context of the business problem
  * What should stakeholders _do_ with this information?

#### Exceeds Objective

Communicates the rationale, results, limitations, and specific recommendations of statistical analyses

> See above for extended explanations of these terms.

#### Meets Objective (Passing Bar)

Successfully communicates the results of statistical analyses without any major errors

> The minimum requirement is to communicate the _results_, meaning at least one overall model metric (e.g. r-squared or RMSE) as well as at least two feature coefficients. See the Approaching Objective section for an explanation of what a "major error" means.

#### Approaching Objective

Communicates the results of statistical analyses with at least one major error

> A major error means that some aspect of your explanation is fundamentally incorrect. For example, if a feature coefficient is negative and you say that an increase in that feature results in an increase of the target, that would be a major error. Another example would be if you say that the feature with the highest coefficient is the "most statistically significant" while ignoring the p-value. One more example would be reporting a coefficient that is not statistically significant, rather than saying "no statistically significant linear relationship was found"

> "**If a coefficient's t-statistic is not significant, don't interpret it at all.** You can't be sure that the value of the corresponding parameter in the underlying regression model isn't really zero." _DeVeaux, Velleman, and Bock (2012), Stats: Data and Models, 3rd edition, pg. 801_. Check out [this website](https://web.ma.utexas.edu/users/mks/statmistakes/TOC.html) for extensive additional examples of mistakes using statistics.

> The easiest way to avoid making a major error is to have someone double-check your work. Reach out to peers on Slack and ask them to confirm whether your interpretation makes sense!

#### Does Not Meet Objective

Does not communicate the results of statistical analyses

> It is not sufficient to just display the entire results summary. You need to pull out at least one overall model metric (e.g. r-squared, RMSE) and at least two feature coefficients, and explain what those numbers mean.



