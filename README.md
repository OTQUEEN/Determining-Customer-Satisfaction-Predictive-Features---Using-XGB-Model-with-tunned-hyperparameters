# Determining-Customer-Satisfaction-Predictive-Features---Using-XGB-Model-with-tunned-hyperparameters
XGBoost model

# Introduction
Using the same dataset used for the decision tree model, the data is already cleaned and prepared for the modeling. Though `XGBClassifier` is capable of handing missing values in a datset. When it encounters a missing value at a node, it tries both left and right splits and learns the path leading to a higher loss for each node. This process is repeated when working on the testing data.
However, still use the final data prepared during the Decision Tree model process.

# Import packages

# Import relevant libraries and modules.

import numpy as np
import pandas as pd
import matplotlib as plt
import pickle

from sklearn.model_selection import train_test_split
from sklearn.model_selection import GridSearchCV
from sklearn import metrics

from xgboost import XGBClassifier
from xgboost import plot_importance
