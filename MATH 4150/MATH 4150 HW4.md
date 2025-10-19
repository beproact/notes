#### 1
##### a
###### First Part
Proof
We prove by induction.
Base Case:
$a=1$
Then
$$
\sum_{m=1}^1m=1=\frac{1(1+1)}{2}
$$
Induction Step:
Assume for some $i >1$ that
$$
\sum_{m=1}^im=\frac{i(i+1)}{2}
$$
We will show that this is true for $i+1$ as well.
$$
\begin{align}
\sum_{m=1}^{i+1}m=\sum_{m=1}^{i}m+i+1
\end{align}
$$
By our induction hypothesis we can rewrite this as
$$
\begin{align}
\sum_{m=1}^{i+1}m&=\frac{i(i+1)}{2}+i+1 \\
&=\frac{i(i+1)+2i+2}{2} \\
&=\frac{i^2+i+2i+2}{2} \\
&=\frac{i^2+3i+2}{2} \\
&=\frac{(i+1)(i+2)}{2} \\
&=\frac{(i+1)((i+1)+1)}{2}
\end{align}
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
###### Second Part
Proof
We prove by induction
Base Case:
$a=1$
$$
\sum_{m=1}^1m^3=1=\left( \frac{1(1+1)}{2} \right)^3
$$
Induction Step:
Assume for some $i >1$ that
$$
\sum_{m=1}^im^3=\left( \frac{i(i+1)}{2} \right)^2
$$
We will show that this is true for $i+1$ as well.
$$
\begin{align}
\sum_{m=1}^{i+1}m^3=\sum_{m=1}^{i}m^3+(i+1)^3
\end{align}
$$
By our induction hypothesis we can rewrite this as
$$
\begin{align}
\sum_{m=1}^{i+1}m^3&=\left( \frac{i(i+1)}{2} \right)^2+(i+1)^3 \\
&=\frac{i^2(i+1)^2}{4}+(i+1)^3 \\
&=\frac{i^2(i+1)^2+4(i+1)^3}{4} \\
&=\frac{i^4+2i^3+i^2+4i^3+12i^2+12i+4}{4} \\
&=\frac{i^4+6i^3+13i^2+12i+4}{4} \\
&=\frac{(i+1)^2(i+2)^2}{4} \\
&=\left( \frac{(i+1)((i+1)+1)}{2} \right)^2
\end{align}
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
We know $v(d)$ is multiplicative. Since $v(d)$ is multiplicative then $\sum_{d|n}v(d)$ is multiplicative and so is $\left( \sum_{d|n}v(d) \right)^2$. In addition, $v(d)^3$ must also be multiplicative and so must $\sum_{d|n}(v(d))^3$. This means both arithmetic functions are defined by their behavior on prime powers, so we only need to prove this for prime powers.
Let $a,p \in \mathbb{Z}$ with $p$ being prime. $p^a$ has $1,p,2p,\dots,p$ factors so $v(p^a) =a+1$. Since $p^a$ is a prime power, every single factors of $p$ is also a power $p$. This means that
$$
\begin{align}
\sum_{d|n}v(p^a)=\sum_{i=0}^a(i+1)
\end{align}
$$
This tells us that 
$$
\left( \sum_{d|n}v(p^a) \right)^2=\left( \sum_{i=1}^{a}i+1 \right)^2
$$
We also know that 
$$
\sum_{d|n}(v(p^a))^3=\sum_{i=0}^a(i+1)^3
$$
By part a we know that 
$$
\left( \sum_{i=1}^{a}i+1 \right)^2=\left( \frac{a(a+1)}{2} \right)^2=\sum_{i=0}^a(i+1)^3
$$
So both sides are equal for prime powers. Since both functions are multiplicative this means they are equal for all numbers.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 2
Proof

