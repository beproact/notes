#### 1
##### a
GCD: $2^2\cdot3^2\cdot5\cdot7$
LCM: $2^2\cdot3^3 \cdot5  \cdot 7^2$
##### b
GCD: $5\cdot 11$
LCM: $2^2\cdot 3 \cdot 5^2\cdot 7^3\cdot 11^2 \cdot 13\cdot 17$
##### c
GCD: 1
LCM: $2^2\cdot 3^2\cdot 5^7\cdot 11^{13}\cdot 13^{11}$
##### d
GCD: 19
LCM: $3\cdot 5 \cdot 7^2 \cdot 11\cdot 17 \cdot 19^2 \cdot 23  \cdot29$
#### 2
##### a
The statement is false.
Proof
We will provide a counterexample.
Counterexample: $a=8$,$b=4$.
$a^2=64$ and $b^3=64$
$64 \mid 64$ but $8\nmid 4$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof.
Using the fundamental theorem of arithmetic, both a and b have unique prime factorizations. Then we can write $a=p_{1}^{c_{1}}\cdot\dots\cdot p_{m}^{c_{m}}$ and $b=p_{1}^{d_{1}}\cdot\dots\cdot p_{m}^{d_{m}}$, where $p_{1}\dots p_{m}$ are prime. For any prime that $a$ and $b$ do not share, we can set the exponent to $0$. Then we know $a^2= p_{1}^{2c_{1}}\cdot\dots\cdot p_{m}^{2c_{m}}$ and $b^2=p_{1}^{2d_{1}}\cdot\dots\cdot p_{m}^{2d_{m}}$. Since $a^2|b^2$ then $p_{1}^{2c_{1}}\cdot\dots\cdot p_{m}^{2c_{m}} \mid p_{1}^{2d_{1}}\cdot\dots\cdot p_{m}^{2d_{m}}$ this means that $k(p_{1}^{2c_{1}}\cdot\dots\cdot p_{m}^{2c_{m}})= p_{1}^{2d_{1}}\cdot\dots\cdot p_{m}^{2d_{m}}$. We can divide by each prime factor to get $k=p_{1}^{2d_{1}-2c_{1}}\cdot\dots\cdot p_{m}^{2d_{m}-2c_{m}}$. We know that for any $1\leq i\leq m$ that $d_{1}>c_{1}$ since $k$ is an integer and if any exponents were less than $0$ that would be dividing a number by a prime not in its prime factorization.
We can then separate out the exponent to get $k=(p_{1}^{d_{1}-c_{1}}\cdot\dots\cdot p_{m}^{d_{m}-d_{m}})^2$. Lets say that $l=p_{1}^{d_{1}-c_{1}}\cdot\dots\cdot p_{m}^{d_{m}-d_{m}}$. We know $l$ is an integer because $d_{i}\geq c_{i}$, so all prime numbers are to a positive exponent. This gives us that 
$$
\begin{align}
l^2a^2&=b^2 \\
la&=b
\end{align}
$$
Since $b$ can be written as $a$ times an integer, then $a|b$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

##### c
Proof
Since $p^4|a^3$ and $p|p^4$ we know by Proposition 1.1 that $p|a$. Since $p|a$ that means $p$ is in the prime factorization of $a$ with some exponent $c\geq1$. We can then write $a$ as the $p$ prime factor multiplied by the any other numbers in the prime factorization $a=p^cm$. Since $m$ is made up entirely prime numbers other than $p$ we know that $p\nmid m$ and $p$ is not in the prime factorization of $m$. We can then cube both sides to get $a^3=p^{3c}m^3$. Since $p^4|a^3$ then we know that $p^4|p^{3c}m^3$. However, we know that $p$ is not in the prime factorization of $m$ so $p^4\nmid m^3$. This means $p^4|p^{3c}$. This is only possible if $c\geq2$. Therefore $a=p^2m$, so $p^2|a$.

#### 3
Proof



We can express the harmonic numbers as a fraction.
When adding multiple fractions together, we can make the denominator the LCM of the numbers. This is because, when adding fractions you want to find a common multiple to make the denominator. When the fraction is the most, that multiple is the LCM. 
Lets call the LCM, $M$. We can call the numerator $N$.

