#### 1
##### a
Proof
By corollary 2.15 we know that $a^p\equiv a \pmod p$ and $b^p\equiv b \pmod p$. We can plug this into $a^p\equiv b^p \pmod p$ to get that $a\equiv b \pmod p$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
We know by part a that $a\equiv b \pmod p$. From this we know there exists $c\in \mathbb{Z}$ where $a=b+pc$. We can then take each side to the power of $p$ to get $a^p=(b+pc)^p$. Using the binomial theorem we can find that $a^p=b^p+\binom{p}{1} b^{p-1}pc+\binom{p}{2} b^{p-2}pc+\dots+(pc)^p$ . $p$ choose $1$ is just equal to $p$ so we can rewrite the equation
$$
\begin{align}
a^p&=b^p+ b^{p-1}p^2c+\binom{p}{2} b^{p-2}p^2c+\dots+(pc)^p \\
a^p-b^p&=b^{p-1}p^2c+\binom{p}{2} b^{p-2}p^2c+\dots+(pc)^p \\
a^p-b^p&=b^{p-1}p^2c+\binom{p}{2} b^{p-2}p^2c+\dots+p^pc^p \\
a^p-b^p&=p^2(b^{p-1}c+\binom{p}{2} b^{p-2}c+\dots+p^{p-2}c^p)
\end{align}
$$
From this we can find that $a^p\equiv b^p \pmod {p^2}$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 2
##### a
I have copied the part of my answer to HW1 problem 2 here.

Proof
We show $m|n$ implies $a^m-1|a^n-1$. Since $m|n$ there exists $c\in \mathbb{Z}$ where $cm=n$. Then $$a^n-1=a^{cm}-1=(a^m)^c-1=(a^m-1)((a^m)^{c-1}+(a^m)^{c-2}+\dots(a^m)+1)$$Since $a^n-1$ can be written as $a^m-1$ times a number, we know that $a^m-1|a^n-1$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

Proof
We have proven a more general case of this problem in HW1 problem 2. We know that if $m|n$ then $a^m-1|a^n-1$. This also applies if we replace $a$ with 2. So from that we know that if $a|b$ then $2^a-1|2^b-1$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

##### b
Proof
First we prove that $2^{n-1}\equiv1 \pmod n$ implies $n$ is an odd pseudo prime.
We can multiply by $2$ on both sides to show that $2^n\equiv2 \pmod n$, showing that $n$ is pseudo prime. 
We next need to prove $n$ is odd. Assume to the contrary that $n$ is even. In addition, since $n$ is composite then $n\geq4$. Since $2^{n-1}\equiv1 \pmod n$ we know that $n|2^{n-1}-1$. Since $n$ is even and divides $2^{n-1}-1$ then $2^{n-1}-1$ must be even also. However, since for all $n\geq4$ we know that $2^{n-1}$ is even, $2^{n-1}-1$ is odd. Contradiction, $n$ must be odd, and $n$ must be an odd pseudo prime.  

Next we prove that $n$ being pseudo prime means $2^{n-1}\equiv1 \pmod n$.
By definition if, $n$ is an pseudo prime, it must meet the condition that $2^n\equiv2 \pmod n$. Since $n$ is then $(2,n)=1$. This tells us that $\bar{2}$ exists. So we can multiply that on both sides to get that $2^{n-1}\equiv1 \pmod n$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### c
Proof

