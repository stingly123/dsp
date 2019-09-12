[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

import numpy as np

pmf_1000 = thinkstats2.Pmf(np.random.random(1000))

thinkplot.Pmf(pmf_1000)

thinkplot.Config(xlabel='number 0-1',ylabel='probability of occurence')

#uniform distribution 


cdf_1000 = thinkstats2.Cdf(np.random.random(1000))

thinkplot.Cdf(cdf_1000)

thinkplot.Config(xlabel='number 0-1',ylabel='CDF')

#distribution is uniform.


