Decision Trees: (16 marks) In this question, you will use the Wine dataset1, a popular
dataset to evaluate classication algorithms. The classification task is to determine, based
on various parameters, whether a wine quality is over 7. The dataset has already been
preprocessed to convert this into a binary classification problem (scores less than 7 belong to
the \zero" class, and scores greater than or equal to 7 belong to the \one" class). Each line

describes a wine, using 12 columns: the rest 11 describe the wine's characteristics (details),
and the last column is a ground truth label for the quality of the wine (0/1). You must not
use the last column as an input feature when you classify the data.

(a) (5 marks) Decision Tree Implementation: Implement your own version of the
decision tree using binary univariate split, entropy and information gain. ( WITHOUT using Scikit Learn/sklearn or other libraries)

(b) (5 marks) Cross-Validation: Evaluate your decision tree using 10-fold cross valida-
tion. Please see lecture slides for details. In a nutshell, you will rst make a split of the
provided data into 10 parts. Then hold out 1 part as the test set and use the remaining
9 parts for training. Train your decision tree using the training set and use the trained
decision tree to classify entries in the test set. Repeat this process for all 10 parts, so
that each entry will be used as the test set exactly once. To get the nal accuracy value,
take the average of the 10 folds' accuracies. With correct implementation of both parts
(decision tree and cross validation), your classication accuracy should be around 0.78
or higher.

(c) (6 marks) Improvement Strategies: Now, try and improve your decision tree
algorithm. Some things you could do include (not exhaustive):
• Use Gini index instead of entropy
• Use multi-way split (instead of binary split)
• Use multivariate split (instead of univariate)
• Prune the tree after splitting for better generalization
Report your performance as an outcome of ANY TWO improved strategies.
Deliverables:
