Question 1

c + 0.5c + 0.0.25c = 1
1.75 c = 1
c = $\frac{1}{1.75}$
(b)
Pr[N<=1] = $\frac{1}{1.75} \times 1 + \frac{1}{1.75}\times0.5$

Q3.

Dont need to use Bayes, just normal probability can already

IN this case we use conditional probability to check if the data makes sense

Q5, just do the following

```python
scipy import stats
mu = 30
sigma = 1.8
lower = 28
upper = 33
p_upper = stats.norm.cdf(upper,mu,sigma)
p_lower = stats.norm.cdf(lower,mu,sigma)
p = p_upper - p_lower
```


Q7
**f A and B are correlated, but they’re actually caused by C, which of the following statements are correct?  
a) A and C are correlated  -- if caused, then def correlated
b) B and C are correlated  -- if caused then def correlated
c) A causes B to happen  Not
d) A causes C to happen Not**

Q8.
**ave the flu, while the other 10% are sick with COVID-19. Let F stand for an event of a child being sick with flu and  
C stand for an event of a child being sick with COVID-19, therefore, we have P[F]=0.9 and P[C]=0.1. Assume for  
simplicity that a child is either with flu or with COVID-19, not both.  
  


