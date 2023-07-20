# Prediction-of-wine-quality: Multi-class classification/regression - Ordinal Classification case

**Description:**
This datasets is related to red variants of the Portuguese "Vinho Verde" wine.The dataset describes the amount of various chemicals present in wine and their effect on it's quality. The datasets can be viewed as classification or regression tasks. The classes are ordered and not balanced (e.g. there are much more normal wines than excellent or poor ones).Your task is to predict the quality of wine using the given data.

A simple yet challenging project, to anticipate the quality of wine.
The complexity arises due to the fact that the dataset has fewer samples, & is highly imbalanced.
To overcome these obstacles & build a good predictive model to classify them, we need to oversample the dataset and try to approach the different ways.

This data frame contains the following columns:

Input variables (based on physicochemical tests):\
1 - fixed acidity\
2 - volatile acidity\
3 - citric acid\
4 - residual sugar\
5 - chlorides\
6 - free sulfur dioxide\
7 - total sulfur dioxide\
8 - density\
9 - pH\
10 - sulphates\
11 - alcohol\
Output variable (based on sensory data):\
12 - quality (score between 0 and 10)


**In this case:**
Practical applications of machine learning sometimes involve a situation where the target values exhibit an order among different categories. However standard classification algorithms cannot make use of this ordering information, because they treat each class attribute as a set of unordered values.

**Problem Definition**
In statistics, ordinal regression (also called “ordinal classification”) is a type of regression analysis used for predicting an ordinal variable, i.e. a variable whose value exists on an arbitrary scale where only the relative ordering between different values is significant.

Some examples of ordinal regression problems are predicting human preferences ( strongly disagree to strongly agree), predict a temperature (Hot, Mild, Cold), predict a book/movie ratings (1 to 5).

**Some Possible Approach**:
Some simple and naive way to tackle an ordinal regression problem is

- Treat it as a regression problem:
If the ordinal value represent interval or ratio and we have that original interval/ratio value we can just treat it as a regression problem
we fit a regression algorithms to the corresponding interval/ratio value that can be mapped to the actual ordinal value
Cons: we can’t use this approach if the ordinal value is not representing any continuous interval/ratio (like book/movie ratings), or if we don’t have the original interval/ratio value.

- Treat it as a standard classification problem:
We treat each ordinal value as an unordered set and fit a multiclass classification algorithm on it
Cons: lose the ordering information of each class because the standard classification algorithm treat each class as a set of unordered values


Please see more details in the Python file attached above!
