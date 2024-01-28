# Eigendecomposition
Decompose $n * n$ matrix of real values into product of several matrices.


# Principle Components Analysis (PCA)

## Overview
### Linear Projection
into Principal components, new attributes defined as linear combinations of original attributes.
### Minimizes reconstruction error:
* Minimize information loss
* Tends to preserve variance
* tends to preserve distance between data items
### Applications
* Data compression
* dimensionality reduction
* visualisation

## Basic Idea
* linear projection -> preserve most important information about data
* find components with highest variance
* components with small variance -> dominated by noise

## Principal components
* Eigenvectors
* linear combination of original attributes
* corresponding eigenvalues indicate proportion of variance
* selected subset forms lower-dim. data space

## Summary
PCA performs rotation of the data set X in d-dimensional data space into k-dimensional output space where coordinates are orthonormal and correspond to directions of largest variance in X

\+ produces explicit new attributes (explainable)
\- strictly linear projection
\- assumes that data shows a high signal-to-noise ratio

# Multidimensional Scaling (MDS)

## Basics
- meta-algorithm
- allows non-linear transformation
- project data onto low-dimensional space
	- usual 2-dimensional space
- try find mapping -> $p \sim d$
	- $p$ = proximity in data space
	- $d$ = distance in output space
- measure quality of mapping via error function $\mathbb{E}$

## Measuring the Error
* Raw Stress
* Kruskal's Stress
* Sammon's Mapping

General considerations
* Stress is badness-of-fit measure depending on
	* $n$ number of data points -> higher $n$ higher stress
	* $k$ dimensionality of the MDS (output) space -> higher $k$ lower stress
	* properties of data -> higher noise higher stress

## Judging quality of mapping
* Shepherd Plot
	* Plot distance $d_{ij}$ versus original prox. $p_{ij}$
