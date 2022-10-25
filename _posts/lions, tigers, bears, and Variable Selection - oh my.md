## **lions, tigers, bears, and Variable Selection - oh my!**
### Yes, Yes, the dreaded subject of variable selection for regression modeling.





Prior to researching and reading, I knew using forward, backward, and stepwise regression came with problems of overfitting, so we had to be careful.  Granted, the code was simple, and it produced lots of what seems like credible output. Now, I fully realize I (we) need to avoid using those techniques.  

[Curious as to why]( https://link.springer.com/content/pdf/10.1057/jt.2009.26.pdf)

My plan to determine which variables to use in a regression model is a continuation of EDA process discussed in my last post on 10/xx/2022 and includes many of the techniques mentioned in the article above.
1.	If we haven't done so already, I would define the problem. If you are working for an organization, shareholders and management may already have a question that needs to be answered.  Otherwise, ask yourself, what are trying to learn from the data?  But always keep in mind “the model must always follow the data, and not the other way around”
2.	After applying EDA / Cleaning techniques and noting relationships and trends, I would review any correlations between dependent and independent variables.  I would remove any variables that have collinearity relationships.  
3.	Still looking at correlations, I would look at values for the remaining variables.  I would select any relationships that are greater than absolute value of .5.  Again, we should not have any relationships with 1, -1.  I would use these variables as a baseline to compare its R-squared to the others.
4.	Next, I would determine the R-squared value with the full model.
5.	If our baseline model from step 3 is better than the model from step 4, I would fine tune the model. I would add one or two lesser variables to see if there is a significant increase in the R-squared.  Plus ask if it makes sense to see an increase in the R-squared.
6.	As an alternative, I would create a model with the response variable and highest non-collinear variable and determine the R-squared value.  Then, add variables to see if there is an increase in R-squared.
7.	Finally, I would select the variables from the model that produced the highest R-squared. Although, I didn’t talk about AIC, it should produce the lowest AIC.
8.	For this initial phase, I would not consider transformation, or adding polynomial or interaction terms.

After reading this you might be thinking - “didn’t you just complete the forward and backward stepwise?”  yes, I guess, I did.  But I have control over what variables are being added the model. Again, I think the hard work is the preparation before analysis.

Thanks for reading.  Good Luck with variable selection!
