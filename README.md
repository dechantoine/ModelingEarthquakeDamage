# ModelingEarthquakeDamage
In this repository lies the complete, cleaned and commented notebooks I have produced for the competition 
*Richter's Predictor: Modeling Earthquake Damage* on [DrivenData.org](https://www.drivendata.org/competitions/57/nepal-earthquake/).

Based on aspects of building location and construction, my goal is to predict the level of damage to buildings caused by the 2015 Gorkha 
earthquake in Nepal. All the data have been previously anonymized and dataset are available on [DrivenData.org](https://www.drivendata.org/competitions/57/nepal-earthquake/data/)

I chose to present this work in 8 thematics notebooks.

### 1 - Exploration part. 1

This notebook presents basic statistics and plots produced with pandas in-built functions. Goal here is to become familiar with features
from this dataset: type, range, distribution, etc. Also, I identified several step for preprocessing.

### 2 - Exploration part. 2

This notebook deepen the exploration by looking for relations between features. My aim is to find ways to reduce dimensionality of 
this dataset later in preprocessing.

### 3 - Preprocessing

In this notebook the dataset is shaped to suit machine learning algorithms. Outliers from training set are removed, categorical features are
either dropped or grouped together and then one hot encoded, real features are scaled between 0 and 1, labels are also scaled between 0 
and 1 and some new statistical features are added. Also, I created 10 subsets (train,test) for crossvalidation.

### 4 - Regression

Since labels of this dataset are ordinal, it is possible to apply regression on it. Once regression is fitted, I have to find the optimum
boundaries to separate predictions in 3 bins. In this notebook, I fit linear regression, softmax regression, elastic net and degre 2 
polynomial regression (with some tricks to avoid lack of memory).

### 5 - Classifiers

### 6 - Multi Layered Perceptron

### 7 - Ensemble Learning

### 8 - Error and bias analysis of each algorithm
