Examples are 1 indexed as long as clear we can choose
```python
def mergesort(A[1 ... n/2]):
	if n = 1 return A
	L = mergesort(A[1, ... floor[n/2]])
	R = mergesort(A[floor[n/2] ... n])
	return merge(L,R)
```
$T(n) = 2T(n/2) + O(n)$


```python
def merge(x[1...k], y[1...m]):
	if x is length 0 return y
	if y is length 0 return x
	if x[1] <= y[1]:
		return x[1] ++ merge(x[2...k], y[1...m]) # I chose to use ++ prof used .join
	if y[1] <= x[1]:
		return y[1] ++ merge(y[2...k], x[1...m])
```
$T(n) = T(n-1) + O(1) = O(n)$

This is O(n) this can be found with the masters theorem.
[[Masters Theorem#Mergesort]]



