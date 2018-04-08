[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> REPLACE THIS TEXT WITH YOUR RESPONSE
```python3
import sys
sys.path.append("./ThinkStats2/code")
import nsfg
import thinkstats2
import numpy as np
import thinkplot
%matplotlib inline


def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf.Mult(x, x)
        
    new_pmf.Normalize()
    return new_pmf

resp = nsfg.ReadFemResp()
actual = thinkstats2.Pmf(resp.numkdhh, label='actual')
biased = BiasPmf(actual, label='biased')
thinkplot.PrePlot(2)
thinkplot.Pmfs([actual, biased])
thinkplot.Config(xlabel='Number of children', ylabel='Probability Mass Function')
actual_mean=normal.Mean()
biased_mean=biased.Mean()
print ('actual Mean :',actual_mean)
print('Biased Mean :',biased_mean)
```
