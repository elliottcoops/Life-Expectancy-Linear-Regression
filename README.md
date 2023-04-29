# Life-Expectancy-Linear-Regression

This is a simple model which I have developed in my quest to become omniscient in machine learning.

## What is the model doing

The model is predicting life expectancy based on years in education from about 180 countries around the world.

The dataframe is split into one in which the data is based only of that from 2015.

The dataframe is split into testing and trainig data on an approximate 60/40 split, which is what I found to give the lowest mean square error when playing
around with it.

The end result from this was getting to a MAE of: 3.6342687846127224

## Interesting points

The data is split into training and testing by taking a random sample from the dataframe, using `df.sample(..)` and is then split into a numpy array using `np.split(..)`.

I was able to split the rows into x data and y data, or features and label/target by using the function `getxy(..)`.
x labels and a y label is passed in, and the values are returned in a numpy 2d array.