We want to show that $2^{m-1}\equiv1 \pmod m$. In other terms, we want to show that $m|2^{m-1}-1$. First, since $n$ is an odd pseudo prime we know from part b that $2^{n-1}\equiv1 \pmod n$. This means there exists some $k\in \mathbb{Z}$ where $2^n-1=kn$. Since $m=2^n-1$ we know that
$$
\begin{align}
m-1&=2^n-2 \\
m-1&=2(2^{n-1}-1) \\
m-1&=2(kn) \\
\end{align}
$$
We can then plug this in to get $2^{m-1}-1= 2^{2kn}-1$. Since $n|2kn$ using part a we know that $m=2^n-1|2^{2kn}-1=2^{m-1}-1$.  This tells us that $m|2^m-1$, or that $2^{m-1} \equiv2 \pmod m$. By part b this means that $m$ is an odd pseudo prime.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### d
Proof
Assume to the contrary that there are finitely many odd pseudo primes. By the well ordering principal this means there is a greatest odd pseudo prime $s$. By part c we know that $2^s-1$ is also an odd pseudo prime. However, $2^s-1>s$ contradicting $s$ being the greatest odd pseudo prime. Contradiction, there must be infinitely many odd pseudo primes. 
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 3
##### a
$\phi(20)=\phi(4)\phi(5)=2\cdot4=8$
$$
\begin{align}
29^{198}\equiv 9^{198}\equiv 9^{8^{24}}9^6\equiv 1^{24}9^6\equiv729 \cdot729\equiv9\cdot9\equiv81\equiv 1 \pmod {20}
\end{align}
$$
##### b
$\phi(26)=\phi(2)\phi(13)=12$
$$
99^{999999}\equiv 21^{999999}\equiv 21^{12^{83333}}21^3\equiv1^{8333}21^3\equiv(-5)^3\equiv -125\equiv5 \pmod {26}
$$
#### 4
Proof
If $r_{i}$ is a residue of $m$ then $(m,r_{i})=1$ using Euclid's Algorithm we also know that $1=(m,r_{i})=(m-r_{i},r_{i})=(m-r_{i},r_{i}+m-r_{i})=(m-r_{i},m)$. Since $m-r_{i}$ is coprime with $m$ something equivalent to it must be in the reduced residue system. It is impossible for $m-r_{i}=r_{i}$ since that would mean $m=2r_{i}$ and $r_{i}$ not be coprime with m. This means for each $r_{i}$ there is another residue that is equivalent to $m-r_{i}$ if we add each of these together the $r_{i}$ cancels out and we add together $m$ a bunch of times. This is equivalent to $0$ modulo $m$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 5
##### a
Proof
We want to show for some $g,q \in \mathbb{Z}$ that $\lambda(gq)=\lambda(g)\lambda(q)$. 
Let $p=g_{1}g_{2}g_{3}\dots g_{k}$ where $g_{1},\dots g_{k}$ are prime numbers.
Let $q=q_{1}q_{2}q_{3}\dots q_{c}$ where $q_{1},\dots,q_{c}$ are prime numbers.
This gives us that $\lambda(g)=(-1)^k$ and $\lambda(q)=(-1)^c$ so $\lambda(g)\lambda(q)=(-1)^{k+c}$
We can say that $gq=g_{1}g_{2}g_{3}\dots g_{k}q_{1}q_{2}q_{3}\dots q_{c}$ .Since these are are all primes we can rewrite $gq$ as $gq=p_{1}p_{2}p_{3}\dots p_{k+c}$. This means that $\lambda(gq)=(-1)^{k+c}$. Since $\lambda(g)\lambda(q)=(-1)^{k+c}=\lambda(gq)$ then $\lambda$ is completely multiplicative.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
Since $\lambda$ is completely multiplicative it is also multiplicative. By Theorem 3.1 we also know that $F(n)=\Sigma_{d|n}\lambda(d)$ is multiplicative. This tells us that $F(n)$ is defined by its behavior on prime powers.

Let $p,k \in \mathbb{Z}$ where $p$ is prime.
We find the behavior of $F(p^k)$. All the divisors of $p^k$ are the powers of $p$ up to $p^k$
$$
\begin{align}
\lambda(1)&=1 \\
\lambda(p)&=-1 \\
\lambda(p^2)&=1 \\
\dots \\
\lambda(p^k)&=(-1)^k
\end{align}
$$
$F(p^k)$ would be the sum of all of these numbers. Notice how it alternates between $1$ and $-1$. Most of these would cancel each other out. If the total number of values were even, then the sum would be $0$ with everything canceling each other out. If the total number of values were odd, then there would a $1$ value at the end that didn't cancel with every thing. This corresponds with if $k$ is odd then $F(p^k)=0$ and if $k$ is even then $F(p^k)=1$.

