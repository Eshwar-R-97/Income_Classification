# Income_Classification
Will probably never touch the project again, but if you want to add to it, just add more data yourself or try out the input output to see if it guesses your income level. It's not insanely accurate and could obviously be better but this was a freshman year project. If you have any questions please reach out. 

## Based on the Exploratory Data Analysis and the final model results, we can see that features like the person's age, whether they are married, and especially the magnitude of their capital gain are some of the most influential features. We can also see that as expected the random forest model is the best model because of the high volume of categorical variables and the correlation between each of the variables and income found in the EDA.

# Key Findings:
## The final selected model produced results of an Accuracy of: 0.86, Precision of: 0.79, Recall of: 0.597, and an F1 score of: 0.68.

# Problem Resolution:
## Based on these results the model is determined to be useful to the original intended purpose of classifying people's incomes to be used on online sites like amazon for recommendation algorithms based on income. The main thing to avoid in this use-case would be recommending an expensive product to someone with a lower income, which in this case is a false positive.
## To minimize false positives, we want to maximize precision, and the best performing model produced a precision of 79%, which is high enough to be used by businesses to assist their recommendation algorithms by adding data to seperate demographics.  

#Deployment:
##The model would be used to take data from users until enough data has been gathered to make an accurate prediction on their income level based on this model. From that either budget products will be recommended to lower income users and recommend higher end products to higher income users to ideally match users with products more efficiently.
##New interference of the model would happen everytime a user logs online, so that ads and products can be catered to their income level
##The results on this model will be automatically used in a recommendation algorithm to then recommend a product to user, and besides testing, no results of this model will be directly looked at, and instead are automated and put into a recommendation model.
##Every large shift in the economy, for example when minimum wage is changed, the model will have to be retrained on new data and shifted to adjust for what the economic standard for income is. The model will generally be accurate for a significant amount of time, as while income shifts the speed at which the standard of income shifts is not fast enough to make this model obsolete within less than a decade.
# Improvements:
## Some potential improvements could be to increase the size of the training data and test the usefulness of implementing multiple models at once. By this I mean training multiple models on the data and assigning each model weights for the classification problem. On top of this, some features could be added to the data like their device used to log onto the internet, as those features related to how they are interacting with the enviornment could be useful in determining income. Ontop of this more types of models could be tested to see if another model could produce a higher recall than the low recall of the random forest model without causing a drop in precision. This project could also be made to work with less features and adjusted weights, dropping some features that had low weights in this model.
