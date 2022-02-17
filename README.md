# King County Real Estate Analysis



![from giphy](https://media.giphy.com/media/l0IylQoMkcbZUbtKw/giphy.gif)


Authors:  Andrew Choi, Richard Hinds, and Samira Chatrathi

## Project Overview

For this project, you will use multiple linear regression modeling to analyze house sales in a northwestern county.

## Business Problem
The Real Estate Market is undoubtedly, one of high volatility. Whether it is rooted in a housing bubble or located within a very concentrated region, housing value is determined by a wide-array of factors outside of an individuals control. We, ultimately, strive as a data science team to see what factors we can encourage our stakeholder to consider when making decisions as to what to prioritize within a home rennovation. We are analyzing from the point of view of a homeowner and private flipper in King County, Washington looking to increase the value of their home through controllable factors. Our value is defined as the overall price of the home, and our variables are iterated over five models to see how some factors change the overall value. Not only will our modeling and analysis help our stakeholder understand King County specifically, but it will also provide inferential understanding to help them decide which aspects of home rennovation can give them the best return on investment.

## Data and Methods

We used home sales data for King County, Washington which had a population of 2.25 million people. We reviewed home sales from 2014 to 2015 which contains over 21k datapoints and cleaned our data, removing erroneous values. Some of our limitations stemmed from the fact that our data was collected from the range of 2014-2015. This prevented us from seeing how a current homeowner could use our model while understanding the inflation rate as well as the change in value in the current time period. Another data limitation that we faced, was understanding how rennovation is defined consistently across homeowners, as costs of rennovation are difficult to incorporate with the current dataset. We decided to drop variables that didn't have as much use value to our stakeholder. The columns we decided to drop were latitude, longitude, waterfront, view, The square footage of interior housing living space for the nearest 15 neighbors, and the square footage of the land lots of the nearest 15 neighbors. We chose these varaibles because our stakeholder is focusing on controllable factors for their own rennovation. Of the controllable variables, we were able to create a dummy variable associated with our conditon. Althought, we didn't use the zipcode data in our analysis , we were able to bin zipcdoe based off of rural and not rural. After we cleaned all of our data we labeled the final dataset as 'master_dataset.csv'. 


### Methods
To validate our model, we tested for the assumptions of linear regression.

Check Normal Distributions of Input Variables
Heteroskedasticity - lack of trend in errors
Linearity and Multicollinearity - are input variables too closely correlated















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




