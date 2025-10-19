##### Discrete Distributions
###### Memoryless Property of Geometric Distrubitndodnuf
- $\mathbb{P}(X\geq s+t|X\geq t)=\mathbb{P}(X\geq s)$

###### Binomial
- $\mathbb{E}(X)=np$
- $Var(X)=np(1-p)$
If the length of the sequence is fixed and set to n and X counts successes, then $X\sim Bin(n,p)$
###### Negative Binomial Distribution
- number of failures until one sees the exactly r successes.
- $f_{X}(x)=\binom{x+r-1}{r-1}p^r(1-p)^x,x=0,1,2\dots$
- Almost like doing r concurrent geometric series

###### Hypergeometric Distribution
- Consider a population with N objects with a binary feature that each object either has or not. Further exactly M objects in the population have this feature. Now consider a random sample of size n from the population. Let X be the number of objects in the sample that possess this feature, then X is said to have a hypergeometric distribution with parameters N,M,n.
- M success and N-M failures in population
- Take a sample size n from the population.
- $f_{X}(x)=\frac{\binom{M}{x}\binom{N-M}{n-x}}{\binom{N}{n}}$
- $\mathbb{E}(X)=n\frac{{M}}{N}$
- $Var(X)$
- If N is very big and $\frac{M}{N}$ is fixed this is binomial distribution

###### Poisson Distribution
- Random variable X is said to have a Poisson distribution with parameter $\lambda$ where $\lambda>0$ if its pmf is given by $f_{X}(x)=\frac{{e^{-\lambda}\lambda^x}}{x!},x=0,1,2,\dots$
- $\mathbb{E}=Var(X)=\lambda$
- Examples
	- Number of typos on a page in a given book
	- Number of cracks per mile on I-75
	- Number of car accidents per day a a given intersection
- Space or time constraint
- $P(X=0)=?=e^{-10}*\frac{10^0}{0!}=e^{-10}$
- Can approximate binom with poisson if n is large >100 and np is small <10
##### Continuous Distributions
###### Uniform Distributions
- $f_{X}(x)=\frac{1}{b-a}\mathbb{1}_{[a,b]}(x)$
- Like continuous equally likely outcome model
- $\mathbb{E}(X)=\frac{{a+b}}{2}$
- $cdf=\frac{x-a}{b-a}$ from a to b
- $Var(X)=\frac{(b-a)^2}{12}$
- $mgf= \int_{a}^be^{xt}\frac{1}{b-a}dx=\frac{e^{tb}-e^{ta}}{t{(b-a)}}$
###### Exponential Distribution
- $f_{X}(x)=\lambda e^{-\lambda x}\mathbb{1}_{[0,\infty)}(x)$
- almost like continuous version of geometric
	- How long a light bulb can burn before it breaks