Assume to the contrary there is some $n\in \mathbb{Z}$ where $H_{n}\in\mathbb{Z}$. Then, $H_{n}=1+\frac{1}{2}+\dots+\frac{1}{n}$ let $2^c$ be the largest power of $2$ less than or equal to $n$. Since $M$ is the LCM of $1,\dots ,n$ then $2^c|M$. We know that $2^{c+1} \nmid M$ because then the LCM would have a greater number of $2$s than the max within the prime factorizations in $1,\dots,n$ which violates Proposition 1.17. We can call $M_{1}$ the LCM of $1,\dots,n$ excluding $2^c$. This creates a number where all of $1,\dots,n$ divides $M_{1}$ except for $2^c$. We can the multiply to get that$M_{1}H_{n}=M_{1}+\frac{M_{1}}{2}+\dots+\frac{M_{1}}{2^c}+\dots+\frac{M_{1}}{n}$. Since everything except $2^c$ is divides $M_{1}$ we know that $M_{1}H_{n}$ is the sum of a bunch of integers, and $\frac{M_{1}}{2^c}$ which is not an integer. This means $M_{1}H_{n}$ is not an integer. This means $H_{n}$ is not an integer. Contradiction.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

#### 4
##### a
Proof
Since $a$ and $b$ are expressible in the form $6n+1$ let $a=6c+1$ and $b=6k+1$. Then
$$
\begin{align}
ab&=(6c+1)(6k+1) \\
&=36ck+6c+6k+1 \\
&=6(6ck+c+k)+1
\end{align}
$$
We know that $ab$ can be expressed as $6n+1$ where $n=(6ck+c+k)$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
Assume to the contrary that there are finitely many prime number of the form $6n+5$. Lets call these $p_{0},p_{1},\dots,p_{r}$, with $p_{0}=5$. Consider $N=6p_{1}\dots p_{r}+5$.  The prime factorization of N must contain a prime number $p$ of the form $6n+5$, since otherwise it would only have prime factors of the form $6n+1$ which by 4a make of the form $6n+1$. Other forms are not possible as they are all composite. So $p$ must be either $p_{0}=5$ or one of $p_{1},\dots,p_{r}$.

Case: $p=5$
Then we know $5|N$. By proposition 1.2 we know that $5|N-5$ so $5|6p_{1}\dots p_{r}$. By Corollary 1.15 we know either $5|6$ or $5|p_{i}$ for $i=1,2,\dots,r$. Contradiction

Case: $p=p_{i}$ for some $i=1,2,\dots,r$
Then $p_{i}|N$ implies that $p_{i}|N-4p_{1}p_{2}\cdot\dots\cdot p_{r}$ by Proposition 1.2. This gives that $p_{i}|3$. Contradiction.

Since both cases result in a contradiction there are infinitely many prime numbers of the for $6n=5$.
#### 5
##### a
Proof
Since $a\equiv b \pmod{m}$ and $c\equiv d \pmod{m}$ then there exists $e,f\in \mathbb{Z}$ where $a-b=em$ and $c-d=fm$.
This gives us that 
$$
\begin{align}
a-b-(c-d)&=em-fm \\
(a-c)-(b-d)&=(e-f)m
\end{align}
$$
This shows that $(a-c)\equiv(b-d) \pmod{m}$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
This statement is false.
Proof
Counterexample:
$a=5,b=10,c=5,d=5,m=5$.
$a|c$ since $5|5$.
$d|b$ since $5|10$.
$a\equiv b \pmod m$ since $5\equiv10 \pmod5$ 
$c\equiv d \pmod m$ since $5\equiv5 \pmod5$
However, $\frac{a}{c}\not\equiv \frac{b}{d} \pmod5$ since $1\not\equiv 2 \pmod5$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

