Naive Algorithm is $O(n^2)$

```python
def mult(x,y):
	if y = 0 return 0
	z = mult(x,floor(y)
	if y is even return 2 * z
	if y is off return 2 * z + x 
```

###### Correctness proof
base case y = 0
Case 1 y is even $2z=2\left( \frac{x\cdot y}{2} \right) = xy$
Case 2 y is odd $2z + x = 2\left( x\cdot\frac{{y-1}}{2} \right) + x=xy$


## Another Algo
$x=2^{n/2}x_{L}+x_{R}$ Same for y
$y=2^{n/2}y_{L}+y_{R}$
We can then foil
Use [[Masters Theorem]]
a = 4
b = 2
d = 1
$O(n^2)$

### Karatsuba Method
middle 2 part of the foil
$x_{L}y_{R}+x_{R}y_{L}=(x_{L}+y_{R})(y_{l}+y_{r})-x_{L}y_{L}-x_{R}y_{R}$
a = 3
b = 2
d = 1
$O(n^{\log_{2}3})$

