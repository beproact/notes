Choose a picot place it correctly
ensures things less than it are placed before
ensure thing greater than it are place after it
recursively sort above and below
```python
Quicksort(A,l,u):
	p_i=partition(A,l,u)
	Quicksort(A,l,p-1)
	Quicksort(A,p+1,u)
	return A
Quicksort(A,l,n) for A[1...n]
```

```python
partition(A,l,u):
	p=A[u] # instead choose random
	i=l-1
	for j in l...u-1
		if A[j] <=p
			i++
			swap A[i] and A[j]
	swap A[i+1],A[u]
	return i+1
```
Worst Case $O(n^2)$


Best Case
$T(n)=2T\left( \frac{n}{2} \right)+O(n)$

Biased Case
$T(n)=T\left( \frac{999}{1000}n \right)+T\left( \frac{1}{1000}n \right) + O(n)$
$\frac{n}{\left( \frac{1000}{999} \right)^i}=O(1)$
$i=\log_{\frac{1000}{999}}(n)$
$i=O(\log n)$
$O(n\log n)$


$A[1\dots n]$
$T(n)=T(i)+T(n-1)+n$
$$
\begin{gather}
T(n)=\frac{1}{n}\left[ \sum_{i=0}^{n-1}[T(i)+T(n-i)] \right]+n \\
T(n)=\frac{1}{n}\left[ 2\sum_{i=0}^{n-1}[T(i)] \right]+n \\
nT(n)=2\left[ \sum_{i=0}^{n-1}[T(i)] \right]+n^2
\end{gather}
$$
evaluate n->n-1
$$
\begin{gather}
(n-1)T(n-1)=2\left[ \sum_{i=0}^{n-2}[T(i)] \right]+(n-1)^2 \\
nT(N)-(n-1)T(n-1)=2T(n-1)+2n +1 \\
\frac{T(n)}{n+1}=\frac{T(n-1)}{n}+\frac{2}{n+1} \\
\frac{T(n)}{n+1}=\frac{T(1)}{2}+2\sum_{i=3}^{n+1}{\frac{1}{i}}
\end{gather}
$$
Harmonic numbers are $O(\log n)$
$$
\begin{gather}
\frac{T(n)}{n+1}=\frac{T(1)}{2}+O(\log n) \\
\frac{T(n)}{n}=O(\log n) \\
T(n)=O(n\log n)
\end{gather}
$$
$\braket{ \psi |  }$