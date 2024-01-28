# K Nearest Neighbour Classification (KNN)
* Use most frequent class among unseen item's closest date point
![[knn.png]]
\+ No training required
\+ Intuitive and easy to exaplin
\+ Simple
\~ Does not produce model
\- very slow / computationally expensive

# Decision Trees
ID3 tree like in AI, traditionally classification but regression possible
* Classification
	* Assign to $x$ the class appearing most frequently
* Regression
	* Predict for $x$ the arithmetic mean of target value among samples associates with leaf node
* Overfitting
	* Max. tree depth above threshold
	* IG below threshold
	* Number of samples in node below threshold
* Pruning: Remove unnecessary deep subtrees
	* Reduced error pruning
		* Remove nodes, not leading to decrease of prediction performance
	* Cost-complexity pruning
		* Remove subtree which leads to the smallest increase of error per removed leaf
# Random Forest
* Ensemble method of i.e. DTs
* Multiple classifiers are trained to reduce variance
* Results of individual trees are aggregated
Learning:
* CART (Classification and Regression Trees)
* Only binary trees
* Grown to full depth without pruning