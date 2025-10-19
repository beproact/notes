#### 1
##### a
Proof

We need to show that $a|b$ implies $ac|bc$ and $ac|bc$ implies $a|b$.
First we show $a|b$ implies $ac|bc$. Since $a|b$ we know that there exists $d\in \mathbb{Z}$ where $ad=b$. We can multiply both sides by $c$ to get $adc=bc$. We can rewrite this to be $(ac)d=bc$. Since $bc$ can be written as $ac$ times a number $ac|bc$.
Next we show $ac|bc$ implies $a|b$. Since $ac|bc$ we know there exists $e\in \mathbb{Z}$ where $ace=bc$. We can divide by $c$ on both sides to get $ae=b$. Since $b$ can be written as $a$ time a number we know that $a|b$.
Since $a|b$ implies $ac|bc$ and $ac|bc$ implies $a|b$ we know $a|b$ if and only if $ac|bc$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Counterexample
$a=2,b=3,c=0$
$2\nmid3$ but $0|0$
#### 2
We need to show $m|n$ implies $a^m-1|a^n-1$ and $a^m-1|a^n-1$ implies $m|n$.
First we show $m|n$ implies $a^m-1|a^n-1$. Since $m|n$ there exists $c\in \mathbb{Z}$ where $cm=n$. Then $$a^n-1=a^{cm}-1=(a^m)^c-1=(a^m-1)((a^m)^{c-1}+(a^m)^{c-2}+\dots(a^m)+1)$$Since $a^n-1$ can be written as $a^m-1$ times a number, we know that $a^m-1|a^n-1$.
Next we show $a^m-1|a^n-1$ implies $m|n$. Using the division algorithm we can say that there exist $q,r\in \mathbb{Z}$ where $n=qm+r$ and $0\leq r<m$. Plugging that in we get $$a^n-1=a^{qm+r}-1=a^ra^{qm}-1$$
Since $m|qm$ we know from the first implication that $a^m-1|a^{qm}-1$. Using Proposition 1.2 we can see that $a^m-1|a^ra^{qm}-1-a^ra^{qm}+a^r$ which simplifies to $a^m-1|a^r-1$. However, $0\leq r<m$ and $a>1$. This means $a^m-1>a^r-1$. The only way this is possible is if $a^r-1=0$ so $r=0$. Since $r=0$ we can write $n=qm$. Since we can write $n$ as a multiple of $m$ and a number, $m|n$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 3
##### a
Proof
We proceed with induction on n.
If $n=0$ then $3|n^3-n$ is true since every number divides 0.
Assume $3|k^3-k$ for $k$. We will show that this is true for $k+1$. This means we need to show $3|(k+1)^3-(k+1)$. This means
$$
\begin{align}
(k+1)^3-(k+1)&=k^3+3k^2+3k+1-k-1\\&=k^3-k+3k^2+3k\\&=(k^3-k)+3(k^2+k)
\end{align}
$$
Since $3(k^2+k)$ can be written as number times $3$ we know that $3|3(k^2+k)$. By our inductions hypothesis $3|k^3-k$. By Proposition 1.2 we know that $3|(k^3-k)+3(k^2+k)$. This shows for any $n>0$ that $3|n^3-n$.
If $3|k^3-k$ is true for $k$, then we also know that it is true for $-k$. This is because $$(-k)^3-(-k)=-(k^3-k)$$
We know that  $3|-(k^3-k)$ by Proposition 1.2.
Thus we know $3|n^3-n$ for all $n\in \mathbb{Z}$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
We proceed with induction on n.
If $n=0$ then $5|n^5-n$ is true since every number divides 0.
Assume $5|k^5-k$ for $k$. We will show that this is true for $k+1$. This means we need to show $5|(k+1)^5-(k+1)$. This means
$$
\begin{align}
(k+1)^5-(k+1)&=k^5+5k^4+10k^3+10k^2+5k+1-k-1\\&=k^5-k+5(k^4+2k^3+2k^2+k)
\end{align}
$$
Since $5(k^4+2k^3+2k^2+k)$ can be written as number times $5$ we know that $5|5(k^4+2k^3+2k^2+k)$. By our inductions hypothesis $5|k^5-k$. By Proposition 1.2 we know that $5|k^5-k+5(k^4+2k^3+2k^2+k)$. This shows for any $n>0$ that $5|n^5-n$.
If $5|k^5-k$ is true for $k$, then we also know that it is true for $-k$. This is because $$(-k)^5-(-k)=-(k^5-k)$$
We know that  $5|-(k^5-k)$ by Proposition 1.2.
Thus we know $5|n^5-n$ for all $n\in \mathbb{Z}$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### c
Counterexample: $n=2$
$2^4-2=14$
$4\nmid14$
#### 4
Proof
$a^n+1$ is prime, so we know that it has no prime factors other than itself. This means unless $a^n+1$ is two, it must be odd. Since $a>1$ there is no way for $a^n+1$ to be 2. This means that $a^n+1$ is odd. Since $a^n+1$ is odd, then $a^n$ must be even. Since $a^n$ is even, one of its prime factors must be $2$ and $2|a^n$. This is equivalent to $2|a\cdot a\cdot\dots \cdot a$. By Lemma 1.14, 2 must divide $a$. Thus $a$ is even.

