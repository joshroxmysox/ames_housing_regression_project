# Josh Slizinov Project 2



### Problem statement
Assessing the price of a home property the traditional way takes time and money. Can a linear regression model be developed to perform the evaluation as successfully as a human?

Success of the model will be determined by neg mean squared error, root mean squared error, and r2 score. The more accurate the model is, the more confidence we can have that a model can perform as well as a human.

## Description of data

Size: The initial size of this dataset is 2051 columns (not including header) by 81 rows.

You can find the data dictionary for this dataset at the following link: http://jse.amstat.org/v19n3/decock/DataDocumentation.txt
One thing to note in addition to the data dictionary: All columns that involved years (i.e. 192, 1950, 2000 etc.) that were used as features in these models were converted to age. Age was calculated by subtracting the year in question from the maximum year, which in this dataset is 2010. You can think of it as positive distance from 2010.

Target: Regression


## Model performance on training/test data

I fit 6 total models: 2 linear regressions, 2 lasso regression, 2 ridge regressions.
The scores for the three final models, which were one of each of the above were as follows (r2 scores):

Linear regression: 0.832; Lasso: 0.838; Ridge: 0.838

*GridSearchCV was used to determine optimal parameters for Lasso and Ridge.

I chose the linear regression model because I am more familiar with it and the difference in r2 score was not enough for me to pick the Lasso or Ridge models.


## Primary findings/conclusions/recommendations

I found that a linear regression model can predict home prices fairly well and had I had the knowledge I do now, at the beginning of the project, I could develop a linear model that is significantly better. Currently, I wouldn't recommend using this as a method to evaluate the price of a home, but a linear model can replace a human when estimating the value of a property.

## Next steps

The model already has a pretty good r2 score, but I believe with some mroe feature engineering and additional categorical variable exploration, I can improve the performance significantly. Additionally, more advanced models may return significantly better results.

I think a model like this can be applied to almost anything. If you wre to download sell data from ebay, you could probably estimate the price for many things without having to guess what people would pay for them.


Thanks for reading!



Link to video:

https://drive.google.com/file/d/1VyIeNxiByNNDKR8fVnjUT4TtEj0xXHUQ/view?usp=sharing