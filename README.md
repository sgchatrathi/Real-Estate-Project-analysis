# King County Real Estate Analysis



![from giphy](https://media.giphy.com/media/l0IylQoMkcbZUbtKw/giphy.gif)


Authors:  [Samira Chatrathi](https://github.com/sgchatrathi), [Andrew Choi](https://github.com/cjunhyuk), and [Richard Hinds](https://github.com/RH3421)

## Business Problem
The Real Estate Market is undoubtedly, one of high volatility. Whether it is rooted in a housing bubble or located within a very concentrated region, housing value is determined by a wide-array of factors outside of an individuals control. We, ultimately, strive as a data science team to see what factors we can encourage our stakeholder to consider when making decisions as to what to prioritize within a home rennovation. We are analyzing from the point of view of a homeowner and private flipper in King County, Washington looking to increase the value of their home through controllable factors. Our value is defined as the overall price of the home, and our variables are iterated over five models to see how some factors change the overall value. Not only will our modeling and analysis help our stakeholder understand King County specifically, but it will also provide inferential understanding to help them decide which aspects of home rennovation can give them the best return on investment.

## Data and Preparation

We used home sales data for King County, Washington which had a population of 2.25 million people. We reviewed home sales from 2014 to 2015 which contains over 21k datapoints and cleaned our data, removing erroneous values. Some of our limitations stemmed from the fact that our data was collected from the range of 2014-2015. This prevented us from seeing how a current homeowner could use our model while understanding the inflation rate as well as the change in value in the current time period. Another data limitation that we faced, was understanding how rennovation is defined consistently across homeowners, as costs of rennovation are difficult to incorporate with the current dataset. We decided to drop variables that didn't have as much use value to our stakeholder. The columns we decided to drop were latitude, longitude, waterfront, view, The square footage of interior housing living space for the nearest 15 neighbors, and the square footage of the land lots of the nearest 15 neighbors. We chose these varaibles because our stakeholder is focusing on controllable factors for their own rennovation. Of the controllable variables, we were able to create a dummy variable associated with our conditon. Althought, we didn't use the zipcode data in our analysis , we were able to bin zipcode based off of rural and not rural. After we cleaned all of our data we labeled the final dataset as 'master_dataset.csv'. 


### Methods

We used Scikit Learn as well as Sci-py to validate that our model. 


## Modeling

## Baseline Model

Our first model was undoubtedly our baseline model. We used a baseline model to show us a progression of our iterations. The baseline model represented the average price of homes within King County within the time frame of 2014-2015


### Model 1

Our first model contained a list of all of the continuous variables we kept from the original data set. This included 'bedrooms', 'bathrooms', 'sqft_lot', 'floors', 'sqft_above', and 'yr_built'. We believed including these variables would be helpful because it would give us a holistic understanding of variables that take on a wide-array of values. Our intention with Model 1, was to see which potential variables would need to be dropped. The R-squared value for Model 1 was 0.481. This tells us that our x-variables (Bedrooms, Bathrooms, Sqft-Lot, Floors, SqFt-Above, and Yr-built) accounted for 48% of variability in our price or value of the house. We also analyzed the root mean squared error (RMSE) which was $258662. Outside of our R-Squared our RMSE is a metric error in our model. We chose RMSE over Absoulte Mean Squared Error because AMSE is highly biased for higher values. RMSE is better in terms of reflecting performance when dealing with large error values, and in this case, housing prices.


### Model 2

Our iteration of only having one variable (Square-Foot Living) in Model 2 was to see how this would effect our overall R-Squared value. From the heatmap correlation table we were able to see that Square-Foot Living was the variable that had the highest correlation (0.7) with price. After conducting the model, The R-squared value of Model 2 proved to be  0.498 which is an improvement on Model 1. This tells us that our x-variable (sqft_living) accounts for 50% of variability in home sale price. Our RMSE was $254336.12, a %1.7 increase from our prior model, showing us that this model is off by the aforementioned dollar amount.



### Model 3

Our third model wanted to take advantage of the recursive feature elimination that we conducted after model 1 in order to prioritize which variables would be the most effective to keep in our model. Recursive feature elimination is a feature selection method that fits a model while also removing the weakest features until the specified number of features to keep. We decided to keep six features in our model, dropping the lowest two. Rennovations are expensive and considering the most important variables will undoubtedly help our homeowner narrow down their priorities. We also included oour categorical variable of condition allowing us to see how a baseline status and overall up keep of a home can contribute to the overall price.   The R-squared value of Model 3 is 0.531 which is an improvement on Model 2. This tells us that our x-variables account for 53% of variability in house sale price. However, multicollinearity between bathrooms and sqft_living might have played a role in increasing this metric. 




### Model 4

From the heat map analysis, we wanted to see which variables had high multicollinearity. Multicollinearity occurs when more than one independent variable is highly correlated with another one in the regression model. An independent variable can be predicted from another independent variable in a regression model, which can convey some inaccuracies in the overall dataset. From our heat map we saw high multicollinearity between bathrooms and sqft_living, so we decided to feature engineer a ratio of floor to bathrooms to compensate for that factor. The R-squared value of Model 4 is 0.535 which is an improvement on Model 3. This tells us that our x-variables account for 54% of variability in house sale price. 

### Final Model

For Model 5 decided to add yr_built to the independent variables used in Model 4 as we anticipated that we could improve our model by taking the age of the home into account. yr_built was also ranked as the third most important variable during our recursive feature analysis. Ultimately, our final model explored the continuous independent variables of bedrooms, floor_to_bath, sqft_living, and yr_built as well as the categorical independent variable of condition. Our final model was built to optimize R-squared with as few features as possible. 



## Regression Results

Ultimately the R-squared value of Model 5 (our final model) is 0.564 which is best for all the models run. This tells us that our x-variables account for 56% of variability in house sale price with a root mean squared error of $240,146.63. In terms of feature coefficients with all other features held constant, home values drop by $62,863.31 for every 1 bedroom, increase $60,136.22 for every 1 unit increase in floor-to-bathroom ratio, increase $347.16 for every additional square foot, increase $2,245.52 for every year the house ages, decrease $7,7720.71 if categorized as poor condition, decrease $69,601.81 if categorized as fair condition, increase $2,779.43 if categorized as good condition, and increase $4,6333.11 if categorized as very good condition.



### Post Model Assumptions

As a means of validating our model, we tested for the assumptions of linear regression. These assumptions include, Linearity, Multicollinearity (checked before modeling), a Normal Distribution of Errors, and Heteroskedasticity or a lack of trend in errors. 







### Conclusions and Key Takeaways






## For More Information
View the full analysis via the [Jupyter Notebook](https://github.com/sgchatrathi/Real-Estate-Project-analysis/blob/main/Main%20Notebook.ipynb).
View the full presentation via the our [slides](https://github.com/sgchatrathi/Real-Estate-Project-analysis/blob/main/Presentation.ipynb).








