$$
F_{0} = 0 , F_{1} = 1, n \geq f_{n}= F_{n-1} + F_{n-2}
$$
```python
def f1(n):
	if n=0,1 : return n
	else:
		return f1(n-1) +f1(n-2)
```

correctness

Time Function:
$$
T(n) = T(n-1)+T(n-2) + 20
$$
monotonic - always increasing so $T_(n-1) > T_{n-2}$ so
$$
T(n ) > 2T(n-2) +20
$$
We can save time by saving previous numbers.

```python
def f2(n):
	if n = 0 return n
	arr = [0] * (n+1) #allovate array of n+1 zeroes
	arr[0] = 0
	arr[1] = 1
	for i in range (2, n + 1):
		arr[i] = arr[i-2] + arr[i-1]
	return arr[n]
```
addition is not always constant time 
This means the function is $O(n^2)$
*Difference between the functions is whether or not the problem is solved*

We can use matrix multiplication

Also can use closed form. $F_{n} = \frac{1}{\sqrt{ 5 }} (\frac{{1+\sqrt{ 5 }}}{2})-\frac{1}{\sqrt{ 5 }} (\frac{{1-\sqrt{ 5 }}}{2})$


