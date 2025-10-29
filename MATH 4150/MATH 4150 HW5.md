#### 1
##### a
$(7,11)=1$
$$
\begin{align}
x^2&\equiv 23 \pmod{7} \\
x^2&\equiv 2 \pmod{7}  \\
x&\equiv3,4\pmod{7}
\end{align}
$$
$$
\begin{align}
x^2&\equiv 24 \pmod{11} \\
x^2&\equiv 1 \pmod{11} \\
x&\equiv 1,10 \pmod{11}
\end{align}
$$
We have 4 cases
Case 1:
$$
\begin{align}
x&\equiv3\pmod{7} \\
x&\equiv1\pmod{11} \\ \\

x&\equiv 45 \pmod{77} 
\end{align}
$$
Case 2:
$$
\begin{align}
x&\equiv4\pmod{7} \\
x&\equiv1\pmod{11} \\ \\

x&\equiv 67 \pmod{77} 
\end{align}
$$
Case 3:
$$
\begin{align}
x&\equiv3\pmod{7} \\
x&\equiv10\pmod{11} \\ \\

x&\equiv 10 \pmod{77} 
\end{align}
$$
Case 4:
$$
\begin{align}
x&\equiv4\pmod{7} \\
x&\equiv10\pmod{11} \\ \\

x&\equiv 32 \pmod{77} 
\end{align}
$$
Solved CRT equations by guessing and checking. 
$$
x\equiv10,32,45,67 \pmod{77} 
$$
##### b
$(3,13)=1$
$$
\begin{align}
x^2&\equiv 11 \pmod{3} \\
x^2&\equiv 2 \pmod{3}  \\
\end{align}
$$
This has no solutions, so there are no solutions
##### c
$(3,5)=(3,7)=(5,7)=1$
$$
\begin{align}
x^2&\equiv 46 \pmod{3} \\
x^2&\equiv 1 \pmod{3}  \\
x&\equiv\pm1\pmod{3}
\end{align}
$$
$$
\begin{align}
x^2&\equiv 46 \pmod{5} \\
x^2&\equiv 1 \pmod{5}  \\
x&\equiv\pm1\pmod{5} \\
\end{align}
$$
$$
\begin{align}
x^2&\equiv 46 \pmod{7} \\
x^2&\equiv 4 \pmod{7}  \\
x&\equiv 2,5\pmod{7}
\end{align}
$$
We have 8 cases
Case 1:
$$
\begin{align}
x&\equiv1\pmod{5} \\
x&\equiv1\pmod{3} \\
x&\equiv2\pmod{7} \\ \\
 \\
x&\equiv1\pmod{15} \\x&\equiv2\pmod{7} \\ \\


x&\equiv 16\pmod{105} 
\end{align}
$$
Case 2:
$$
\begin{align}
x&\equiv1\pmod{5} \\
x&\equiv1\pmod{3} \\
x&\equiv 5\pmod{7} \\ \\
 \\
x&\equiv1\pmod{15} \\x&\equiv 5\pmod{7} \\ \\
x&\equiv 61\pmod{105} 
\end{align}
$$


Case 3:
$$
\begin{align}
x&\equiv-1\pmod{5} \\
x&\equiv-1\pmod{3} \\
x&\equiv2\pmod{7} \\ \\
 \\
x&\equiv-1\pmod{15} \\x&\equiv2\pmod{7} \\ \\


x&\equiv 44\pmod{105} 
\end{align}
$$
Case 4:
$$
\begin{align}
x&\equiv-1\pmod{5} \\
x&\equiv-1\pmod{3} \\
x&\equiv 5\pmod{7} \\ \\
 \\
x&\equiv-1\pmod{15} \\x&\equiv 5\pmod{7} \\ \\
x&\equiv 89\pmod{105} 
\end{align}
$$
Case 5:
$$
\begin{align}
x&\equiv1\pmod{5} \\
x&\equiv-1\pmod{3} \\
x&\equiv 2\pmod{7} \\ \\
 \\