We know that $\sigma(n!)$ is the sum of divisors of $n!$. Another way of saying this is adding up every subset of prime factors of $n!$ multiplied. This means that 
$$
\begin{align}
\sigma(n!) &= n!+\frac{n!}{n}+\frac{n!}{n-1}\dots+2+1 \\
\frac{\sigma(n!)}{n!}&=1+\frac{1}{n}+\frac{1}{n-1}+\dots+\frac{2}{n!}+\frac{1}{n!} \\
&=\sum _{d|n!}\frac{1}{d}
\end{align}
$$
We know that $1,2,\dots,n$ are all factors of $n!$ so
$$
\begin{align}
\frac{\sigma(n!)}{n!}&=\sum_{i=1}^n\frac{1}{i}+\sum _{d|n!,i>n}\frac{1}{d} \geq\sum_{i=1}^n\frac{1}{i}
\end{align}
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 3
##### a
Proof
$120=2^3\cdot3\cdot5$
Since $\sigma$ is multiplicative $\sigma(120)=\sigma(2^3)\sigma(3)\sigma(5)=15\cdot 4\cdot6=360=3\cdot 120$. Since $\sigma(120)=3\cdot120$ then $120$ is $3$-prime.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
$2^k,3,p$ are all coprime. Since $\sigma$ is multiplicative that means $\sigma(2^k3p)=\sigma(2^k)\sigma(3)\sigma(p)$.
In addition, by theorem 3.10 we can get that $\sigma(2^k)\sigma(3)\sigma(p)=(2^{k+1}-1)(4)(p+1)$. 
$$
\begin{align}
(2^{k+1}-1)(4)(p+1)&=2^k3^2p \\
(2^{k+3}-4)(p+1)&=2^k9p \\
\frac{p+1}{p}&=\frac{2^k9}{2^{k+3}-4} \\
1+\frac{1}{p}&=\frac{2^k9}{2^{k+3}-4} \\
\frac{1}{p}&=\frac{2^k9-2^{k+3}+4}{2^{k+3}-4} \\
\frac{1}{p}&=\frac{9(2^k)-8(2^{k})+4}{2^{k+3}-4} \\
\frac{1}{p}&=\frac{2^k+4}{8(2^k)-4} \\
p&=\frac{8(2^k)-4}{2^k+4} \\
p&=8-\frac{36}{2^k+4}
\end{align}
$$
$p$ must be an odd prime so $2^k+4$ must divide $36$.
$k=1$
$p=8-\frac{36}{2+4}=8-6=2$
Not valid, $p$ must be an odd prime.
$k=2$
$p=8-\frac{36}{4+4}$
Not valid $p$ must be an integer.
$k=3$
$p=8-\frac{36}{8+4}=5$
Valid
$k=4$
$p=8-\frac{36}{16+4}$
Not valid, $p$ must be an integer.
$k=5$
$p=8-\frac{36}{32+4}=7$
Valid
Anything larger results in $2^k+4$ being larger than $36$ meaning $p$ would not be an integer.
Our answers are $2^3\cdot3\cdot 5$ and $2^5\cdot 3\cdot7$.
##### c
Proof
If $n$ is $p$-perfect then $\sigma(n)=p(n)$. Since $p \nmid n$ then $n$ and $p$ are coprime. Since $\sigma$ is multiplicative that means $\sigma(np)=\sigma(n)\sigma(p)=pn(p+1)$. Since $\sigma (np)=np(p+1)$ then $np$ is $p+1$-prime.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 4
Proof
We can show that for $n$ with prime factorization $p_{1}^{a_{1}}\dots p_{n}^{a_{n}}$
$$
\begin{align}
\sum_{d|n}\Lambda (d)&=a_{1}\ln(p_{1})+\dots+a_{n}\ln(p_{n}) \\
&=\ln(p_{1}^{a_{1}}\dots p_{n}^{a_{n}}) \\
&=\ln(n)
\end{align}
$$
By Mobius Inversion we know know from this that $\Lambda(n)=\sum_{d|n}\mu(d)\ln\left( \frac{n}{d} \right)$. 
$$
\begin{align}
\Lambda(n)&=\sum_{d|n}\mu(d)(\ln(n)-\ln d) \\
\Lambda(n)&=\ln(n)\sum_{d|n}\mu(d)-\sum_{d|n}\mu (d)\ln(d)
\end{align}
$$
We know by proposition 3.14 that 
$$
\sum_{d|n}\mu(d)= \begin{cases}
1 &n=1 \\
0 &n>1
\end{cases}
$$
Therefore, for $n>1$ we know that $\Lambda(n)=-\sum_{d|n}\mu (d)\ln(d)$. To show the case of $n=1$, we can just plug into the equation. $\Lambda(1)=\ln(1)=0=-\sum_{d|n}\mu(1)\ln(1)$. This shows for all $n>0$ that $\Lambda(n)=-\sum_{d|n}\mu (d)\ln(d)$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 5
##### a
Proof
We want to show 
$$
\sum _{d|n}f(d)g\left( \frac{n}{d} \right)=\sum _{d|n}g(d)f\left( \frac{n}{d} \right)
$$
This is true because if $d|n$ then $\frac{n}{d}|n$. Both sides of the equation effectively loop through the same set of numbers in a different order.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof 
$$
\begin{gather}
f\star g=\sum _{d|n}f(d)g\left( \frac{n}{d} \right)=\sum _{d|n}f\left( \frac{n}{d} \right)g\left( d \right) \\
g\star h=\sum _{d|n}g(d)h\left( \frac{n}{d} \right)
\end{gather}
$$
$$
\begin{align}
(f\star g)\star h&= \sum_{d|n}\left( \sum _{d'|n}f\left( \frac{d'}{n} \right)g\left( d'\right) \right)h\left( \frac{n}{d} \right) \\
&= \sum_{d|n}\left(  \sum _{d'|n}f\left( \frac{d'}{n} \right)g\left( d'\right)  h\left( \frac{n}{d} \right) \right) \\
&=\sum_{d'|n}\left(  \sum _{d|n}f\left( \frac{d'}{n} \right)g\left( d\right)  h\left( \frac{n}{d} \right) \right) \\
&=\sum_{d'|n}\left(  f\left( \frac{d'}{n} \right)\sum _{d|n}\left( g\left( d\right)  h\left( \frac{n}{d} \right) \right) \right) \\
&=f\star(g\star h)
\end{align}
$$
Since $(f\star g)\star h=f\star(g\star h)$ convolution is associative.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### c
Proof
$f\star \delta=\sum _{d|n}f(d) \delta \left( \frac{n}{d} \right)$. We know that $\delta\left( \frac{n}{d} \right)$ is nonzero only when $\frac{n}{d}=1$ or when $d=n$. This tells us that $f\star \delta=\sum _{d|n}f(d) \delta \left( \frac{n}{d} \right)=f(n)$. Since convolution is commutative as shown in part a we know that $f\star\delta =\delta \star f=f$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### d
Proof
$\mu\star 1=\sum _{d|n}\mu(d) 1 \left( \frac{n}{d} \right)=\sum _{d|n}\mu(d)$. By proposition 3.14 
$$
\sum_{d|n}\mu(d)= \begin{cases}
1 &n=1 \\
0 &n>1
\end{cases}
$$
which is the same as our definition of $\delta$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### e
Proof
We show that $f=g\star1$ if and only if $g=\mu \star f=f\star \mu$
First we prove $f=g\star1$ implies $g=\mu \star f=f\star \mu$. 
$$
\begin{align}
f&=g\star1 \\
f\star\mu&=g\star1\star\mu \\
f\star \mu&=g\star\delta \\
f\star \mu&=g
\end{align}
$$
Since convolution is commutative as shown in part a $g=\mu \star f=f\star \mu$.
Next we prove $g=\mu \star f=f\star \mu$ implies $f=g\star1$
$$

\begin{align}
g&= f \star \mu \\
g \star1=f\star \mu \star1 \\
g\star 1 = f\star\delta \\
g\star1 = f
\end{align}
$$
We have shown  $f=g\star1$ if and only if $g=\mu \star f=f\star \mu$. This is equivalent to Mobius Inversion.
This is because the convolution $f=g\star1$ is the same as $f(n)=\sum_{d|n}g(d)1\left( \frac{n}{d} \right)=\sum_{d|n}g\left( d \right)$ and $g=\mu \star f=f\star \mu$ is equivalent to $g(n)=\sum_{d|n}\mu(d)f\left( \frac{n}{d} \right)=\sum_{d|n}\mu\left( \frac{n}{d} \right)f\left( d \right)$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$