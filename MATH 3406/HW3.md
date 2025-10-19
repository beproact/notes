## Jason Low
#### 1
Proof
A basis of $\text{null}(T)$ is $(1,3,0,0),(0,0,1,5)$. This means $\dim \text{null}(T)=2$.
$\dim \text{range}(T)=\dim(\mathbb{F}^4)-\dim \text{null}(T)=4-2=2$.
Since $T$ has a range with dimension of $2$ and the co-domain of $T$ has a dimension of 2 then $T$ is surjective.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 2
Proof
$$
(AC)^t_{j,k}=(AC)_{k,j}
$$
According to how we define matrix multiplication $(AC)_{k,j}$ is equal to the dot product of  row $k$ of $A$ and column $j$ of $C$. However, row $k$ of $A$ is the same as column $k$ of $A^t$ and column $j$ of $C$ is the same as row $j$ of $C^t$. The dot product of row $j$ of $C^t$ and column $k$ of $A^t$ would be equal to $(C^tA^t)_{j,k}$. So we know $(AC)^t_{j,k}=(C^tA^t)_{j,k}$. Since every single row column combination is equal then $(AC)^t=C^tA^t$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 3
Proof
From the definition of an inverse we know that $I=TT^{-1}$. We can apply $\mathcal{M}$ to both sides to get that $\mathcal{M}(I)=\mathcal{M}(TT^{-1})$. The matrix of the identity transformation is just the identity matrix so $I=\mathcal{M}(TT^{-1})$. 
Since we know that $\mathcal{M}(TU)=\mathcal{M}(T)\mathcal{M}(U)$ so we can get that $I=\mathcal{M}(T)\mathcal{M}(T^{-1})$. Since $\mathcal{M}(T)$ multiplied by $M(T^{-1})$ is the identity matrix, $M(T^{-1})$ must be the unique inverse of $\mathcal{M}(T)$. This means that $(\mathcal{M}(T))^{-1}=\mathcal{M}(T^{-1})$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 4
Proof
First we prove if $\text{null}(S)=\text{null}(T)$ there exists invertible $E\in \mathcal{L}(W)$ where $S=ET$.
Let a $v_{1},v_{2},\dots,v_{k}$ be a basis of $V$. Since $\text{null}(S)=\text{null}(T)$ if $S(v_{i})=0$ for some $1\leq i\leq k$then $T(v_{i})=0$. This means $S$ and $T$ have the same basis vectors in $v_{1}$ that do not equal zero. We can label this subset of the basis vectors $u_{1},\dots u_{m}$. 

$T(u_{1}),\dots, T(u_{m})$ must be linearly independent. If they are not then for some $a_{1}T(u_{1})+\dots a_{m}T(u_{m})=0$ for some $a_{1},\dots,a_{m}\in \mathbb{F}$. This means $T(a_{1}u_{1}+\dots+a_{m}u_{m})=0$ so then $a_{1}u_{1}+\dots+a_{m}u_{m}=0$. Which would imply some subset of the basis of $V$ is not independent, which is impossible as all vectors in a basis are linearly independent. We can use similar logic to show that $S(u_{1}),\dots,S(u_{m})$ is linearly independent. 

We can then extend $T(u_{1}),\dots, T(u_{m})$ to a basis of $W$, labeled $T(u_{1}),\dots, T(u_{m}),w_{1},\dots w_{n}$
We can then extend $S(u_{1}),\dots,S(u_{m})$ to a basis of , labeled $S(u_{1}),\dots,S(u_{m}),v_{1},\dots v_{n}$.
We can then make an mapping $E\in \mathcal{L}(W)$ where $E(T(u_{i}))=S(u_{i})$ for $1\leq i\leq m$ and it maps $E(w_{j})=v_{j}$ for $1\leq j\leq n$. 

An inverse of $E$, $E^{-1}$ exists that maps $E^{-1}(S(u_{i}))=T(u_{i})$ and $E^{-1}(v_{j})=w_{j}$. Therefore $E$ is invertible.

