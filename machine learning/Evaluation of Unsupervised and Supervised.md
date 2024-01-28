# Evaluation of Clustering and Data Projection
* Intra-cluster distance
* Inter-cluster distance
* Ration: between-cluster / within-cluster
* Neighbourhood preservation ratio (NPR)
* Mean Quantisation error
	* Avg. distance between data items and corresponding cluster centre
* Topographic error
	* Proportion of all data items for which first and second BMUs are not adjacent
* Shepherd plot
	* Plots distance in output space versus original distances in input space
# Evaluation of Classification
* Learning/Training -> Validation -> Testing
* With what to train/test?
	* Random selection
		* randomly select instances for training set, rest testing
	* K-fold cross validation
		* Partition into k subsets k-1 for training, remaining testing
		* Avg errors of all subsets as test
	* Leave-one-out cross validation
		* 1 datapoint for testing -> small data
## Evaluation Criteria
+ Predictive accuracy
+ Efficiency
	+ Training
	+ Testing
+ Robustness: Handling noise/missing values
+ Scalability: Increasing amount of data
+ Interpretability: Insight provided by model
+ Compactness: size of tree, number of rules, number of parameters

## Basic performance measures
Contingency table:
![[perf_measure.png]]
TPR - Recall: $recall = \frac{TP}{TP+FN}$
Precision: $precision=\frac{TP}{TP+FP}$
FPR/FAR: $FPR = \frac{FP}{FP+FN}$
Accuracy: $accuracy= \frac{TP + TN}{TP + TN + FP + FN}$
F: $F=2*\frac{precision * recall}{precision + recall}$

### Confusion Matrix
Extended variant of contingency table for larger number of classes

## Receiver operator characteristics (ROC)
* confidence score / discrimination threshold for classification
* Plot recall (TPR) vs false alarm rate (FAR)

## Area under the curve (AUC)
* Area under normalized ROC curve
* Single number to measure quality of classifier

# Evaluation of Regression
* Mean absolute error (MAE): Quantifies how close predicted values are to true values. No distinction between "severity" of errors
* Root Mean squared error (RMSE): Penalises large prediction errors disproportionately
* $R^2$ statistics, closeness of the ground truth data to regression function. Describes percentage of variance of the data
