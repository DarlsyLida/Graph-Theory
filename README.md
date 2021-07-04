# Graph-Theory
Graph theory can be used as a tool for investment in the stock market: both as a way of predicting stock movements and for analysing market behaviour during major financial events (e.g. 2008 financial crisis, COVID).
The methodology: from time series of stock market data, we can created correlation matrices. These correlation matrices can be converting into adjacency matrices by thresholding (i.e. we turn correlations into 0s and 1s depending on their value). One major thing to look at is how to threshold effectively. Suppose we want to turn a correlation matrix C into adjacency matrix A. Then we can say

A(i,j) = 1 <=> C(i,j) > t

or

A(i,j) = 1 <=> C(i,j) < t

or

A(i,j) = 1 <=> t1 < C(i,j) > t2

The three cases lead to very different network structures, and in all case depend on the precise values of t, t1 and t2.

Once a network has been constructed you can look at:

Centrality...which nodes appear to most important?

Community structure...do certain groups of shares behave in similar ways?

Clustering coefficient...how does this change over time/choice of t, t1, t2?

You can look at different networks from different markets/time periods to look for patterns.
