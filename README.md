# Transfer Entropy

Implementation in python3 of transfer entropy statistic between two time series.
Transfer entropy from Y to X, where X,Y are two random processes, is an asymmetric statistic measuring the reduction in uncertainty for a future value of X given the history of X and Y. Or the amount of information from Y to X. Calculated through the Kullback-Leibler divergence with conditional probabilities.

- refer to `test_TE.ipynb` as a reference on the usage of `transfer_entropy(X, Y, delay)` and examples with different cases

- plot of different TE (Y to X) values for a timeseries X generated from two other timeseries Y and K with a lag and some weight coefficients, where: $ X[t] = W_Y \cdot Y[t-t_{LAG}] + (1- W_Y) \cdot K[t-t_{LAG}]$ (see `test_TE.ipynb` for the associated code).

![png](README_files/fig1.png)
