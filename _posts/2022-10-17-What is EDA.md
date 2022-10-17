## What is EDA?
EDA is known as Exploratory Data Analysis.  The overall goal of EDA (in my opinion) is to get a “feel” for the data.  What is the data trying to tell 
us? By understanding the data, it will help us determine what answers we can get from the data.  These “answers” can lead us to other
questions.

My strategy is comprised of two parts – First, Exploring the data while cleaning.  This is the most important part of my EDA process.
I say this because you don’t want to be halfway through a project and realize you missed something at the beginning of the process. Plus, we cannot analysis data until it has been cleaned, free of errors, and any questions addressed.

**Exploring the Data while cleaning**

1. Create an Excel spreadsheet or Word document to document your EDA process. You should save it in the directory of your project 
  or assignment.  This will be helpful, if you need to recreate your results in the future and a reminder as to what you did.
    1. Document any changes made to the data
    2. Document the main points from the steps below. 
    
2. What is the shape? 
    1. Number of observations? 
    2. Format?  Long or Wide?
    3. Is the data large enough in size?

3. Create a table describing the data set.
    1. Variable (column name)
    2. Data Type (Date, Continuous, Discrete, Character, etc.)
    3. Description of the variable
    4. Read any meta data or separate files on the data set.
 
4. Are there any missing values (blanks, NA, periods, etc.)?
    1. Ask yourself, why are they missing?
    2. Did participants just fail to answer or is there a bigger problem? 
    3. How are you going to address the missing information? 
        1. Impute it
        2. Remove it
        3. Leave it as is and try to work around it
    4. Do you need to consult with anyone else before deciding?
  
 5. Look at any date variable.
    1. Verify the date format is correct.
  
 6. Look at any variables (columns) that could be converted to factors.  
    1. Are the values consistent?
    2. Use ndistinct().  I’ve ran into situations where gender field contained M, F, Male, and Female.
  
 7. Based on step 3b – make any data type changes, if necessary
   
   
 **Next, Exploring the data with visualization and tools**
 
 8.  Summarize the data using functions such as summary() to get basic statistical information.
     1. Does the results make sense?
     2. Look at mean and median – Is the data skewed?
     3. Outliers?    Why do we have outliers?
  
 9.  Create contingency table to further explore the data

10. Plot the data to determine the distribution or shape.
    1. Referring to step 3, create a plot based on the data types being explored. 
        1. One variable
            1.  Histogram
            2.  Boxplot  
        2. Two (multiple) variables
            1.  Scatter plot
            2.  Bare Chart
            3.  Heat Map
            4.  Line Chart 
        3. Categorical variables
            1.  Bar Chart    
    2. What do you see?  Trends? Relationships?
   
11.  Use correlation to confirm or disaffirm any relationships.
      1. 	Using cor(), ggpairs(), and/ or ggcorr().  


From the outline above, after all of step one, I think the most important thing is plotting and looking the distribution.  Visually, 
it’s easier to see patterns and trends in the data, which can help answer questions.

As you are completing the EDA, you are trying to look for relationships and ask why those relationships exist in the first place.  
Honestly, I think that is the only reason to complete EDA.


Thank again for reading my blog post.  I am working on my narrative and trying to find my voice.