x&\equiv11\pmod{15} \\
x&\equiv-4\pmod{15} \\x&\equiv 2\pmod{7} \\ \\
x&\equiv 86\pmod{105} 
\end{align}
$$
Case 6:
$$
\begin{align}
x&\equiv1\pmod{5} \\
x&\equiv-1\pmod{3} \\
x&\equiv 5\pmod{7} \\ \\
 \\
x&\equiv-4\pmod{15} \\x&\equiv 5\pmod{7} \\ \\
x&\equiv 26\pmod{105} 
\end{align}
$$
Case 7:
$$
\begin{align}
x&\equiv-1\pmod{5} \\
x&\equiv1\pmod{3} \\
x&\equiv 2\pmod{7} \\ \\
 \\
x&\equiv 4\pmod{15} \\
x&\equiv 2\pmod{7} \\ \\
x&\equiv 79\pmod{105} 
\end{align}
$$
Case 8:
$$
\begin{align}
x&\equiv-1\pmod{5} \\
x&\equiv1\pmod{3} \\
x&\equiv 5\pmod{7} \\ \\
 \\
x&\equiv4\pmod{15} \\x&\equiv 5\pmod{7} \\ \\
x&\equiv 19\pmod{105} 
\end{align}
$$

Solved CRT equations by guessing and checking. 
$$
x\equiv 16,19,26,44,61,79,86,89 \pmod{105}
$$
#### 2
Proof
Since all the numbers in the series are perfect squares they must all be quadratic roots modulo $p$. We have to show that these are all distinct. 
By Proposition 3.1 if $x^2\equiv a \pmod p$ then $(-x)^2\equiv (p-x)^2\equiv a \pmod p$ otherwise it has no solutions. If $1\leq x\leq \frac{p-1}{2}$ like in the list, only one of these solutions is possible. So restricting $1\leq x\leq \frac{p-1}{2}$ get rid of one the two possible solutions to the congruence. This means all of the sequence is distinct modulo $p$. 
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 3
##### a
Proof
As shown in part two, we can write the quadratic residues as
$$
1^2,2^2,\dots ,\left( \frac{p-1}{2} \right)^2
$$
Using the standard formula for sum we know the sum of these is
$$
\begin{align}
\sum_{i=1}^{(p-1)/2}i^2&=\frac{\frac{p-1}{2}\left( \frac{p-1}{2} +1 \right)\left(2 \frac{p-1}{2} +1 \right)}{6} \\
&=\frac{\frac{p-1}{2}\left( \frac{p-1}{2} +1 \right)\left(p-1 +1\right)}{6} \\
&=\frac{(p-1)\left( \frac{p}{2}+\frac{1}{2} \right)(p)}{12} \\
&=\frac{(p-1)\left( p+1 \right)(p)}{24} \\
 \\
24\sum_{i=1}^{(p-1)/2}i^2 &=(p-1)(p+1)(p)
\end{align}
$$
Therefore, we know that $p|24\sum_{i=1}^{(p-1)/2}i^2$. In addition since $p>3$ we know that $(p,24)=1$. This means that $p|\sum_{i=1}^{(p-1)/2}i^2$. This tells us that $p$ divides the sum of quadratic residues.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
The sum of the non quadratic residues squared is the same as the sum of all residues squared minus the square of the quadratic residues.
Since the quadratic residues are 
$$
1^2,2^2,\dots ,\left( \frac{p-1}{2} \right)^2
$$
The square of the quadratic residues squared is
$$
1^4,2^4,\dots ,\left( \frac{p-1}{2} \right)^4
$$
$$
\begin{align}
\sum_{i=1}^pi^2 -\sum_{i=1}^{(p-1)/2}i^2&=\frac{p(p+1)(2p+1)}{6}-\frac{\frac{p-1}{2}\left( \frac{p-1}{2} +1 \right)\left(2 \frac{p-1}{2} +1 \right)\left( 3\left( \frac{p-1}{2} \right)^2+3\left( \frac{p-1}{2} \right) -1 \right)}{30} \\
&=\frac{p(p+1)(2p+1)}{6}-\frac{(p-1)\left(\frac{p}{2} +\frac{1}{2} \right)\left(p \right)\left( 3\left( \frac{p-1}{2} \right)^2+3\left( \frac{p-1}{2} \right) -1 \right)}{60} \\
&=\frac{10p(p+1)(2p+1)}{60}-\frac{(p-1)\left(\frac{p}{2} +\frac{1}{2} \right)\left(p \right)\left( 3\left( \frac{p-1}{2} \right)^2+3\left( \frac{p-1}{2} \right) -1 \right)}{60}  \\
&=\frac{10p(p+1)(2p+1)-(p-1)\left(\frac{p}{2} +\frac{1}{2} \right)\left(p \right)\left( 3\left( \frac{p-1}{2} \right)^2+3\left( \frac{p-1}{2} \right) -1 \right)}{60}  \\
&=p\frac{10(p+1)(2p+1)-(p-1)\left(\frac{p}{2} +\frac{1}{2} \right)\left( 3\left( \frac{p-1}{2} \right)^2+3\left( \frac{p-1}{2} \right) -1 \right)}{60} \\
 \\
