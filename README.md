# SeattleAirBNB
Seattle Air BnB analysis for Udacity  

## Project Overview  
This project is part of the Udacity DataScientist NanoDegree.  
In it we will analyze a Seattle AirBnB dataset (Sourced from Kaggle) two answer three question.
  1. How does the listing's summary, space, and description length impact the listing's annual income.  
  2. Does local vs distant hosts impact the average sentiment of the listing's reviews  
  3. What factors lead to a listing's rental rate

## Data Overview  
The data was sourced from [Kaggle](https://www.kaggle.com/datasets/airbnb/seattle/data)  
The data is three csv files:
 * Listings
 * Reviews 
 * Calendar (2016)  

It should be noted that the data was originally part of Airbnb Inside and sourced from [here](https://insideairbnb.com/get-the-data/)

## Libraries Used 
For this project, we used the libraries:  
 * numpy
 * pandas  
 * matplotlib  
 * copy  
 * textblob  
 * re  
 * sklearn

## Files  
Other than the data files, the only file used in this analysis is DGray_SeattleAirBNB.ipynb, the jupyter notebook where the python was written and run.  

## Results  
For this analysis we asked three questions.  

1) How does the listing's summary, space, and description length impact the annual income  
Using both a scatter plot and correlation calculation, we find minimal relationship between a listing's annual income and the summed length of their summary, space, and description fields.  
The scatter plot showed know relationship, and the correlation was -0.03   
So essentially 0

2) Does local vs distant hosts impact the average review sentiment  
Again we calculated correlation between the target (review sentiment) and the input variable (binary flag of whether or not the host lives near the listing)  
The correlation came out to 0.0007 So essentially zero.  
We also plotted a histogram and found that while there are many more local hosts vs distant hosts, they follow similar distributions.  
3) What factors lead to a listing's rental rate  
For this question, we were largely using existing variables (other than the target variable) so there was less feature engineering than we saw in the previous questions.  
&nbsp;&nbsp;&nbsp;&nbsp;The only new feature engineering would be converting categorical variables to dummy variables (also called one hot encoding)  
However, since we are using a large number of columns, we do have a bit more data cleansing that we had to perform (dealing with Nulls, etc)  
After the data prep was done, made a linear regression model, as a way to get variable impact via their coefficients.    

| Variable  | Blag |  
| --------- | ---  |  
| blig      | 12   |  
| blig      | 12   |  





blig

## Acknowledgements


[here](https://insideairbnb.com/get-the-data/)
