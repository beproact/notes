[[Set]]: Well-defined collection of objects
Enumerative: Just listing out the objects. {a,b,c}
Descriptive: Describing the objects {x| description on x} x *such that* description on x
Subset: A is a subset of B if every element of A is an element of B

Union: Set of element that are in either set $\cap$ "or"
Intersection: Set of elements that are in both $\cup$ "and"
Difference: Set of elements in first set but not in the second \
Complement: Set of all elements not in the given set, relative to the universal set $A^c$ "not"
Disjoint sets: $A\cap B = \emptyset$

Symmetric Difference: xor

Finite Set: Set with finite number of elements
Carnality: number of elements |A|

Permutations are ordered. Formula is $P(n,r)={\frac{n!}{(n-r)!}} = \binom nr r!$
Combinations are not ordered. Formula is $C(n,r)= \binom{n} {r} ={\frac{n!}{(n-r)!}}$

###### Perspectives of Probability
Frequentist: classical
- Probability is limit as probability gets bigger
- based on repeatable experiments
- relative frequency will converge to the theoretical probability
Bayesian: more modern
- Probability represent an individuals belief

Random experiment an experiement that:
- Can be repeated under the same condition
- whose outcome is subject to randomness
- whose exact outcome in a concrete realization cannot be determined ahead of time but the collection of all its outcomes can be understood
- If $\mathcal{E}$ is random experiment the collection of all its outcomes is called its sample space, denoted by $\Omega$


###### Probability Space
[[Probability]]

| Set Language            | Random exp. language      |
| ----------------------- | ------------------------- |
| universal set           | sample space              |
| subset of universal set | events                    |
| $\emptyset$             | imposssible event         |
| $\Omega$                | certain event             |
| Singleton               | Simple event              |
| Disjoint Set            | Mutually Exclusive events |
|                         |                           |

Event: Given an event is a subset of its samples space $\Omega$
- Examples:
	- impossible event $\emptyset$
	- certain event $\Omega$
	- simple event: event with only one outcome
	- composite event 
- Outcomes are different from events!
Outcomes: One of the possibilities 

Partition:
 - $E_{1}\dots E_{n}$ form a partition of $\Omega$ if
	1.$E_{i}\cap E_{j}=\emptyset$
	2.$\cup^n_{i=1}E_{i}=\Omega$
A and B are independent if $\mathbb{P}(A\cap B)=\mathbb{P}(A)\mathbb{P}(B)$
A and B are conditionally independent if $\mathbb{P}(A\cap B|C)=\mathbb{P}(A|C)\mathbb{P}(B|C)$
Bayes Theorem 
$$
\mathbb{P}(E_{i}|A)=\frac{{\mathbb{P}(A|E_{I})\mathbb{P}(E_{I})}}{\sum^n_{j=1}\mathbb{P}(A|E_{j})\mathbb{P}(E_{j})}
$$
Random Variable a map from $\Omega$ to $\mathbb{R}$. or $\Omega \to \mathbb{R}$
Discrete Random variable: If sample space $S_{X}$ is finite or countably infinite
- Comes from counting\
Continuous Random Variables:
- $S_{X}$ is uncountably infinite
- $\mathbb{P}(X=c)=0$ for all $c\in \mathbb{R}$
Probability Mass Function:$f_{X}(x)=\mathbb{P}(X=x)$ for all $x \in S_{X}$
Expected Value: $\mathbb{E}(X)=\sum_{x\in S_{X}}xf_{x(x)}$
Cumulative Distribution Function: $F_{X}(x)=\mathbb{P}(X\leq x)$
- Loosely Speaking CDF takes real value and outputs its percentile rank 




pmf: $f_{X}(x)=\mathbb{P}(X=x)$
- $f_{X}(x)\geq0$
- $\sum_{x \in S_{X}}f(x)=1$

Bernoulli means there are two outcomes 0 and 1, $S_{X}=\{0,1\}$

Expected values
- Discrete $\mathbb{E}(X)=\sum_{S_{X}}xf_{X}(x)$
- Continuous $\mathbb{E}=\int_{-\infty}^{\infty}f_{X}(x)dx$
Variance
- $Var(X)=\mathbb{E}(X^2)-\mathbb{E}^2(X)$
Standard Deviation
- $\sigma_{X}=\sqrt{ Var(X) }$
LOTUS
- $E(h(X))=\sum h(x)f(x)$
- $E(h(X))=\int h(x)f(x)$
Properties of expected value and variance
- $\mathbb{E}(aX+b)=a\mathbb{E}(X)+b$
- If $X\in[a,b]$ then $\mathbb{E}(X) \in [a,b]$
- $Var(aX+b)=a^2Var(X)$
Moment generating function
- $M_{X}(t)=\mathbb{E}(e^{tX})$
- $\frac{d^n}{dt^n}M_{X}(t)|_{t=0}=E(X^n)$

CDF Cumulative Distribution Function
- $F_{X}(x)=\mathbb{P}(X\leq x)$
- Right Continuous
- non decreasing
- Limit when $-\infty$ is 0
- Limit when $\infty$ is 1

[[Distributions]]