Let $v\in V$.
We can express $v=a_{1}v_{1}+\dots+ a_{k}v_{k}$. Note that for any $v_{i}\in v_{1},v_{2},\dots,v_{k}$ where $v_{i} \notin u_{1},\dots u_{m}$ that $S(v_{i})=T(v_{i})=0$.
Then $S(v)=S(a_{1}v_{1},+\dots a_{k}v_{k})=a_{1}S(v_{1})+\dots +a_{k}S(v_{k})=a_{1}S(u_{1})+\dots +a_{k}S(u_{m})$
In addition $T(v)=T(a_{1}v_{1},+\dots a_{k}v_{k})=a_{1}T(v_{1})+\dots+ a_{k}T(v_{k})=a_{1}T(u_{1})+\dots+ a_{k}T(u_{m})$
This means that 
$$
\begin{align}
ET(v)&=E(a_{1}T(u_{1})+\dots+ a_{k}T(u_{m})) \\
&=a_{1}ET(u_{1})+\dots+ a_{k}ET(u_{m}) \\
&=a_{1}S(u_{1})+\dots +a_{k}S(u_{m}) \\
&=S(v)
\end{align}

$$
So there exists an $E \in \mathcal{L}(W)$ where $S=ET$.


Next we prove if there exists $E\in \mathcal{L}(W)$ where $S=ET$ that $\text{null}(S)=\text{null}(T)$.
Let $n\in \text{null}(S)$. Then $0=S(n)=ET(n)$. $E$ is invertible so $E^{-1}$ exists. We can use that to get that $0=T(n)$. So $n \in \text{null}(T)$. This means $\text{null}(S) \subseteq \text{null}(T)$. 
Let $m\in \text{null}(T)$. Then $S(n)=ET(n)=E(0)=0$. Therefore $m\in \text{null}(S)$. This means that $\text{null}(S) \supseteq \text{null}(T)$. 
Therefore $\text{null}(S) = \text{null}(T)$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 5
Proof
We can just show that $\dim \mathcal{L}(V_{1}\times\dots \times V_{m},W) = \dim(\mathcal{L}(V_{1},W)\times\dots \times\mathcal{L}(V_{m},W))$. The dimension of $\dim\mathcal{L}(V,W)=\dim V\cdot\dim W$ and the dimension of a cartesian product is the sum of dimensions so
$$
\begin{align}
\dim \mathcal{L}(V_{1}\times\dots \times V_{m},W)&= (\dim V_{1}+\dots+\dim V_{m}) \dim W
\end{align}
$$
In addition
$$
\begin{align}
\dim(\mathcal{L}(V_{1},W)\times\dots \times\mathcal{L}(V_{m},W))&= (\dim V_{1}\dim W+\dots+\dim V_{m}\dim W) \\
&=(\dim V_{1}+\dots+\dim V_{m}) \dim W \\
&=\dim \mathcal{L}(V_{1}\times\dots \times V_{m},W)
\end{align}
$$
Since $\dim \mathcal{L}(V_{1}\times\dots \times V_{m},W) = \dim(\mathcal{L}(V_{1},W)\times\dots \times\mathcal{L}(V_{m},W))$ we know that $\mathcal{L}(V_{1}\times\dots \times V_{m},W)$ and $\mathcal{L}(V_{1},W)\times\dots \times\mathcal{L}(V_{m},W))$ are isometric.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
#### 6
Proof
Since $U$ is a subspace, it contains $0$. Therefore $v\in v+U$ since $v=v+0$. We then also know that $v \in x+W$. This means $v=x+w_{0}$ for some $w_{0}\in W$

Since $v+U=x+W$ there exists $u\in U$ and $w_{1}\in W$ where $v+u=x+w_{1}$. We can plug in the value we found for $v$ to get $x+w_{0}+u=x+w_{1}$. Simplifying, we get $u=w_{1}-w_{0}$. Since $u$ can be written in term of elements of $W$ this means $u\in W$. This means that $U\subseteq W$.
We can use similar logic to show that $W\subseteq U$. Therefore, $U=W$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$




