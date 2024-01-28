# Clustering
Unlabled input data automatically categorised into number of clusers without knowing clusters beforehand

# K-means
* Simplest clustering algorithms
* Uses Expectation Maximization strategy
* Algorithm
	* determine nearest cluster centre for each data instance
	* Adapt all cluster centre with mean of data instance of children
\+ easy to implement
\+ usually very fast
\+ suited for large datasets
\- determine a good number of clusters is difficult
\- assumes exactly $k$ clusters in dataset
\- heuristic
\- cannot guarantee to converge to global optimum
# Self-Organising Maps (SOM)

## Training / Learning
On-line/Off-line learning

Different topologies:
* Hexagonal Grid
	\+ tighter relationship
	\+ more connections
* Rectangular
	\+ easier to visually grasp
	\- diagonally neighbouring map units do not fit neighbourhood function
	
Initialisation:
* Random
	* Random values in same range as X
	* Randomly select data items from X
	\+ Fast
	\- Mapping not consistent for different runs
* Linear
	* perform Eigendecomposition of matrix
	\+ mapping consistent for different runs
	\- computationally more complex
	

## Visualization
* Attribute distributions
	* Component Planes
	  ![[clustering - component planes.png]]
	* Bar Chars/Chernoff's Faces
	  each attribute value is displayed via bar in d-dimensional bar chart visualization
	  each attribute value is mapped to a specific property of Chernoff face
* Data distributions
	* SOM-grid: each data item is displayed
	* Smoothed Data Histogram (SDH): density of data items in an area [[Clustering - K-means, SOM#^5002e9]]
* Distance between map units
	* U-matrix: distance between units
	* Distance matrix: aggregated distance of model vectors to neighbouring units

### Smoothed Data Histogram (SDH)
* Summary
	* Visualisation of item density
	* Reveal larger clusters in data
	* Let data items vote for number of best matching units
* Architecture
	* Voting matrix -> size equals SOM size
* Parameter
	* Spread $S$, number of map units each data item can vote for
^5002e9