#### 6
##### a
Proof
Since $a$ is even we know that $2|a$ and $c\in \mathbb{Z}$ exists where $2c=a$. Then, we can square both sides to get $4c^2=a^2$. Since $a^2$ can be written as a number times $4$ then $4|a^2$. Since $4|a^2$ this means that $a^2\equiv0 \pmod4$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
Since $a$ is odd, then we can write $a$ as $a=2c+1$, where $c\in \mathbb{Z}$. We can square this on both sides to get $a^2=4c^2+4c+1$. This can be rewritten as $4c(c+1)+1$. We now have two cases, $c$ is even and $c$ is odd.

$c$ is even:
Since $c$ is even, there exists $k$ where $c=2k$. We can plug this in to get $a^2=4(2k)(2k+1)+1=8k(2k+1)+1$. We can get from this $a^2-1=8(k(2k+1))$. This shows that $a^2\equiv1 \pmod8$.

$c$ is odd:
Since $c$ is even, there exists $k$ where $c=2k+1$. We can plug this in to get $a^2=4(2k+1)(2k+1+1)+1=4(k+1)(2k+2)+1=8(2k+1)(k+1)+1$. We can get from this $a^2-1=8((2k+1)(k+1))$. This shows that $a^2\equiv1 \pmod8$.

As we have proven both cases we know that $a^2\equiv1 \pmod8$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

$a^2\equiv1 \pmod4$
Proof
Since $a^2\equiv1 \pmod8$ we know that $8|a^2-1$ this means that there exists $c$ where $8c=a^2-1$. This is equivalent to $4(2c)=a^2-1$. This shows that $4|a^2-1$. Therefore, $a^2\equiv1 \pmod4$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### c
Proof
We know from 6a and 6b that if $a$ is even then $a^2\equiv0 \pmod4$ and that if $a$ is odd then $a^2\equiv1 \pmod4$. We want to show that if $a,b\in \mathbb{Z}$ then $a^2+b^2 \not\equiv3 \pmod4$.
We have $3$ cases. Both are even, both are odd and each have different parity.

Both are even:
Since both are even, $a^2\equiv0 \pmod4$ and $b^2\equiv0 \pmod4$. By Proposition 2.4 we know that $a^2+b^2\equiv0 \pmod4$.

Both are odd:
Since both are odd, $a^2\equiv1 \pmod4$ and $b^2\equiv_{1} \pmod4$. By Proposition 2.4 we know that $a^2+b^2\equiv2 \pmod4$.

They have different parity:
Without loss of generality say that $a$ is even and $b$ is odd. 
Since $a$ is even, $a^2\equiv0 \pmod4$ and since $b$ is odd, $b^2\equiv_{1} \pmod4$. By Proposition 2.4 we know that $a^2+b^2\equiv1 \pmod4$.

Since for none of the cases is $a^2+b^2 \equiv3 \pmod4$ true. We know that it is never true. This means if $n \equiv3 \pmod4$, then $n$ is not the sum of two squares of integers.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### d
The converse is not true.
Proof
Counterexample. $n=3$
The number $3$ cannot be written as the sum of two squares, but $3\equiv3\pmod3$.

#### 7
##### a
$$
\begin{align}
35&=4(8)+3 \\
8&=2(3)+2 \\
3&=1(2)+1 \\
1&=1(1)+0 \\
 \\

1&=1(3-1(2)) \\
&=3-(8-2(3)) \\
&=3(3)-8 \\
&=3(35-4(8))-8 \\
&=3(35)-13(8)
\end{align}
$$

$$
\begin{align}
-13(8)=1\pmod {35} \\
-13=22\pmod {35}
\end{align}
$$
22 is the inverse
##### b
$$
\begin{align}
99&=1(51)+48 \\
51&=1(48)+3 \\
48&=16(3)+0
\end{align}
$$
$(99,51)=3$ so there is no inverse modulo since it requires the GCD to be 1.

##### c
$$
\begin{align}
1517&=1(1333)+184 \\
1333&=7(184)+45 \\
184&=4(45)+4 \\
45&=11(4)+1 \\
 \\
