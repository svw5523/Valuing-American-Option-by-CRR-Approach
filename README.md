# Valuing American Option by CRR Model

### Introduction

The binomial approach is a discrete valuation model for European/American options on derivative securities, it was first suggested by William Sharpe in 1978. However, this methodology is normally associated with the paper by John Cox, Stephen Ross, and Mark Rubinstein in 1979.

The binomial approach also known as lattice approach can be used to value wide-range of general derivative securities and also to obtain exact formula by taking the limit in which the binomial tree converges to a continuum.

As proposed by Cox, Ross, Rubinstein, this method divides the time until option maturity into discrete intervals and presumes that, during each of these intervals, the price of the asset — e.g., the stock — follows a binomial process moving from its initial value, S, to Su (with probability p) or Sd (with probability 1-p). Given this set of share prices, the call/put can be valued by working backwards from maturity. [links here](https://medium.com/@polanitzer/cox-ross-rubinstein-1979-binomial-model-predict-european-and-american-options-prices-c0902039a951).

### Python code to reproduce the Cox, Russ, and Rubinstein Binomial Model

Inspired by the Cox, Russ, and Rubinstein (1979) binomial Model (CRR Model), this python notebook builds a simple and generalized pricing framework for the American call/put option by working in backwardation.

Generate the underlying stock price paths by binomial lattice implementation.

At the end, I did a separate test to compare the performance of Longstaff-Schwartz(2001) Least Square Monte Carlo (LSM) approach and Cox, Russ, and Rubinstein (1979) binomial Model, by sensitizing the option strike, maturity, and volatility inputs.
