Write Your Own Random Forest classifier WITHOUT sklearn /similar libraries (this should be relatively easy, given you have
written your own decision tree code) to apply to the Spam dataset [data, information].

Use 30% of the provided data as test data and the remaining for training.

Compare your results in terms of accuracy and time taken with Scikitlearn’s built-in random
forest classifier. 

(Note that you can’t use in-built decision tree functions to implement
your code. You can modify your decision tree code of the Assignment 1, or code a new
one, to implement a random forest. You can however use the inbuilt train test split of
sklearn to divide the data into train and test.)

(b) Explore the sensitivity of Random Forests to the parameter m (the number of features
used for best split).
(c) Plot the OOB (out-of-bag) error (you have to find what this is, and read about it!) and
the test error against a suitably chosen range of values for m. (Use your implementation
of random forest to perform this analysis.)
