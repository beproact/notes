Fixed point arithmetic
- Addition and multiplication take constant time

constant number of numbers
size of the number

Ways to represent numbers
- decimal
	- takes $\log_{10}x$ digits
- binary
	- takes $\log_{2}x$ digits
$\log_{2}x=\frac{{\log_{10}x}}{\log_{10}2}$
So all logs are multiples of each other so all logs have the same asymptotic size. They grow at the same rate.
n bits {0, ... $2^{n}-1$}

### Addition
O(n)
$\theta(n)$
### Multiplication
[[Multiplication]]

### Modular Exponentiation
$a^x\pmod n$
```python
def modexp (a, x, n):
	if x = 9 return 1
	z = modexp(a, floor(x/2), N)
	if x is even return z*z mod N
	if x is odd return a*z*z mod N
```
$O(n^3)$