60(\sum_{i=1}^pi^2 -\sum_{i=1}^{(p-1)/2}i^2)&=p(10(p+1)(2p+1)-(p-1)\left(\frac{p}{2} +\frac{1}{2} \right)\left( 3\left( \frac{p-1}{2} \right)^2+3\left( \frac{p-1}{2} \right) -1 \right))
\end{align}
$$
From this we can see that since $60\left( \sum_{i=1}^pi^2 -\sum_{i=1}^{(p-1)/2}i^2 \right)$ can be written as a multiple of $p$ then $p|60\left( \sum_{i=1}^pi^2 -\sum_{i=1}^{(p-1)/2}i^2 \right)$. Since $p>5$ then we know $(p,60)=1$. This tells us that $p|\sum_{i=1}^pi^2 -\sum_{i=1}^{(p-1)/2}i^2$. This means $p$ divides the sum of the squares of non quadratic residues.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 4
Proof
The Legendre Symbol is $-1$ when a number is not a quadratic residue and $1$ when a number is a quadratic residue so this equation is equivalent to saying the exactly half the numbers from $1,\dots,\frac{p-1}{2}$ are quadratic residues. 

We already know that there are the same number of quadratic residues and quadratic non residues, from $1,\dots ,p$.

By theorem 4.6 we know that since $p\equiv1 \pmod4$ then $\left( \frac{-1}{p} \right)=1$. This tells us for any residue $a$ that
$$
\left( \frac{p-a}{p} \right)=\left( \frac{-a}{p} \right)=\left( \frac{{-1}}{p} \right)\left( \frac{a}{p} \right)=\left( \frac{a}{p} \right)
$$
So for any quadratic residue, $a \leq\frac{p-1}{2}$ there is a corresponding residue $a-p$ greater than $\frac{p-1}{2}$ where $\left( \frac{p-a}{p} \right)=\left( \frac{a}{p} \right)$. This tells half of the quadratic residues are at most $\frac{p-1}{2}$ and the other half are greater than $\frac{p-1}{2}$. This also tells us half of the quadratic non residues are at most $\frac{p-1}{2}$ and the other half are greater than $\frac{{p-1}}{2}$. Since there are the same number of quadratic residues and quadratic non residues, from $1,\dots ,p$ and half of the quadratic residues and quadratic non residues are at most $\frac{p-1}{2}$. There are the same number of quadratic residues and quadratic non residues at most $\frac{p-1}{2}$. This proves the summation.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 5
##### a
Proof
If one $2,5$ are a quadratic residues then we are done.
By proposition 4.5 we know that $\left( \frac{2}{p} \right)\left( \frac{5}{p} \right)=\left( \frac{10}{p} \right)$. This means if both $2,5$ are not quadratic residues then $10$ is one since $\left( \frac{10}{p} \right)=\left( \frac{2}{p} \right)\left( \frac{5}{p} \right)=(-1)(-1)=1$. At least one of $2,5,10$ must be a quadratic residue.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
Exactly two of $2,5,10$ cannot be quadratic residues.
By proposition 4.5 we know that $\left( \frac{2}{p} \right)\left( \frac{5}{p} \right)=\left( \frac{10}{p} \right)$. 
We have 3 cases.
If $2,5$ are both quadratic residues then $10$ is also since $\left( \frac{10}{p} \right)=\left( \frac{2}{p} \right)\left( \frac{5}{p} \right)=(1)(1)=1$
If exactly one of $2,5$ are a quadratic residue then $10$ is not since $\left( \frac{10}{p} \right)=\left( \frac{2}{p} \right)\left( \frac{5}{p} \right)=(-1)(1)=-1$
If both $2,5$ are not quadratic residues then $10$ is a quadratic residue since $\left( \frac{10}{p} \right)=\left( \frac{2}{p} \right)\left( \frac{5}{p} \right)=(-1)(-1)=1$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### c
Proof
By part a we know one of $2,5,10$ must be a quadratic residue. We have 3 cases.
Case 1: $2$ is a quadratic residue
Since $1=1^2$ is a perfect square, it must be a quadratic residue. Therefore $1,2$ are both quadratic residues and two consecutive residues are quadratic.