Assume to the contrary that $a^n+1$ is prime, but $n$ is not a power of $2$. This means that $n$ has a prime factor that is not a power of $2$. This means there exists $p,k\in \mathbb{Z}$ where $p$ is an odd prime and $pk=n$. This means that $a^{k^p}+1$ is prime. However, since $p$ is odd we know that this can be factored as $(a^k+1)((a^k)^{p-1}-(a^k)^{p-2}+(a^k)^{p-3}+\dots-a^k+1)$. Since $a^n+1$ can be factored when $n$ is not a power a two. Contradiction, $n$ must be a power of two.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 5
Proof
By question 4, we know that if $a^n+1$ is prime, then $a$ must be even. This means there exists $c\in \mathbb{Z}$ where $2c=a$. We can plug this in to get 
$$
\begin{align}
(2c)^2+1=4c^2+1=4(c^2)+1
\end{align}
$$
As $c$ is an integer we know that $c^2$ is also an integer. This shows that we can write $a^2+1$ in the form $4k+1$ with $k=c^2$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 6
##### a
Proof
Since $(a,b)=1$, then $a$ and $b$ are coprime and share no prime factors. Since $a|c$ then there exists $d\in \mathbb{Z}$ where $ad=c$. We can plug this into $b|c$ to get $b|ad$. By Lemma 1.12, either $b|a$ or $b|d$. Since $a$ and $b$ share no prime factors either $b\in \{1,-1\}$ or $b\nmid a$. Either way, $b|d$. This means that there exists $e\in \mathbb{Z}$ where $be=d$. We can multiply both sides by $a$ to get $abe=ad$. Recall that $ad=c$. This means $(ab)e=c$. Since $c$ can be written as $ab$ times a number, $ab|c$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
$a=6,b=4,c=12$
$6|12$ and $4|12$, but $24\nmid12$

##### c
Proof
We proceed by induction on $n$. If $n=1$ then $a_{1}|a_{1}$. If $n=2$ then we have already proven in 6a that $a_{1}|c$ and $a_{2}|c$ means $a_{1}\cdot a_{2}|c$.
Assume that if $a_{j}|c$ each, then $a_{1}\dots a_{k}|c$ for $n=k$. We will will show this is true for $n=k+1$. We know that $a_{k+1}|c$ and $a_{1}\dots a_{k}|c$. By our proof in 6a this means that $a_{1}\dots a_{k}\cdot a_{k+1}|c$. this is equivalent to $a_{1}\dots a_{k+1}|c$. This shows our statement is true for $k+1$. Therefore, if $a_{j}$ each, then $a_{1}\dots a_{n}|c$ for any $n$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 7
Proof
We need to show both $(a,b)=1$ implies $(a+b,ab)=1$ and $(a+b,ab)=1$ implies $(a,b)=1$.
First we show $(a,b)=1$ implies $(a+b,ab)=1$. Let $d=(a+b,ab)$. This means that $d|a=b$ and $d|ab$. By Lemma 1.14 we know that either $d|a$ or $d|b$. Assume without loss of generality that $d|a$. Then by Proposition 1.2 $d|a+b-a$. This means that $d|b$. Since d divides $a$ and $b$ it can be at $(a,b)$. This means $d=1$
Next we show $(a+b,ab)=1$ implies $(a,b)=1$. Let $d=(a,b)$. This means that $d|a$ and $d|b$.
By Proposition 1.2 $d|a+b$ and $d|ab$ as both are linear combinations of $a$ and $b$. Therefore, since $d|a+b$ and $d|ab$ it can be at most the $(a+b,ab)$. This means $d=1$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 8
$$
\begin{align}
1155-2(441)&=273 \\
441-1(273)&=168  \\
273-1(168)&=105  \\
168-1(105)&=63 \\
105-1(63)&=42 \\
63-1(42)&=21 \\
42-2(21)&=0
\end{align}
$$
$$
(1155,441)=(441,273)=(273,168)=(168,105)=(105,63)=(63,42)=(42,21)=(21,0)=21
$$
$$
\begin{align}
(1155,441)=21&=63-1(42) \\
&=63-1(105-63)=2(63)-1(105) \\
&=2(168-105)-105=2(168)-3(105) \\
&=2(168)-3(273-168)=5(168)-3(273) \\
&=5(441-273)-3(273)=5(441)-8(273) \\
&=5(441)-8(1155-2(441))=21(441)-8(1155) \\
21&=21(441)-8(1155)
\end{align}
$$
#### 9
We need to find $a,b\in \mathbb{Z}$ where 
$$
\begin{align}
\frac{a}{11}+\frac{b}{13}&=\frac{7}{143} \\
\frac{13a}{143}+\frac{11b}{143}&=\frac{7}{143}
\end{align}
$$
We need to find an integer linear combination of $13$ and $11$ that adds to 7.
We can use the Euclidean Algorithm. 
$$
\begin{align}
13-11&=2 \\
11-5(2)&=1 \\
2-2(1)&=0 \\
 \\
1&=11-5(2) \\
1&=11-5(13-11) \\
1&=6(11)-5(13)
\end{align}
$$
We can then multiply both sides by $7$ to get 
$$
7=42(11)-35(13)
$$
So $a=-35$ and $b=42$ and 
$$
\frac{-35}{11}+\frac{42}{13}=\frac{7}{143}
$$
