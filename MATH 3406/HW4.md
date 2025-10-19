#### 1
Proof
If $p$ is a polynomial in a real space it can be expressed as 
$$
p(x)=c(x-\lambda_{1})\dots(x-\lambda_{m})(x^2+b_{1}x+c_{1})\dots(x^2+b_{n}x+c_{n})
$$
This tells us that the degree of $p$ is $m+2n$. We know the degree of $p$ is odd. Since $2n$ is always even, that means $m$ is odd. We can't have a negative number of terms, so the least value for $m$ is $1$. This tells us $p$ has at least $1$ real root.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 2
##### a
Proof
If $U \subseteq \text{null}(T)$ that means for any $u\in U$ then $Tu=0$. Since $U$ is a subspace then $0\in U$. This tells us for any $u \in U$ then $Tu \in U$. This means $U$ is invariant under $T$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### b
Proof
If $\text{range}(T) \subseteq U$ then for any $v\in V$ we know that $Tv\in U$. Since $U \subseteq V$ this tells us that $Tu\in U$. This means $U$ is invariant under $T$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 3
Proof
If $ST$ has an eigenvalue $\lambda$ we want to show that $\lambda$ is also an eigenvalue of $TS$. 
If $ST$ has an eigenvalue $\lambda$ then for some $v\in V$ $STv=\lambda v$. Consider $Tv$. 
Case: $Tv\neq0$
$$
\begin{align}
TS(Tv)&=T(ST)v \\
&=\lambda Tv
\end{align}
$$
So if $Tv\neq0$ then $\lambda$ is an eigenvalue of $TS$. 

Case: $Tv=0$
If $Tv=0$ then $STv=S(0)=0$. So then $\lambda=0$. This tells us that $ST-0 I=ST$ is not invertible. 

If $ST$ is invertible then both $S,T$ are invertible. This means $S^{-1}$ and $T^{-1}$ exist. Then $TS(S^{-1}T^{-1})=I$. So $TS$ has an inverse. This shows if $ST$ is invertible then $TS$ is in vertible. We can use similar logic to show the converse. Therefore $ST$ is invertible if and only if $TS$ is invertible. This means if $ST$ is not invertible then $TS$ is not invertible.

From this we know $TS$ is not invertible and has an also has an eigenvalues of $0$.

We can use similar logic to show if $TS$ has eigenvalue $\lambda$ then $\lambda$ is also an eigenvalue of $ST$. Therefore $TS$ and $ST$ have the same eigenvalues.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 4
$$
\begin{gather}
(w,z) \\
T(w,z)= (-z,w) \\
T^2(w,z)=T(-z,w)=(-w,-z)
\end{gather}
$$
Minimal polynomial by inspection is
$$
p(z)=z^2+1
$$
#### 5
Proof
Let $r(z)$ be the minimal polynomial of $T-\lambda I$.
$q$ is monic and has the same degree as $p$.
$$
q(T-\lambda I)=p(T-\lambda I+\lambda I)=p(T)=0
$$
This tells us that $q$ is a multiple of the minimal polynomial $r$. From this we know the degree of $q$ is greater than or equal to $r$. 

Let $s(z)=r(z-\lambda)$. We know that $s$ and $r$ have the same degree.
$$
\begin{align}
s(T)=r(T-\lambda I)=0
\end{align}
$$
So $s$ is a multiple of the minimal polynomial $p$. This tells us the degree of $s$ is greater than or equal to the degree of $p$. This is equivalent to the degree of $r$ being greater that or equal to the degree of $r$. Since we also know the degree of $q$ is greater than or equal to $r$ this means the degree of $r$ is equal to the degree of $q$. Since $q$ is a monic polynomial with the same degree as the minimal polynomial of $T-\lambda I$ where $q(T-\lambda I)=0$ then $q$ is the unique minimal polynomial of $T-\lambda I$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 6
Counterexample:
$$
\begin{gather}
T=\begin{pmatrix}
0 & -1\\1 & 0
\end{pmatrix} \\
T^2=\begin{pmatrix}
-1 & 0 \\
0 & -1
\end{pmatrix}
\end{gather}
$$
$T^2$ is upper triangular but $T$ is not. $T$ has no real eigenvalues therefore cannot be expressed as an upper triangular matrix in any basis.