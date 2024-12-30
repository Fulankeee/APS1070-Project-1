# APS1070 Project 1 - Basic Principles and Models
-	Use of Panda: pd.concat; pd.DataFrame; 
-	Use of Numpy: np.where; np.arange
-	Use of matplotlib.pyplot: plt.plot;
-	Use of sklearn:
sklearn.model_selection - train_test_split; cross_validate; GridSearchCV(for tuning use)
sklearn.neighbors – KneighborsClassifier
sklearn.tree – DecisiontreeClassifier
sklearn.preprocessing - StandardScaler
-	Use of seaborn: sns.lmplot (visualize two groups data) 
-	Python Basics: .iloc; .loc; map(lambda p: ‘formula of p’); .append

Part 1 - Data Cleaning and Visualization
-	Work with the California housing dataset. This dataset was derived from the 1990 U.S. census.
-	The target variable is the median house value for California districts, in $100,000.
-	Add dummy variable 1 or 0 (if the target value is below the median or equal to the median) or 1 (if the target value is greater than the median).
-	Split the data to training and testing.
-	Visualize and compare the data with and without standardization.

Part 2 - KNN Classifier
-	Using KNN Classifier with cross-validation and tune the best k (numbers of neighbors) from 1 – 1000 according to best cross-validation accuracy.
-	Analyzing problem of underfitting and overfitting.

Part 3 - Feature Selection Function of KNN Classifier based on Tree Importance
-	Design a function of “Feature selector” that accepts dataset (X_train , y_train) and a threshold of 95% as inputs. The function includes:
	Fitting decision tree classifier to gain feature importance and get the importance score in order. Then remove one of the least important feature until only one feature left or if the mean cross-validation accuracy after tuning k is bellow (full_feature_score * 95%).
	Starting with the best KNN score of full model, then get the best KNN neighbor count and KNN accuracy as output

Part 4 - Explore the effect of Standardization
-	Note: We cannot compute the mean or standard deviation of the whole dataset to standardize it as we cannot touch the testing data while training models.
-	Standardization helped to stabilize accuracy.

Part 5 - Decision Tree Classifier
-	Train a decision tree classifier on the standardized dataset.
-	Tune the max_depth and min_samples_split parameters of the tree using cross-validation.

Part 6 – Test Data

