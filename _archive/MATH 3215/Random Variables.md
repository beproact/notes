Random variable X is a function that assigns a real numerical value
placeholder for some numerical value we care about in a random experiment.
Random variable is like a map from sample space to the real line.
$$
X\to \mathbb{R}
$$
Notation: $X,Y,Z...$ upper-case letters for a random variables. Lower-case letters $x,y,z$ are concrete values.

- All possible values of X is X's samples space denoted $S_{X}$
- If $S_{X}$is discrete we call $X$ a discrete random variable
- If $S_{X}$ is unaccountably infinite set AND $P(X=c)=0$ for all $c \in \mathbb{R}$ we call X a continuous variable.
- There are types that are neither continuous or discrete

#### Probability Mass Function
$f_{X}(x)=\mathbb{P}(X=x)$ for all $x \in S_{X}$
 $$
\begin{gather}
\sum_{s \in S_{X}}f_{X}(x)=1 \\
f_{X}(x)\geq 0
\end{gather}
$$
$\mathbb{E}(X)=\sum_{x\in S_{X}}xf_{x(x)}$

#### Cumulative Distribution Function
Cumulative Distribution Function: $F_{X}(x)=\mathbb{P}(X\leq x)$
- Loosely Speaking CDF takes real value and outputs its percentile rank 
$$
\begin{gather}
\mathbb{P}(a<X\leq b)=F_{X}(b)-F_{X}(a) \\
\mathbb{P}(X<A)-\lim_{ x \to a -}F(x) \\
\mathbb{P}(X=a)=F_X(a)-\lim_{ x \to a- } F_{X}(x)
\end{gather}
$$
$\mathbb{P}(X=a)$ pmf at a
When X is discrete $F_{X}(x)=\sum_{s\leq x}f_{X}(s)$

##### Probability Density Functions
f(x) is a probability density function of X if
$\mathbb{P}(X\leq a)=\int_{-\infty}^af(x)dx$
If X's CDF is $F_{X}(x)$ then
$F_{X}(a)=\int_{-\infty}^af(x)dx$

$$
\begin{gather}
f_{X}(x)\geq 0 \\
\int_{-\infty}^\infty f_X(x)dx=1 \\
\mathbb{P}(a<X\leq b)=\int_{a}^b f_{X}(x)dx
\end{gather}
$$
#### Indicator Function
Indicator on se