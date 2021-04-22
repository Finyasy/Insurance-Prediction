# Insurance-Prediction
Insurance prediction using machine learning.

# Zindi-Competition-Challenge-Insurance-Prediction-
You have been appointed as the Lead Data Scientist to build a predictive model to determine if a building will have an insurance claim during a certain period or not. You will have to predict the probability of having at least one claim over the insured period of the building.The model will be based on the building characteristics. The target variable, Claim, is a:  {1} if the building has at least a claim over the insured period. {0} if the building doesn’t have a claim over the insured period.

The objective of the hackathon is to predict the probability of having at least one claim over the insured period of the building. The data set consist of ((7160, 14), (3069, 13)) training rows, training columns, test rows and test columns.

# Tips to Get Started
1.Perform explanatory data analysis(EDA)

2.Area Under Curve metrics is to predict probablities(model.predect_proba()[:,1])

3.F1_score metrics is for perfect (0,1)

4.Always find a good baseline

5.Never stick to one Encoding method(always try to see the best first)

6.Feature engineering and Feature Selection are very important

7.Domain expertise can go a long way to have a better features

8.Always start with small features

9.Ensemble tricks also improve score to win

My approach is as follows:
# Exploratory Data Analysis(EDA)
Performing initial approach on data helps to discover patterns,spot anomalies and to test hypothesis and check assumptions with the help of summary statistics and graphical representations.
*Examples of python functions used in EDA*

a)df.shape----->It gives the total number of rows and columns in our dataset(df)

b)df.info------->It is also a good practice to know the columns and their corresponding data types,along with finding whether they contain null values or not.

c)df.describe------>The describe() function in pandas is very handy in getting various summary statistics.This function returns the count, mean, standard deviation, minimum and maximum values and the quantiles of the data.

d)unique() function

e)value_counts() function 

f)“.corr()” function can visualize the correlation matrix using a heatmap in seaborn.It’s a good practice to remove correlated variables during feature selection.

g)A box plot (or box-and-whisker plot) shows the distribution of quantitative data in a way that facilitates comparisons between variables.The box shows the quartiles of the dataset while the whiskers extend to show the rest of the distribution.The box plot (a.k.a. box and whisker diagram) is a standardized way of displaying the distribution of data based on the five number summary:Minimum,First quartile,Median,Third quartile,Maximum.It helps us in detection of outliers in data

# MODEL BASELINE
A baseline is a method that uses heuristics, simple summary statistics, randomness, or machine learning to create predictions for a dataset. You can use these predictions to measure the baseline's performance (e.g., accuracy)-- this metric will then become what you compare any other machine learning algorithm against.

A baseline is the result of a very basic model/solution. You generally create a baseline and then try to make more complex solutions in order to get a better result. If you achieve a better score than the baseline, it is good.

Human baseline in machine learning provides a hint if a model is  a feasible solution for our problem.It offers some kind of "Ground Truth".It will tell you whether there is enough signal in the data to build a model with predictive capabilities.

# FEATURE ENGINEERING

