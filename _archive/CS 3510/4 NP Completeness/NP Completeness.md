
If problem A reduces to problem B, then a solution to B can be used to solve  A.
$A\leq_{p}B$


"If some of the problems is found if and only if we solve an NP complete problem we know the problem is NP hard. "

I can solve this puzzle ok solve this np complete problem that is the same thing

Is everything easy to verify easy to compute.

When you don't know how to code
- algorithm has a runtime
- problem has a complexity

Any specific problem can have multiple solutions. 

A can look at fast upper bound and smallest lower bound. 
$\Theta(n)$

Upper bounds are generally easy.
Lower bounds are harder.

NP Completeness is a hack around this.
If $P\neq NP$ then $NP$ complete problems are "hard" $2^{\Omega(n)}$

1. Give Up
2. Approximate
3. SMT solvers
4. Reasonable

#### P
Decision Problem
RELPRIME = ${\braket{  a,b }}$ a is relatively prime to $b$
$P$ = class of problems decidable in polynomial time
RELPRIME $\in P$

PATH = $\braket{ G,s,t } \exists$ a path in G $S\to t$
PATH $\in P$

 1. Efficient/ You have a nontrivial mathematical understanding of the problem
 2. Closure $f,g$ are polynomials then $f\cdot g,f+g$ are polynomial
 3. Usually you can make them more efficient
 4. Every machine architecture has the same P

#### NP
Nondeterministic Polynomial Time
$A\in NP$
$x\in E \iff \exists w V(x,w)$ returns true

COMPOSITES = {$\braket{  n  }$ | n is composite}
```python
def V(<n>,<c>): #c can'ts be 1 or n
	return n(mod c) == 0
```

$P\subseteq NP$

#### EXP
Problems solvable in $2^{n^k}$

### Reduction
Input: n unsorted elements
Output: indices of the elements if they were sorted
Can we solve in less than $O(n\log n)$. No we can't

Assume to the contrary we can solve this in less time. If we could then we could solve sorting in O(nlogn) violating the $\Omega(n\log n)$
