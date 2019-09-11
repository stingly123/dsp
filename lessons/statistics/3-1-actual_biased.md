[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

resp = nsfg.ReadFemResp()

pmf_actual = thinkstats2.Pmf(resp.numkdhh)

pmf_biased = pmf_actual.Copy()

for value,p in pmf_actual.Items():
    pmf_biased.Mult(value, value)
    
thinkplot.PrePlot(2)

thinkplot.pmf(pmf_actual,label='actual')

thinkplot.pmf(pmf_biased,label='biased')

thinkplot.Config(xlabel='number of children',ylabel='count')


Means:

for num, p in pmf_actual.Items():\t
    mean_a = 0
    mean_a += num*p
    
for num, p in pmf_biased.Items():
    mean_b = 0
    mean_b += num*p
    
mean_b - mean_a
