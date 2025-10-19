Median of medians
$A[1\dots n]$ find kth smallest elemtent
if k = n/2
sort then return $A[k]$
$O(n\log n)$
```python
Quickselect(A,l,u,k):
	if l=u return A
	p_i=partition(A,l,u)
	if p_i>k
		Quickselect(A,l,p_i-1,k)
	if(p_i < k):
		Quickselect(A,p_i+1,u,k)
	if(p_i = k)
		return A[p_i]	
```
worst case
$T(n)=T(n-1)+O(n)$
$T(n)=O(n^2)$

"best case"
$T(n)=T\left( \frac{n}{2} \right)+O(n)$
$O(n)$

average case
$O(n)$

Median of Medians choose pivots better so that the new worst case improves to the average case.

Chop an array in blocks of size 5.
Sort each column
Recursively sort the columns by the medians
We can guarantee the median of medians is between 3/10th and 7/10th