# DifferentialNearestNeighbours
Implementation of the dNN algorithm [2205.08434], a C^1 generalisation of kNN regression, for now up to approximate first order. Eventually will add an experimental dNNClassifier and expand to a C^k approximation for k>1 (smoothness "k" unrelated to the "k" of kNN). Multivariable regression is supported.

Contains example of plots of the test error as n_neighbors and n_derivative_neighbors varies on a toy dataset. n_neighbors behaves as expected, with bias and variance "spoiling" the test error for large and small n_neighbors values respectively and an optimum somewhere inbetween, whereas in this example increasing n_derivative_neighbors seems to monotonically decrease error.  

![plot](/img/dNNRegressor_heatmap.png)
