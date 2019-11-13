Apply KNN(brute force version) on these feature sets
Set 1: categorical, numerical features + project_title(BOW) + preprocessed_essay (BOW)
Set 2: categorical, numerical features + project_title(TFIDF)+ preprocessed_essay (TFIDF)
Set 3: categorical, numerical features + project_title(AVG W2V)+ preprocessed_essay (AVG W2V)
Set 4: categorical, numerical features + project_title(TFIDF W2V)+ preprocessed_essay (TFIDF W2V)

Hyper paramter tuning to find best K
Find the best hyper parameter which results in the maximum AUC value
Find the best hyper paramter using k-fold cross validation (or) simple cross validation data
Use gridsearch-cv or randomsearch-cv or write your own for loops to do this task

Representation of results
You need to plot the performance of model both on train data and cross validation data for each hyper parameter, as shown in the figure
Once you find the best hyper parameter, you need to train your model-M using the best hyper-param. Now, find the AUC on test data and plot the ROC curve on both train and test using model-M.
Along with plotting ROC curve, you need to print the confusion matrix with predicted and original labels of test data points
Select top 2000 features from feature Set 2 using `SelectKBest` and then apply KNN on top of these features