Case 2: $5$ is a quadratic residue
Since $4=2^2$ is a perfect square, it must be a quadratic residue. Therefore $4,5$ are both quadratic residues and two consecutive residues are quadratic.

Case 3: $10$ is a quadratic residue
Since $9=3^2$ is a perfect square, it must be a quadratic residue. Therefore $9,10$ are both quadratic residues and two consecutive residues are quadratic.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 6
Proof
Numbers in this form can be expressed $p\equiv1 \pmod4$. By Theorem 4.6 we know that $\left( \frac{-1}{p} \right)=1$.
Assume to the contrary there are finite numbers of the form $4n+1$. Then we can list out these numbers as $p_{1},\dots,p_{r}$. Consider the number $N=4p_{1}^2\dots p_{r}^2+1$. Any prime factor must be of the form $4n+1$ or $4n+3$. Any prime factor $p$ of $N$ must divide $N$ so we know that 
$$
\begin{align}
4p_{1}^2\dots p_{r}^2+1&\equiv0 \pmod p \\
4p_{1}^2\dots p_{r}^2&\equiv-1 \pmod p  \\
(2p_{1}\dots p_{r})^2&\equiv-1 \pmod p
\end{align}
$$
This tells us that $-1$ is a quadratic residue of $p$ so $\left( \frac{-1}{p} \right)=1$. By Theorem 4.6 this means that $p\equiv1 \pmod 4$. However, for any $p_{i}$ in the list of $p_{1},\dots,p_{r}$ we know that $p_{i} \equiv 1 \pmod {p_{i}}$. So no prime of the form $4n+1$ can divide $N$. Contradiction, there must be infinite primes of the form $4n+1$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 7
Proof
Since $p=q+4a$ we know that $p\equiv q \pmod 4$.
We have two cases. 
Case 1: $p\equiv q \equiv1 \pmod 4$
Since $p\equiv q \equiv1 \pmod 4$ by quadratic reciprocity we know that $\left( \frac{p}{q} \right)=\left( \frac{q}{p} \right)$. 
$$
\begin{align}
\left( \frac{p}{q} \right)&=\left( \frac{q+4a}{q} \right) \\
&=\left( \frac{4a}{q} \right) \\
&=\left( \frac{a}{q} \right)
\end{align}
$$
$$
\begin{align}
\frac{q}{p}&=\left( \frac{p-4a}{p} \right) \\
&=\left( \frac{-4a}{p} \right) \\
&=\left( \frac{-1}{p} \right)\left( \frac{a}{p} \right)
\end{align}
$$
Since $p\equiv1 \pmod 4$ by Theorem 4.6 we know that $\left( \frac{-1}{p} \right)=1$
So we know that
$$
\left( \frac{a}{q} \right)=\left( \frac{p}{q} \right)=\left( \frac{q}{p} \right)=\left( \frac{a}{p} \right)
$$
Case 2: $p\equiv q \equiv3 \pmod 4$
Since $p\equiv q \equiv3 \pmod 4$ by quadratic reciprocity we know that $\left( \frac{p}{q} \right)=-\left( \frac{q}{p} \right)$.
$$
\begin{align}
\left( \frac{p}{q} \right)&=\left( \frac{q+4a}{q} \right) \\
&=\left( \frac{4a}{q} \right) \\
&=\left( \frac{a}{q} \right)
\end{align}
$$
$$
\begin{align}
\left( \frac{q}{p} \right)&=\left( \frac{p-4a}{p} \right) \\
&=\left( \frac{-4a}{p} \right) \\
&=\left( \frac{-1}{p} \right)\left( \frac{a}{p} \right)
\end{align}
$$
Since $p\equiv3 \pmod 4$ by Theorem 4.6 we know that $\left( \frac{-1}{p} \right)=-1$
So we know that
$$
\left( \frac{a}{q} \right)=\left( \frac{p}{q} \right)=-\left( \frac{q}{p} \right)=-\left( -\left( \frac{a}{p} \right) \right)=\left( \frac{a}{p} \right)
$$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 8
##### a
Proof
$$
\left( \frac{-2}{p} \right)=\left( \frac{-1}{p} \right)\left( \frac{2}{p} \right)
$$
This means $\left( \frac{-2}{p} \right)=1$ if $\left( \frac{-1}{p} \right)=\left( \frac{2}{p} \right)=1$ or $\left( \frac{-1}{p} \right)=\left( \frac{2}{p} \right)=-1$.
We have two cases:
Case 1:
$\left( \frac{{-1}}{p} \right)=1$ if $p\equiv 1 \pmod4$. $\left( \frac{2}{p} \right)= 1$ if $p\equiv1,7 \pmod 8$. So $p\equiv1 \pmod8$
Case 2:
$\left( \frac{{-1}}{p} \right)=-1$ if $p\equiv 3 \pmod4$.$\left( \frac{2}{p} \right)= -1$ if $p\equiv3,5 \pmod 8$. So $p\equiv3 \pmod8$

