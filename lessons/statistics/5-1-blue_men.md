[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

import scipy.stats

dist = scipy.stats.norm(loc=178, scale=7.7)

dist.cdf(185.42) - dist.cdf(177.8)

#around 34.3% of the US male population qualify.
