	oq2wwq25##### 1
$\frac{1}{\sqrt{ 2 }}+\frac{i}{\sqrt{ 2 }}$
$-\frac{1}{\sqrt{ 2 }}-\frac{i}{\sqrt{ 2 }}$
##### 2
Proof: Let $v\in V$. We know that $-(-v)$ is the additive inverse of $-v$.  This means $-v+(-(-v))=0$. We can add $v$ on both sides of this equation to get:$$v+(-v)+(-(-v))=0 +v$$Since $-v$ is the additive inverse of $v$ we know that $v+(-v)=0$. Thus
$$
\begin{align}
v+(-v)+(-(-v))&=0+v \\
0+(-(-v)) & =0+v \\
-(-v)&=v
\end{align}
$$
This shows that $-(-v)=v$. 
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

##### 3
Proof:
Let $v\in V$. We know there are addition and scalar multiplication. We want to show that $0v=0$ if and only if every vector has a additive inverse. 

First, we show that $0v=0$ implies every vector has a additive inverse.  We know that $0=1+(-1)$. Using that, we can get that $(1+(-1))v=0$. We can use the distributive law to get $1v+(-1)v=0$. We can use the fact that 1 is the multiplicative inverse to get $v+(-1)v=0$. Since our vector space is closed under scalar multiplication we know that $(-1)v$ is in our vector space. Since $v+(-1)v=0$ that means for every $v$ there is a vector where adding it to $v$ results in $0$. This means every vector has an additive inverse.

Now, we show that every vector having an additive inverse implies that $0v=0$. 
We know that $0v=(0+0)v$. We can then distribute to find the $0v=0v+0v$. We can then add the additive inverse of $0v$ to both sides to get that $0=0v$. This shows that $0=0v$

Since we have shown that $0v=0$ implies that every vector has an additive inverse and that every vector having an additive inverse implies that $0v=0$ we have shown that $0v=0$ is true if and only if every vector has an additive inverse. 
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$


##### 4
Proof:
To show that the set of differentiable real-valued functions on $\mathbb{R}$ is a subspace of $\mathbb{R}^{\mathbb{R}}$. We must show that the set of differentiable real-valued functions on $\mathbb{R}$ has the additive identity, is closed under addition and is closed under scalar multiplication.

We know that the $0$ function is differentiable since its derivative is itself. This means the set contains the additive identity.

Since two differentiable functions added together are differentiable, we know that the set is closed under addition.

Since a differentiable function multiplied by a scalar is differentiable we know that the set is closed under scalar multiplication.

Since the set of differentiable real-valued functions on $\mathbb{R}$ contains the additive identity, is closed under addition and closed under multiplication, we know that it is a subspace of $\mathbb{R}^\mathbb{R}$.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

##### 5
Proof:
To show that $V_{1}\cap V_{2}$ is a subspace of $V$ we need to show that $V_{1}\cap V_{2}$ contains the additive identity, is closed under addition and closed under scalar multiplication.

Because both $V_{1}$ and $V_{2}$ are subspaces of V, we know they contain the additive inverse. Since both contain the additive inverse, their intersection contains the additive inverse.

Let $u,v\in V_{1}\cap V_{2}$.
Since $V_{1}$ is a subspace, it is closed under addition. Since every element in $V_{1}\cap V_{2}$ is in $V_{1}$ adding $u+v$ will always result in a vector that is in $V_{1}$. We can use similar logic to show that $u+v\in V_{2}$. Since $u+v$ is in $V_{1}$ and $V_{2}$, $u+v\in V_{1}\cap V_{2}$. This shows that $V_{1}\cap V_{2}$ is closed under addition.

Let $v\in V_{1}\cap V_{2}$. Let $\lambda \in \mathbb{F}$
Since $V_{1}$ is a subspace, it is closed under scalar multiplication. Since every element in $V_{1}\cap V_{2}$ is in $V_{1}$, we know that $\lambda v\in V_{1}$. We can use similar logic to show $\lambda v\in V_{2}$. Since $\lambda v$ is in $V_{1}$ and $V_{2}$ we know that $\lambda v\in V_{1}\cap V_{2}$. This shows that $V_{1}\cap V_{2}$ is closed under scalar multiplication.
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\square$

##### 6
Counterexample:
$U=\{(0,y)\in \mathbb{F}^2:y\in \mathbb{F}\}$
$V_{1}=\{(x,0)\in \mathbb{F}^2:x\in \mathbb{F}\}$
$V_{2}=\{(z,z)\in \mathbb{F}^2:z\in \mathbb{F}\}$