Combining the two cases $(\frac{-2}{p})=1$ if $p\equiv 1,3 \pmod 8$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
We want find values where $\left( \frac{3}{p} \right)=1$
By quadratic reciprocity we know that
$$
\left( \frac{3}{p} \right)= \begin{cases}
\left( \frac{p}{3} \right) & p\equiv1 \pmod4 \\
-\left( \frac{p}{3} \right) & p\equiv{3} \pmod4
\end{cases}
$$
We know that $\left( \frac{1}{3} \right)=1$ and $\left( \frac{2}{3} \right)=-1$. 

So $\left( \frac{3}{p} \right)=1$ if $p\equiv1 \pmod4$ and $p\equiv1 \pmod3$ or if $p\equiv{3} \equiv -1 \pmod4$ and $p\equiv 2 \equiv -1\pmod3$.
If $p\equiv1 \pmod4$ and $p\equiv1 \pmod3$ then $p\equiv1 \pmod{12}$. 
If $p\equiv{-1} \pmod4$ and $p\equiv -1 \pmod3$ then $p\equiv-1 \pmod{12}$
Combining these cases we know that $p\equiv\pm1 \pmod{12}$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### c
$$
\left( \frac{-3}{p} \right)=\left( \frac{-1}{p} \right)\left( \frac{3}{p} \right)
$$
This means $\left( \frac{-3}{p} \right)=1$ if $\left( \frac{-1}{p} \right)=\left( \frac{3}{p} \right)=1$ or $\left( \frac{-1}{p} \right)=\left( \frac{3}{p} \right)=-1$.
$\left( \frac{-1}{p} \right)=1$ if $p\equiv 1 \pmod4$. 

We have two cases:
Case 1:
$\left( \frac{{-1}}{p} \right)=1$ if $p\equiv 1 \pmod4$. $\left( \frac{3}{p} \right)= 1$ if $p\equiv \pm1 \pmod {12}$ by part $b$. So $p\equiv1 \pmod {12}$.
Case 2:
$\left( \frac{{-1}}{p} \right)=-1$ if $p\equiv 3 \pmod4$.$\left( \frac{3}{p} \right)= -1$ if $p\not\equiv \pm1 \pmod {12}$. So $p\equiv 3,7 \pmod{12}$. We exclude $3$ since $\left( \frac{3}{3} \right)=0$. So $p\equiv7 \pmod{12}$.

Combining the two cases we get $p\equiv 1,7 \pmod{12}$. This is equivalent to $p\equiv 1 \pmod{6}$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
