Gradient Boosting: (2 + 4 = 6 marks) 

In this question, we will explore the use of
pre-processing methods and Gradient Boosting on the popular Lending Club dataset. You
are provided with two files: loan train.csv and loan test.csv. The dataset is almost as
provided by the the original source, and you may have to make the necessary changes to make
it suitable for applying ML algorithms. (If required, you can further divide loan train.csv
into a validation set for model selection.)

Your efforts will be to Pre-process the data appropriately,
and then apply gradient boosting to classify whether a customer should be given
a loan or not. 

The target attribute is in the column loan status, which has values “Fully
Paid” for which you can assign +1 to, and “Charged off” for which you can assign -1 to. The
other records with loan status values “Current” (in both train and test) are not relevant to
this problem. You can see this link and this link to know more about the different attributes
on the dataset (but please use the provided data, there are several versions of the dataset
online.)
Your tasks are to do the following : 

(a) Pre-process the data as needed to apply the classifier to the training data (you are free
to use pandas or other relevant libraries. Note that test data should not be used for
pre-processing in any way, but the same pre-processing steps can be used on test data.
Some steps to consider:

• Check for Missing Values, and how you want to handle them (you can delete the
records, or replace the missing value with mean/median of the attribute - this is
a decision you must make. Please document your decisions/choices in the final
submitted report.)
• Check whether you really need all the provided attributes, and choose the necessary
attributes. (You can employ feature selection methods, if you are familiar; if not,
you can eyeball.)
• Transform Categorical data into Binary features, and any other relevant columns to
suitable datatypes
• Any other steps that help you perform better

(b) Apply gradient boosting using the function sklearn.ensemble.GradientBoostingClassifier
for training the model. You will need to import sklearn, sklearn.ensemble, and
numpy. Your effort will be focused on predicting whether or not a loan is likely to
default.
• Get the best test accuracy you can, and show what hyperparameters led to this
accuracy. Report the precision and recall for each of the models that you built.
• In particular, study the effect of increasing the number of trees in the classifier.
• Compare your final best performance (accuracy, precision, recall) against a simple
decision tree built using information gain. (You can use sklearn’s inbuilt decision
tree function for this.)