Let $m=p_{1}^{a_{1}}p_{2}^{a_{2}}\dots p_{k}^{a_{k}}$. Then since $F(n)$ is multiplicative we know that $F(m)=F(p_{1}^{a_{1}})F(p_{2}^{a_{2}})\dots F(p_{k}^{a_{k}})$. The only way for $F(m)=1$ is if $F(p_{1}^{a_{1}})=F(p_{2}^{a_{2}})=\dots =F(p_{k}^{a_{k}})=1$. This means $a_{1},\dots a_{k}$ are all even. This means there exists $c_{1},\dots c_{k}$ where for $a_{i}=2c_{i}$ for all $1\leq i \leq k$. This means $m=p_{1}^{2c_{1}}p_{2}^{2c_{2}}\dots p_{k}^{2c_{k}}=(p_{1}^{c_{1}}p_{2}^{c_{2}}\dots p_{k}^{c_{k}})^2$ which tells us that if $F(m)=1$ then $m$ is a perfect square. If the power of any prime in the prime factorization of $m$ is odd then $m$ is not a perfect square and the product would result in $0$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 6
Proof
Let $p,a \in \mathbb{Z}$ with $p$ being prime. By Theorem 3.3 $\phi(p^a)=p^a-p^{a-1}=p^{a-1}(p-1)$. Since $\phi(n)$ is multiplicative we know that $\phi(n)=\phi(p_{1}^{a_{1}})\phi(p_{2}^{a_{2}})\dots\phi(p_{k}^{a_{k}})$. We can substitute what we found to get that 
$$
\begin{align}
\phi(n)&=p_{1}^{a_{1}-1}(p_{1}-1)p_{2}^{a_{2}-1}(p_{2}-1)\dots p_{k}^{a_{k}-1}(p_{k}-1) \\
&=p_{1}^{a_{1}-1}p_{2}^{a_{2}-1}\dots p_{k}^{a_{k}-1}\prod _{i=1}^m(p_{i}-1)
\end{align}
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 7
Proof
Since $\phi(n)$ counts numbers less than $n$ coprime with $n$, it has a lower bound of $k$. We can't count more numbers than the amount we search through.

By question 6 we know $k=p_{1}^{a_{1}-1}p_{2}^{a_{2}-1}\dots p_{k}^{a_{k}-1}\prod _{i=1}^m(p_{i}-1)$. This tells us that $p_{i}-1\leq k$ for all $1\leq i \leq k$ since otherwise $p_{1}^{a_{1}-1}p_{2}^{a_{2}-1}\dots p_{k}^{a_{k}-1}\prod _{i=1}^m(p_{i}-1)$ would be greater than k. This is equivalent to saying $p_{i}\leq k+1$. This tells us that $n=p_{1}^{a_{1}}p_{2}^{a_{2}}\dots p_{k}^{a_{k}}\leq (k+1)^{a_{1}+a_{2}+\dots+a_{k}}$. This is finite since it is made up entirely of integers. 

Since $n$ has a finite lower and upper bound, $\phi(n)=k$ has finite solutions.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

#### 8
##### a
Proof
By the division algorithm all residues must be between $0$ and $n$ so there are at most $n$ residues. This tells us that $\phi(n)\leq n$.

Now we prove $\frac{\sqrt{ n }}{2}\leq \phi (n)$
By theorem 3.4 $\phi (n)=n \prod_{p|n}\left( 1-\frac{1}{p} \right)$. Or in other words if $n$ has a prime factorization of $p_{1}^{a_{1}}\dots p_{k}^{a_{k}}$ then $\phi(n)=n\prod_{i=1}^k\left( 1-\frac{1}{p_{i}} \right)$
We proceed with induction on the number of indistinct prime factors. This means at each step we will multiply by a prime. Due to the fundamental theorem of arithmetic, if we have a base case of $n=1$ this will induct to all positive integers.
Base Case $n=1$
$\phi(1)=1$. $\frac{1}{2}\leq1$.
Base Case n=2
$\phi(2)=1$. $\frac{\sqrt{ 2 }}{2}\leq2$

Induction step. Assume for $n$ that $\frac{\sqrt{ n }}{2}<\phi (n)$. Also assume for any positive integer $m$ less than $n$ that $\frac{\sqrt{ m }}{2}\leq \phi (m)$. We will prove that for any prime $p$ that $\frac{\sqrt{ np }}{2}<\phi(pn)$. 

