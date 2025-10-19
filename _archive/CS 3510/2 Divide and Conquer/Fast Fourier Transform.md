Theres going to be some handwavy math
Fixed point arithmetic. 

$A(x)=a_{0}+a_{1}x+a_{2}x^2+ \dots +a_{n-1}x^{n-1}$
Operations on polynomials.
- add them
- multiply
- evaluate
coeff form

##### Addition
$A = [a_{1},a_2,\cdots,a_{n-1}]$
$B = [b_{1},b_2,\cdots,b_{n-1}]$
A+B = just add the terms i'm not writing them out
O(n) if addition is constant time

##### Multiplication
Naive is $O(n^2)$

##### Evaluation
Naive is $O(n^2)$
$a_{0}+a_{1}x +a_{2}x^2\dots$
$a_{0}+x(a_{1}+x(a_{2\dots}))$

### Sample Form
a nth degree polynomial can be uniquely expressed with n+1 points.
$A=[A(x_{0}),A(x_{1}),A(x_{2})\dots]$
$B=[B(x_{0}),B(x_{1}),B(x_{2})\dots]$
$A+B=$ Add the samples
$A\cdot B=$ Multiply the samples
O(n)

Evaluateing takes $O(n^2)$

FFT lets you go from coeffs to sample in and reverse in $O(nlogn)$
This means you can convert to sample form and multiply then convert back to coeffs.

on paper

```python
def FFT(A, w):
	if w = 1 output A(1)
	find Ae, Ao such that A(x)=Ae(x^2)+x*Ao(x^2)
	:=FFT(Ae(x^2), w^2)
	FFT(Ao(x^2), w^2)
```
$O(n\log n)$


1. Compute samples of a using FFT
2. Compute samples of b using FFT 
3. Multiply
4. convert back to coeffs (cause FFT is invertable somehow)

TAing 
grading
responding to questions
1-2 hours office hours maybe

4 ta lab lectures
threads lecture
out of class workshops
- resume review

Don't apologize for talking.
Have a preparation for what who I am.