1&=45-11(4) \\
1&=45-11(184-4(45)) \\
1&=45(45)-11(184) \\
1&=45(1333-7(184))-11(184) \\
1&=45(1333)-326(184) \\
1&=45(1333)-326(1517-1333) \\
1&=371(1333)-326(1517)
\end{align}
$$
This gives us that $371(1333)\equiv1 \pmod{1517}$ so $371$ is the inverse modulo of $1333$.

#### 8
##### a
$$
\begin{align}
x-3&=4c \\
x&=4c+3  \\
4c+3&\equiv2 \pmod5 \\
4c&\equiv4 \pmod5 \\
4\bar{4}c&\equiv4 \bar{4} \pmod5 \\
c&\equiv1 \pmod5 \\
 \\
x-3&\equiv4 \pmod{20} \\
x&=7
\end{align}
$$
##### b
$$
\begin{align}
M&=210 \\
M_{1}&=105 \\
M_{2}&=70 \\
M_{3}&=42 \\
M4&=30 \\
\\
105\bar{M}_{1}&\equiv 1 \pmod2 \\
\bar{M}_{1}&\equiv 1 \pmod2 \\ \\

70 \bar{M_{2}}&\equiv 1 \pmod3 \\
\bar{M_{2}}&\equiv 1 \pmod3  \\

 \\
42 \bar{M_{3}}&\equiv 1 \pmod5 \\
\bar{M_{3}}&\equiv 3 \pmod 5 \\
 \\
  
30 \bar{M_{3}}&\equiv 1 \pmod 7 \\
2\bar{M_{3}}&\equiv 1 \pmod 7 \\ 
\bar{M_{3}}&\equiv 4 \pmod 7 \\
  \\
x&\equiv1\cdot 105\cdot 1+2\cdot 70 \cdot 1+4\cdot 42\cdot 3 + 6\cdot30 \cdot4  \pmod {210} \\
&\equiv1469\pmod {210} \\
&\equiv 209 \pmod {210} \\
 \\
x=209
\end{align}
$$
##### c
$$
\begin{align}
3x&\equiv2\pmod {4} \\
3\cdot3x&\equiv3\cdot2\pmod {4} \\
x&\equiv2\pmod {4} \\
 \\
4x&\equiv1  \pmod {5} \\
4\cdot4x&\equiv4\cdot1  \pmod {5} \\
x&\equiv4  \pmod {5} \\
 \\
6x&\equiv 3  \pmod {9} \\ 
2x&\equiv 1  \pmod {3} \\
x&\equiv 2  \pmod {3} \\
\end{align}
$$
$$
\begin{align}
x \equiv 2 \pmod4 \\
x \equiv 4 \pmod5 \\
x \equiv 2 \pmod 3
\end{align}
$$
$$
x=14
$$

#### 9
$$
\begin{align}
n \equiv -1 \pmod2 \\
n \equiv -1 \pmod 3 \\
n \equiv -1 \pmod 4 \\
n \equiv -1 \pmod 5 \\
n \equiv -1 \pmod 6 \\ 
\end{align}
$$
This means that $n+1$ is equivalent to $0$ for modulus $2,\dots,6$. Therefore, $n+1$ is a multiple of $2,...6$. 
$$
[2,3,4,5,6]=60
$$
Therefore we know that 
$$
\begin{align}
n+1&\equiv 0\pmod{60} \\
n+1&= 60c \\
n&=60c-1
\end{align}

$$
and that 
$$
\begin{align}
60c-1& \equiv 0 \pmod 7 \\
4c &\equiv 1 \pmod 7 \\
2\cdot 4c &\equiv2 \pmod 7 \\
c &\equiv 2 \pmod 7 \\
 \\
n&=60\cdot 2-1=119
\end{align}
$$
#### 10
Proof
First we prove $(m_{i},m_{j})|b_{i}-b_{j}$  if the system of linear congruences is solvable. 
If the system has a solution then for each $i$, $x\equiv b_{i} \pmod {m_{i}}$ and for each $j$, $x\equiv b_{j} \pmod {m_{j}}$. This gets us that $x=cm_{i}+b_{i}$ and $x=cm_{j}+b_{j}$. Setting these equal we get that 
$$
\begin{align}
cm_{j}+b_{j}&=cm_{i}+b_{i} \\
cm_{j}-cm_{i}&=b_{i}-b_{j}
\end{align}
$$
Since $(m_{i},m_{j})|m_{j}$ and $(m_{i},m_{j})|m_{i}$ we know by Proposition 1.2 that $(m_{i},m_{j})|b_{i}-b_{j}$.