For reasons that become clear later, we don't want to $p$ to be equal to $2$
If $p=2$ we can add it to the prime factorization and remove any other prime in the prime factorization, $p'$. We call this new number created by this $n'$ Since all primes are greater than or equal to $2$ this other prime is greater than $2$. This means $n'p'=np$. To show $\frac{\sqrt{ np }}{2}<\phi(pn)$ we can also show $\frac{\sqrt{ n'p' }}{2}<\phi(p'n')$. The main difference is we have a guarantee that $p'\geq3$. Since $n'\leq n$ we know by our strong induction hypothesis that $\frac{\sqrt{ n' }}{2}\leq \phi(n')$. We can do this only if our prime factorization contains a prime other than $2$, this means we need to also to prove the case where $np$ is a power of $2$. 

Let the prime factorization of $n'$ be $p_{1}^{a_{1}}\dots p_{k}^{a_{k}}$.

We have three cases. Either $np$ is a power of two or $np$ is not a power of two and either $p'=p_{i}$ for some $1\leq i\leq k$ or $p'\neq p_{i}$ for any $1\leq i\leq k$.

Case $np$ is a power of $2$.
Since $np$ is a power of $2$ there exists some $c$ where $np=2^c$. Then $\phi(2^c)=2^c-2^{c-1}=2^c\left( 1-\frac{1}{2} \right)=2^{c-1}$. Then $\frac{\sqrt{ np }}{2}=\frac{\sqrt{ 2^c }}{2}=2^{\frac{c}{2}-1}\leq 2^{c-1} = \phi(np)$

Case $p'=p_{i}$.
If $p'=p_{i}$ for some $1\leq i\leq k$ that means the prime factorization of $n'p_{i}$ is $p_{1}^{a_{1}}\dots p_{i}^{a_{i}+1} \dots p_{k}^{a_{k}}$ since we just multiple the original prime factorization by $p_{i}$. This gives us that $\phi(np)=pn\prod_{i=1}^k\left( 1-\frac{1}{p_{i}} \right)=p\phi(n)$. By our induction hypothesis we know that $\frac{\sqrt{ n }}{2}<\phi(n)$. we can multiply by $p$ on both sides to get that $\frac{p\sqrt{ n }}{2}\leq p\phi(n)$. For any positive integer $\sqrt{ p }\leq p$. So we can get that $\frac{\sqrt{ np }}{2}\leq \phi(np)$.

Case $p'\neq p_{i}$ and $p'\neq2$

We prove this using 
If $p'\neq p_{i}$ for any $1\leq i\leq k$ then the prime factorization of $np$ is $p_{1}^{a_{1}}\dots p_{k}^{a_{k}}p$.  $\phi(n'p')=p'n'\left( \prod_{i=1}^k\left( 1-\frac{1}{p_{i}} \right) \right)\left( 1-\frac{1}{p'} \right)=n'(p'-1)\prod_{i=1}^k\left( 1-\frac{1}{p'_{i}} \right)=(p'-1)\phi(n')$. By our induction hypothesis we know that $\frac{\sqrt{ n' }}{2}\leq \phi(n')$. We can multiply by $p-1$ on both sides to get $\frac{(p'-1)\sqrt{ n' }}{2}\leq(p'-1)\phi(n')=\phi(n'p')$. Since we can force $p\neq2$ we and all prime numbers are greater than or equal to $2$ we can say $p\geq3$. When $p\geq3$ then $p-1\leq \sqrt{ p }$.
Then we can say that $\frac{\sqrt{ n'p' }}{2}\leq\frac{(p'-1)\sqrt{ n' }}{2}\leq \phi(n'p')$. This also gives us $\frac{\sqrt{ np }}{2}\leq \phi(np)$.

$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
If $n$ is composite then there exists $p,q \in \mathbb{Z}$ where $n=pq$. Without loss of generality assume that $q\leq p$. This tells us that of all
$$
p,2p,\dots,pq
$$
all $q$ of these numbers are not coprime with $n$. In other words $\phi(n)\leq n-q$. 
 We know that $q\leq\sqrt{ n }$ since otherwise $n=p*q\geq q^2>\sqrt{ n }^2=n$. We can plug $q\leq\sqrt{ n }$ in to find that $\phi(n)\leq n-\sqrt{ n }$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$