# Fraud Detection using Unsupervised Machine Learning
This is the source code for the Credit Card Fraud Detection Project in Machine Learning.

In this Project we compare the results genereated by Isolation Forest Algorithm and Local Outlier Factor.

The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.The dataset used in the project is obtained from "Kaggle" which is an open source credit card database provider. 

# Packages:
(i)Sys(System-Specific parameters and functions):
This module provides accesss to some variables used or maintained by the interpreter and ti functions that interact strongly with the interpreter.


(ii) NumPy:
This is the fundamental package for scientific computing which adds support for large, multi- dimensional arrays,matrcies with large collection of mathematical functions to operate on arrays.

(iii) Pandas:
This is a BSD(Berkely Software Distribution) licensed package which is used in data manipulation and analysis. It offers data structures and operations for manipulating numerical tables and time series.

(iv)  Matplotlib:
This is a plotting library for python and an numerical extension for NumPy. It provides an object- oriented API for embedding plots i to applicatons using general purpose GUI tools like wxPython.

(v) Seaborn:
This is a data visualization library based on matplotliib. It provides an interface for drawing statistical graphics.

(vi) Scipy:
It is used for scientific & technical computations. It contains modules for optimization, linear algebra, intepolaton, image processing.

(vii) sklearn:
This is the simplest and efficent package for data mining and analysis.

Step 1- Building and Setting up the dataset: 

(i) Import all the necessary packages.

(ii) Load the data.

(iii) Explore the dataset.

(iv) Plot histogram for each parameter.

(v) Calculate Outlier Factor, Number of Fraud and Valid cases.

(vi) Finding correlation among the columns.

(vii) Format and filter the dataset.

Step 2: Applying Algorithms to the dataset.

Now that we have processed our data, we can begin deploying our machine learning algorithms. We will use the following techniques:

1. Local Outlier Factor (LOF):

The anomaly score of each sample is called Local Outlier Factor. It measures the local deviation of density of a given sample with respect to its neighbors. It is local in that the anomaly score depends on how isolated the object is with respect to the surrounding neighborhood.

2. Isolation Forest Algorithm:

The Isolation Forest algorithm isolates observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature. The logic argument goes: isolating anomaly observations is easier because only a few conditions are needed to separate those cases from the normal observations. On the other hand, isolating normal observations require more conditions. Therefore, an anomaly score can be calculated as the number of conditions required to separate a given observation.

The way that the algorithm constructs the separation is by first creating isolation trees, or random decision trees. Then, the score is calculated as the path length to isolate the observation.
