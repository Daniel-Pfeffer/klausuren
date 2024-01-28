# Kernels
* Computational methods, relying on kernel functions
* Types:
	* Support Vector Machines
	* Kernel PCA
	* ...
* Maps 2 vectors to a scalar reflecting their similarities
Kernel matrix/trick
* Kernel matrix is matrix of pairwise similarities of set of data points
* Kernel trick: avoid direct calculation of similarity 

## Kernel functions
* Should be designed to represent similarity of samples
	* Designed by ML practitioner
	* Standard functions are available
	* Custom-designed for specific applications
* Standard in use
	* Linear $k(\boldsymbol x,\boldsymbol y)=\boldsymbol x\cdot \boldsymbol y$ 
	* Polynomial $k(\boldsymbol x,\boldsymbol y)=(\boldsymbol x\cdot \boldsymbol y +\beta)^\alpha$ 
	* Gaussian $k(\boldsymbol x,\boldsymbol y)=exp(-\frac{1}{2\sigma^2}||\boldsymbol x\cdot \boldsymbol y||^2)$ 
	* Sigmoid $k(\boldsymbol x,\boldsymbol y)=tanh(\alpha\boldsymbol x\cdot \boldsymbol y + \beta)$ 
\+ Easy to use, fast to train
\+ Robust training
\+ Well-regularized, robust
\- Similarity measure has to be hand-designed
\- Larger the dataset -> more problematic to train
\- Does not automatically allow for multi-class/task