Next we prove that if the system of linear congruences is solvable then $(m_{i},m_{j})|b_{i}-b_{j}$.

We can use $(m_{i},m_{j})|b_{i}-b_{j}$ to get that $c(m_{i},m_{j})=b_{j}-b_{i}$. $(m_{i},m_{j})$ can be written as an integer linear combination of $m_{i}$ and $m_{j}$. This gives us that $c_{1}m_{i}-c_{2}m_{j}=b_{j}-b_{i}$. We can rewrite this as $x=c_{1}m_{i}+b_{i}=c_{2}m_{j}+b_{j}$. This shows for any two $i,j, i\neq j$ that there is a solution where both $x\equiv b_{i }\pmod{m_{i}}$ and $x\equiv b_{j }\pmod{m_{j}}$. Since this is true for any two, then if the relationship can be used to show that this is true for all $1,\dots ,n$.

Uniqueness
Suppose there are two solutions $x,y$.
Then for each $i$ , $x\equiv b_{i }\pmod{m_{i}}$ and $y\equiv b_{i }\pmod{m_{i}}$. This tells us that $x\equiv y\pmod{m_{i}}$ or $m_{i}|x-y$.Since all of $m_{1},\dots m_{n}$ divides $x-y$ then $[m_{1},\dots,m_{n}]$ divides $x-y$. This tells us that $x\equiv y \pmod{[m_{1},\dots m_{n}]}$. Therefore the solution is unique modulo $[m_{1},\dots,m_{n}]$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 11
##### a
Proof
By Wilson's Theorem we know that 
$$
\begin{align}
(p-1)! \equiv -1 \pmod p \\
(p-1)(p-2)(p-3)! \equiv -1 \pmod p \\
(-1)(-2)(p-3)! \equiv -1 \pmod p \\
2(p-3)! \equiv -1 \pmod p
\end{align}
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
By 11a we know that $2(p-3)! \equiv -1 \pmod p$. $103$ is prime so this formula applies. $2(103-3)! \equiv -1 \pmod{103}$. The least non-negative residue is $102$.
#### 12
Proof
Let $n=\frac{p-1}{2}$. 
We can plug $n$ into the equation to get $1^2 3^2 5^2 \cdots (p-4)^2 (p-2)^2=1^2 3^2 5^2 \cdots (2n-3)^2 (2n-1)^2$. This is equivalent to 
$$
\begin{align}
\left( \frac{(2n)!}{2^nn!} \right)^2=\left( \frac{(p-1)!}{2^nn!} \right)^2
\end{align}
$$
We can use Wilson's Theorem to show that
$$
\left( \frac{(p-1)!}{2^nn!} \right)^2 \equiv\left( \frac{-1}{2^nn!} \right)^2 \equiv  \frac{1}{2^{2n}n!^2}\equiv \frac{1}{2^{p-1}n!^2} \pmod p
$$
Using Fermat's Little Theorem we then get that 
$$
\frac{1}{2^{p-1}n!^2}\equiv \frac{1}{n!^2} \pmod p
$$
We now want to find what $n!^2$ is. We know that $(p-1)!= (1)(2)\dots(p-2)(p-1)$.
$$
\begin{align}
-1&\equiv (1)(2)\dots(p-2)(p-1) \pmod p \\
-1&\equiv (1)(2)\dots(-2)(-1) \pmod p \\
-1&\equiv (-1)^nn!^2 \pmod p \\
-1^{n+1} &\equiv n!^2 \pmod p
\end{align}
$$

We can substitute this to get 
$$
\begin{align}
 \frac{1}{n!^2} \equiv (-1)^{n+1} \equiv (-1)^{(p+1)/2} \pmod p
\end{align}
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$