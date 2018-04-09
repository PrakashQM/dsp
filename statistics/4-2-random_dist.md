[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
import sys
sys.path.append("./ThinkStats2/code")
import nsfg
import thinkstats2

import numpy as np
%matplotlib inline
import thinkplot
sample =np.random.random(1000)

pmf = thinkstats2.Pmf(sample)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='Random sample', ylabel='PMF')

cdf = thinkstats2.Cdf(sample)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random sample', ylabel='CDF')
```

Yes the distribution uniform is uniform.
