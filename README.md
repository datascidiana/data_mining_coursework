# data_mining_coursework
This repository contains my projects developed within the Data Mining course at Illinois Institute of Technology.

In homework 1 (**data visualization, imputation, PCA**):
- Plotted the distribution of survival conditional on age and gender from the titanic dataset from Seaborn. 
- Imputed missing values using the imputer from Scikit in the auto-mpg sample dataset from the UCI Machine Learning Repository. Analyzed which type of imputation resulted in the lowest variance.
- Performed PCA using the Scikit Decomposition component on the iris sample dataset and calculated the percentage of variance explained by each of the Principal Components.
- Plotted a projection of each feature onto the 1st Principal Component against the original feature itself, to analyze which pair of features show a closer relationship to PC1 using Matplotlib. Then, I calculate the correlation coefficient between the pair of features I selected and their projections onto PC1 to see if the result agrees with the visual inspection.
- Investigated how many principal components need to be selected to capture > 95% of the variance of the original data.

In homework 2 (**decision trees**):
- Induced a set of binary Decision Trees on the iris sample dataset. Analyzed which depth values resulted in the highest Recall and why, which value 
resulted in the lowest Precision and why, which value resulted in the best F1 score.
- Induced a binary Decision Tree on the Breast Cancer Wisconsin (Diagnostic) sample dataset from the UCI Machine Learning Repository. Calculated the Entropy, Gini, Misclassification Error, Information Gain. Analyzed what is the feature selected for the first split, and what value determined the decision boundary.
- Performed PCA dimensionality reduction and induced a binary Decision Tree. Analyzed the effect of using PCA on the performance of the model.
- Simulated a binary classification dataset with a single feature using a mixture of normal distributions with NumPy. Induced a binary Decision Tree, and obtained the threshold value for the feature in the first split. Then I analyzed how did this value compare to the empirical distribution of the feature.

In homework 3 (**association rules**):
- Generated Frequent Itemsets from the Online Retail dataset from the UCI Machine Learning Repository using the apriori module from the MLxtend library, for transactions in France. Created association rules. 
- Calculate the binary correlation coefficient Φ for the Chocolate Coffee and Chocolate Cake items in the Extended Bakery dataset (75000-out2-binary.csv). Analyzed whether these two items are symmetric binary variables, by providing supporting calculations. Analyzed whether the association rules {Chocolate Coffee} =⇒ {Chocolate Cake} would have the same value for Φ as {Chocolate Cake} =⇒ {Chocolate Coffee}?

In homework 4 (**clustering**):
- Imputed missing values and performed Hierarchical Clustering on the auto-mpg sample dataset from the UCI Machine Learning Repository. 
- Performed a K-Means analysis on the Boston dataset. Chose an optimal number of clusters K by choosing the best Silhouette Score.
- Performed a K-Means analysis on the wine dataset. Calculated the Homogeneity/Completeness for the optimal K number and analyzed what information do each of these metrics provide. 

In homework 6 (**recommender systems**):
- Built a user profile in terms of movie preferences using the Movielens 100k dataset (ml-100k.zip). Quantified the similarity between user profile and a specific movie to assess the similarity between user's preferences and the type of movie.
- Predicted the rating for a movie from a user based on the average rating of the users with similar profiles.
