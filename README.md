

Bayesian Changepoint Detection
==============================

Methods to get the probability of a changepoint in a time series. Both online and offline methods are availeble. Read the following papers to really understand the methods:


[1] Ryan P. Adams, David J.C. MacKay, Bayesian Online Changepoint Detection,
arXiv 0710.3742 (2007)

[2] Paul Fearnhead, Exact and Efficient Bayesian Inference for Multiple
Changepoint problems, Statistics and computing 16.2 (2006), pp. 203--213

[3] Xuan Xiang, Kevin Murphy, Modeling Changing Dependency Structure in
Multivariate Time Series, ICML (2007), pp. 1055--1062
    
To see it in action have a look at the [example notebook](http://nbviewer.ipython.org/urls/raw.githubusercontent.com/hildensia/bayesian_changepoint_detection/master/Example%20Code.ipynb?create=1 "Example Code in an IPython Notebook").

###Tips:
- The online version is basically a translation of the matlab version of the paper from
author [1] (found in matlab-implementation)
- The offline version is an implementation based on [2] and [3].
- Something conversation I found that might be interesting:
Q: Is it possible to make Ryan Adams algorithm [1] to work on multivariate data too?
A: The change should be relatively easy, but a bit time consuming. It's only updating the student t distribution to handle multivariate data correctly. 
