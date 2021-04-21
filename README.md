# data_mining_coursework
This repository contains my projects developed within the Data Mining course at Illinois Institute of Technology.

In homework 1:
- I plotted the distribution of survival conditional on age and gender from the titanic dataset from Seaborn. 
- Given the auto-mpg sample dataset from the UCI Machine Learning Repository, I used Imputer from Scikit 
to replace missing values in feature horsepower with NaN, mean, median, and mode, after which I analyzed which imputation resulted in the lowest variance.
I calculated summary statistics as well. 
- Given the iris sample dataset, I performed a PCA using the Scikit Decomposition component, and provided 
the percentage of variance explained by each of the Principal Components.
- Using Matplotlib I plotted a projection of each feature onto the 1st Principal Component against the original feature itself, to analyze
which pair of features show a closer relationship to PC1. Then, I calculate the correlation coefficient between the pair of features I selected
and their projections onto PC1 to see if the result agrees with the visual inspection.
- I calculated the total variance of the original features and the total variance of the four eigenvectors to conclude that total variance of the original features
should the equal to the the total variance of the four eigenvectors. I investigated how many principal components need 
to be selected to capture > 95% of the variance of the original data.

In homework 2:
- On the iris sample dataset I induced a set of binary Decision Trees with a minimum of 2 instances in the leaves, no splits of subsets 
below 5, and an maximal tree depth from 1 to 5. Then I analyzed which depth values resulted in the highest Recall and why, which value 
resulted in the lowest Precision and why, which value resulted in the best F1 score. I explained the difference between the micro/macro/weighted 
methods of score calculation.
- On the Breast Cancer Wisconsin (Diagnostic) sample dataset from the UCI Machine Learning Repository I induced a binary Decision Tree with a minimum of 2 instances 
in the leaves, no splits of subsets below 5, and a maximal tree depth of 2. I calculated the Entropy, Gini, and Misclassification Error of the first split, as well as 
the Information Gain.  I analyzed what is the feature selected for the first split, and what value determined the decision boundary.
- Then I induced the same binary Decision Tree as above (now using the continuous data) but performed a PCA dimensionality reduction beforehand.
Using only the first principal component of the data for a model fit, I compared the F1, Precision, and Recall of the PCA-based single
factor model compared to the original (continuous) data. I repeat the process using the first and second principal components. Using the Confusion Matrix, I calculated 
the values for FP and TP as well as FPR/TPR. Then I analyzed whether using continuous data in this case was beneficial within the model and how.
- I simiulated a binary classification dataset with a single feature using a mixture of normal distributions with NumPy. The normal distribution parameters 
were (5,2) and (-5,2) for the pair of samples. I induced a binary Decision Tree of maximum depth 2, and obtained the threshold value for the feature 
in the first split. Then I analyzed how did this value compare to the empirical distribution of the feature.

In homework 3:
- Given the Online Retail dataset from the UCI Machine Learning Repository, and using the apriori module from the MLxtend library, I generated
Frequent Itemsets for all transactions for the country of France. I found the itemset that has the largest support. I set the minimum support threshold to 5% 
and extracted frequent itemsets, used them as input to the association rules module. I used each of the confidence and lift metrics to extract 
the association rules with the highest values, respectively. I analyzed what are the antecedents and consequents of each rule, and whether the rule with 
the highest confidence is the same as the rule with the highest lift.
- Given the Extended Bakery dataset (75000-out2-binary.csv), I calculate the binary correlation coefficient Φ for the Chocolate Coffee and Chocolate Cake items. 
I analyzed whether these two items are symmetric binary variables, by providing supporting calculations. 
I also analyzed whether the association rules {Chocolate Coffee} =⇒ {Chocolate Cake} would
have the same value for Φ as {Chocolate Cake} =⇒ {Chocolate Coffee}?

In homework 4:
- Using the auto-mpg sample dataset from the UCI Machine Learning Repository and only the continuous fields as features, I imputed
any missing values with the mean, and performed Hierarchical Clustering with linkage set to average and the default affinity set to a euclidean. I set
the remaining parameters to obtain a shallow tree with 3 clusters as the target. I obtained the mean and variance values for each cluster, and compared 
these values to the values obtained for each class if we used origin as a class label. Then I analyzed if there is a clear relationship between cluster
assignment and class label.
- Using the Boston dataset, I performed a K-Means analysis on scaled data, with the number of clusters ranging from 2 to 6. I provided the 
Silhouette score to justify which value of k is optimal. I calculated the mean values for all features in each cluster for the optimal clustering, and analyzed 
how do these values differ from the centroid coordinates.
- Using the wine dataset, I performed a K-Means analysis on scaled data, with the number of clusters set to 3. Given the actual class labels, I calculated
the Ho- mogeneity/Completeness for the optimal k and analyzed what information do each of these metrics provide. 
