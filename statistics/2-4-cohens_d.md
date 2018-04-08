[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)


```python3
# append path so we can find nsfg and thinkstats2

import sys
sys.path.append("./ThinkStats2/code")
import nsfg
import thinkstats2
import numpy as np
preg = nsfg.ReadFemPreg()
live = preg[preg.outcome == 1]

def Cohen_d(group1, group2):
    diff_mean = group1.mean() - group2.mean()
    
    N1, N2 = len(group1), len(group2)
    sigma1 = group1.var()
    sigma2 = group2.var()
    

    s = np.sqrt((N1 * sigma1 + N2 * sigma2) / (N1 + N2))
    d = diff_mean/s
    
    return d
    
firsts = live[live.birthord == 1]
others = live[live.birthord != 1]

firsts = live[live.birthord == 1]
others = live[live.birthord != 1]

Cohen_d(firsts.prglngth, others.prglngth)
```
