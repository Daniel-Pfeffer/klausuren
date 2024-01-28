# Feed-forward neural networks
Activiation functions:
* Sigmoid function: $f(x)=\frac{1}{1+e^{-x}}$
* ReLU activation: $f(x)=max(0,x)$
* SELU activation
Deep learning:
* Neural networks together with recent availability of very fast computer/massive data sets
* Multiple levels of sparse representation
Vanishing gradient:
* Gating
	* Most intermediate gradient values close to 0 or 1
	* Long Short Term Memory (LSTM)
	* Residual networks
* Normalisation: distorts gradient, increases noise
* Clever initialisation helps
## Summary
* Neural Networks powerful ML method
* Learn increasingly abstract representation of input
* Flexible method
* Different architectures possible
	* Simples: MLP, feed-forward, fully-connected network
* Computationally costly - typically done on GPUs
* Trained by backpropagation algorithm

# CNN
Images of input -> before training, convolute images
* trained with SGD
	* batch sizes: 32 (images)
	* update: propagate a batch of images through CNN then backpropagate the error, and update weights
	* epoch: running though the training data set once
	* Backward pass typically does not have to be implemented -> automatic differentiation

# RNN
sequential data: Data point has "time dimension"

* forward pass: transformation is applied in each time step
* backward pass
	* analog to MLP
	* time = depth
	* errors backpropagated through layers
	* update: accumulation of errors over time