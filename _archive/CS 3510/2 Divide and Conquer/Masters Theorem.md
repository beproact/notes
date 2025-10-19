$T(n) = aT\left( \frac{n}{b} \right) + O(n^d)$
 a: # subproblems
 b: size of subproblem / maybe more accurate to say how much problem is split
 $n^d$ : time to recombine

$$
T(n)=\begin{cases}
O(n^d) & d>\log_{b}a \\
O(n^d)\log n & d=\log_{b}a \\
O(n^{\log_{b}a}) & d<\log_{b}a
\end{cases}
$$

# Proof

We can form a tree with all the subproblems divided out. 
Let k be the depth. Let K be greatest depth

To find K:
We stop splitting when each subproblem is $O(1)$ 
This is the case when 
$$
\begin{gather}
\frac{n}{b^k}=O(1) \\
n=b^K \\
K=\log_{b}n
\end{gather}
$$
So the maximum depth $K=\log_{b}n$

Each layer of this tree has $a^k$

- First layer has $a\cdot O\left(\left( \frac{n}{b} \right)^d\right)$
- Second layer has $a^2\cdot O\left(\left( \frac{n}{b^2} \right)^d\right)$
- Third layer has $a^3\cdot O\left(\left( \frac{n}{b^3} \right)^d\right)$
- ...
- Kth layer has $a^K\cdot O\left(\left( \frac{n}{b^K} \right)^d\right)$

Then we add work done too each leaf.
The maximum number of leaves is $a^K = a^{\log_{b}n}=n^{\log_{b}a}$

$T(n)=\sum_{i=0}^{\log_{b}n}a^i\cdot O\left( \left( \frac{n}{b^i} \right)^d \right) + O(n^{\log_{b}a})$
Work done at each layer added to work done at each leaf.
Since we only care about the large term with big O we our answer depends on which term is the greatest. 

## Applying to Algorithms

### Mergesort
[[Mergesort]]
$\begin{gather}a =2 \\b=2 \\d=1\end{gather}$
$T(n) = O(nlogn)$

$$
\begin{gather}
\log_{b}a=\log_{2}2 = 1 = d \\
\log _{b}a=d\\
O(n^d\log n)= n\log n
\end{gather}
$$
Number of splits does not decrease time complexity
### Binary Search
$\begin{gather}a =1 \\b=2 \\d=0\end{gather}$
$O(n^0\log n) = O(\log n)$