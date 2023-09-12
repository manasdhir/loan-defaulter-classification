I have used decision trees,bagging,boosting and random forests.
I am going to build a model that predicts if someone who seeks a loan might be a defaulter or a non-defaulter. We have several independent variables like, checking account balance, credit history, purpose, loan amount etc.
I have used decision trees to build this model, it uses gini impurity to build the tree which means that the gini impurity reduces for every branch of the decision tree.
First i have performed EDA on the data to label encode it and to make it fit for building decision tree model.
I have shown the accuracy of the model both with and without regularization.When the model is trained without regularization it tends to overfit on training data and performs poorly on the testing data.The importance of each variable or column being used for prediction is also shown along with a confusion matrix which visualizes the accuracy of the regularized model.
Then I have built a bagging model using the regularized and unregularized decision tree and compared their performance which shows that the unregularized model which is more complex has a higher accuracy for bagging.
While for boosting it is the opposite in which the simplest model which is the default setting - a decision tree with max depth as 1 has the highest accuracy.
After this I have built a random trees model as well with 12 max features which has the maximum accuracy as compared to all other models shown in the notebook.
