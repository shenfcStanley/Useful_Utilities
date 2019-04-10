# Useful_Utilities
1. Feature selection: https://www.datacamp.com/community/tutorials/feature-selection-R-boruta

https://towardsdatascience.com/getting-data-ready-for-modelling-feature-engineering-feature-selection-dimension-reduction-39dfa267b95a 

Boruta: https://www.analyticsvidhya.com/blog/2016/03/select-important-variables-boruta-package/

2. Z-test, t-test, ANOVA python
3. data imputation python
4. How to control imbalanced data: Oversmapling and undersampling (SMOTE etc.)
https://www.kaggle.com/residentmario/undersampling-and-oversampling-imbalanced-data

A few comments:

https://stats.stackexchange.com/questions/60180/testing-classification-on-oversampled-imbalance-data

The option (1) is a very bad idea. Copies of the same point may end up in both the training and test sets. This allows the classifier to cheat, because when trying to make predictions on the test set the classifier will already have seen identical points in the train set. The whole point of having a test set and a train set is that the test set should be independent of the train set.

The option (2) is honest. If you don't have enough data, you could try using k-fold cross validation. For example, you could divide your data into 10 folds. Then, for each fold individually, use that fold as the test set and the remaining 9 folds as a train set. You can then average training accuracy over the 10 runs. The point of this method is that since only 1/10 of your data is in the test set, it is unlikely that all your minority class samples end up in the test set.


to be added...
