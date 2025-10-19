##### 1
Proof
Since $v_{1},v_{2},v_{3},v_{4}$ are linearly independent in $V$, then they have a span in $V$ that is dimension $4$. Lets call the span of $v_{1},v_{2},v_{3},v_{4}$ $U$, and call the span of $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$, $W$.
$v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ are all clearly linear combinations of $v_{1},v_{2},v_{3},v_{4}$. In addition:
$$

\begin{align}
v_{1}&=(v_{1}+v_{2})-(v_{2}-v_{3})-(v_{3}+2v_{4})+2v_{4} \\
v_{2}&=(v_{2}-v_{3})+(v_{3}+2v_{4})-2v_{4} \\
v_{3}&=(v_{3}+2v_{4})-2v_{4} \\
v_{4}&=v_{4}
\end{align}
$$
Since we can represent all of $v_{1},v_{2},v_{3},v_{4}$ in terms of $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ we know that any linear combination of $v_{1},v_{2},v_{3},v_{4}$ can expressed as a linear combination of $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$. Since we can represent all of $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ in terms of $v_{1},v_{2},v_{3},v_{4}$ we know that any linear combination of $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ can be expressed in terms of $v_{1},v_{2},v_{3},v_{4}$. This tells us that $U\subseteq W$ and $W\subseteq U$, so they have that same subset. Since $U$ has dimension $4$ then we know that $W$ has dimension 4. Since $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ has $4$ vectors and spans $W$ which is dimension 4, we know that $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ forms a basis of $W$. This means that $v_{1}+v_{2},v_{2}-v_{3},v_{3}+2v_{4},v_{4}$ is linearly independent.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### 2
Counterexample
$$
\begin{align}
v_{1}&=(1,0,0,0) \\
v_{2}&=(0,1,0,0) \\
v_{3}&=(0,0,1,0) \\
v_{4}&=(0,0,0,1) \\
U&=span\{v_{1},v_{2},v_{3}+v_{4}\}
\end{align}
$$
$v_{1}$ and $v_{2}$ are in $U$ but $v_{3}$ and $v_{4}$ are not. However, $v_{3}+v_{4}$ is in $U$ and there is no way to represent $v_{3}+v_{4}$ in terms of $v_{1}$ and $v_{2}$ so $v_{1}$ and $v_{2}$ do not span $U$. 
##### 3
Proof
Assume to the contrary that $U\cap W=\{0\}$.
We know that $\dim (U+V)=\dim U + \dim V - \dim(U\cap V)$. Since $U\subseteq \mathbb{R}^7$ and $V\subseteq \mathbb{R}^7$ then $U+V\subseteq \mathbb{R}^7$.  $U+V\subseteq \mathbb{R}^7$ and $\dim \mathbb{R}^7=7$, so $\dim(U+V)\leq7$
Since $\dim \{0\}=0$ and $\dim U=\dim V=4$ then, $\dim (U+V) =4+4+0=8$. However, we know that $\dim(U+V)\leq7$. Contradiction, $U\cap W\neq\{0\}$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### 4
Proof
First we show that $p_{0},\dots p_{m}$ are linearly independent. To show this, we need to show that $c_{0}p_{0}+\dots c_{m}p_{m}=0$ only when $c_{0}=c_{1}=\dots=c_{m}=0$. Then
$$
\begin{align}
0&=c_{0}p_{0}+\dots c_{m}p_{m} \\
&=c_{0}x^0(1-x)^{m-0}+\dots+c_{m}x^m(1-x)^{m-m} \\
&=(1-x)^m(c_{0}x^0(1-x)^0+\dots +c_{m}x^m(1-x)^{-m}) \\
&=(1-x)^m\left( c_{0}\left( \frac{x}{1-x} \right)^0+\dots +c_{m}\left( \frac{x}{1-x} \right)^m \right)
\end{align}
$$
$(1-x)^m$ is equal to $0$ only when $x=1$ so whenever $x\neq1$ the other term must equal $0$. So when $x\neq 1$
$$
\begin{align}
0&= c_{0}\left( \frac{x}{1-x} \right)^0+\dots +c_{m}\left( \frac{x}{1-x} \right)^m  \\
\end{align}
$$
If we say that $y=\frac{x}{1-x}$ then we can rewrite this as
$$
\begin{align}
0=c_{0}y^0+\dots+c_{m}y^m
\end{align}
$$
$y^0,\dots, y^m$ is linearly independent. This means the only way for  $0=c_{0}y^0+\dots+c_{m}y^m$ is for $c_{0}=c_{1}=\dots=c_{m}=0$. This also gives us that $p_{0},\dots p_{m}$ are linearly independent. 
Now we show that $p_{0},\dots p_{m}$ is a basis for $\mathcal{P}_{m}(\mathbf{F})$. Since $\mathcal{P}_{m}(\mathbf{F})$ has dimension $m+1$ and $p_{0},\dots p_{m}$ has $m+1$ linearly independent vectors in $\mathcal{P}_{m}(\mathbf{F})$ we know that $p_{0},\dots p_{m}$ form a basis of $\mathcal{P}_{m}(\mathbf{F})$
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### 5
Proof
Assume to the contrary that $v_{1},\dots v_{m}$ is linearly dependent. The there exists $a_{1},\dots a_{m}$ where $a_{1}v_{1}+\dots a_{m}v_{m}=0$. Since linear linear maps preserve additivity and scalar multiplication, then we know that $a_{1}T(v_{1})+\dots+a_{m}T(v_{m})=T(0)$. Every linear map maps $0$ to $0$ so we know that $a_{1}T(v_{1})+\dots+a_{m}T(v_{m})=0$. This contradicts $T(v_{1}),\dots T(v_{m})$ being linearly independent. Therefore, $v_{1},\dots v_{m}$ must be linearly independent.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
##### 6
Lemma: If $T$ is not a scalar multiple of the identity, there exists some $v\in V$ where $Tv$ is not a a scalar multiple of $v$. 
Proof
Assume to the contrary that $T$ is not a scalar multiple of the identity and for all $v\in V$ $Tv$ is a scalar multiple of $v$. Let, $b_{1},\dots b_{n}$ be a basis of $V$. Since for all $v\in V$ we know $Tv$ is a scalar multiple of $v$ we know every $T$ transforms $b_{1},\dots,b_{n}$ to $\lambda_{1}b_{1},\dots \lambda_{n}b_{n}$..
A scalar multiple of the identity,$\lambda I$ where$\lambda\in \mathbb{F}$ would multiply every element of the basis by $\lambda$.  That is a unique linear map from $b_{1},\dots,b_{n}$ to $\lambda b_{1},\dots,\lambda b_{n}$, for every $\lambda$. That means if $\lambda_{1}=\dots=\lambda_{n}$ then $T$ is a scalar multiple of the identity. Therefore, in order for $T$ to not be a scalar multiple of the identity, for some $i,j\in[1,n]$ it is the case that $\lambda_{i}\neq \lambda_{j}$. Then because $T$ is a linear transformation $T(b_{i}+b_{j})=\lambda_{i}b_{i}+\lambda_{j}b_{j}$. However, since $\lambda_{i}\neq \lambda_{j}$ that means that $T(b_{i}+b_{j})$ is not a scalar multiple of $b_{i}+b_{j}$. Contradiction, if $T$ is not a scalar multiple of the identity, there exists some $v\in V$ where $Tv$ is not a a scalar multiple of $v$.  

$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$
Proof
First we prove if $T=\lambda I$ where $\lambda\in \mathbb{F}$ then $ST=TS$. If $ST=S\lambda I=\lambda S=\lambda IS=TS$

Next we prove if $ST=TS$ then $T=\lambda I$ for some $\lambda\in \mathbb{F}$. Assume to the contrary that $ST=TS$ and $T$ is not a scalar multiple of the identity. We will construct an $S$ where $ST\neq TS$.
Since $T$ is not a scalar multiple of the identity, there exists some $v\in V$ where $Tv$ is not a scalar multiple of $v$. This means that the list $Tv,v$ is linearly independent. We can then extend $Tv,v$ to a basis. This means we can assign what values $T$ should map elements of the basis to. We can then define $S(Tv)=0$ and define $S(v)=v$. Given this we can find that 
$$
\begin{align}
ST&=TS \\
STv&=TSv \\
0&=Tv
\end{align}
$$
This would imply $Tv=0$, however we know that $Tv$ is not a scalar multiple of $v$. Contradiction, $T$ must be a scalar multiple of the identity.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$