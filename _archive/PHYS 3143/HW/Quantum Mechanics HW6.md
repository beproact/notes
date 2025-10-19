## Jason Low

#### 6.1
##### a
$$
[\hat{A}\hat{B},\hat{C}]=\hat{A}[\hat{B},\hat{C}]+[\hat{A},\hat{C}]\hat{B}
$$
###### Base Case
We already know that $[\hat{x},\hat{p}_{x}]=i\hbar$
So for the case where $n=1$ we get that
$$
\begin{align}
[\hat{x},\hat{p}_{x}]&=i\hbar \\
[\hat{x}^1,\hat{p}_{x}]&=i\hbar(1)x^{(1-1)}
\end{align}
$$
So we know that the $[\hat{x}^n,\hat{p}_{x}]=i\hbar n\hat{x}^{n-1}$ is true for $n=1$
###### Induction Step
Assume $[\hat{x}^k,\hat{p}_{x}]=i\hbar k\hat{x}^{k-1}$ is true for any $k\geq1$. 
$$
\begin{align}
[\hat{x}^{k+1},\hat{p}_{x}]&= \\
[\hat{x}^{k}\hat{x},\hat{p}_{x}]&= \\
\hat{x}^k[\hat{x},\hat{p}_{x}]+[\hat{x}^k,\hat{p}_{x}]\hat{x}&= \\
\hat{x}^k(i\hbar)+(i\hbar k\hat{x}^{k-1})\hat{x}&= \\
i\hbar \hat{x}^k+i\hbar k\hat{x}^k&= \\
i\hbar \hat{x}^k(1+k)&= i\hbar(k+1)\hat{x}^{(k+1)-1}
\end{align}
$$
We have shown that $[\hat{x}^k,\hat{p}_{x}]=i\hbar k\hat{x}^{k-1}$ implies $[\hat{x}^(k+1),\hat{p}_{x}]=i\hbar (k+1)\hat{x}^{(k+1)-1}$. This means that for all $n$ we know that $[\hat{x}^n,\hat{p}_{x}]=i\hbar n\hat{x}^{n-1}$.
##### b
$$
F(\hat{x})=F(0)+\frac{dF}{dx}_{x=0}x+\frac{1}{2}\frac{d^2F}{dx^2}x^2+\dots+\frac{1}{n!}  \frac{d^nF}{dx^n}x^n\dots
$$
$$
\begin{gather}
[F(\hat{x}),\hat{p}_{x}]=F(\hat{x})\hat{p}_{x}-\hat{p}_{x}F(\hat{x}) \\
= \left( F(0)+\frac{dF}{dx}_{x=0}x+\frac{1}{2}\frac{d^2F}{dx^2}x^2+\dots+\frac{1}{n!}  \frac{d^nF}{dx^n}x^n\dots \right)\hat{p}_{x}- \\
\hat{p}_{x}\left( F(0)+\frac{dF}{dx}_{x=0}x+\frac{1}{2}\frac{d^2F}{dx^2}x^2+\dots+\frac{1}{n!}  \frac{d^nF}{dx^n}x^n\dots \right) \\
=F(0)\hat{p}_{x}-\hat{p}_{x}F(0) + \frac{dF}{dx}_{x=0}x\hat{p}_{x} -\hat{p}_{x}\frac{dF}{dx}_{x=0}x+ \frac{d^2F}{dx^2}_{x=0}\frac{1}{2!}x^2\hat{p}_{x} -\hat{p}_{x}\frac{d^2F}{dx^2}_{x=0}\frac{1}{2!}x^2\dots \\
=\frac{dF}{dx}_{x=0}x\hat{p}_{x} -\hat{p}_{x}\frac{dF}{dx}_{x=0}x+ \frac{d^2F}{dx^2}_{x=0}x^2\hat{p}_{x} -\hat{p}_{x}\frac{d^2F}{dx^2}_{x=0}x^2\dots \\
=\frac{dF}{dx}_{x=0}(x\hat{p}_{x}-\hat{p}_{x}x)+\frac{d^2F}{dx^2}_{x=0}\frac{1}{2!}(x^2\hat{p}_{x}-\hat{p}_{x}x^2)+\frac{d^3F}{dx^3}_{x=0}\frac{1}{3!}(x^3\hat{p}_{x}-\hat{p}_{x}x^3)+\dots \\
=\frac{dF}{dx}_{x=0}[\hat{x},\hat{p}_{x}]+\frac{d^2F}{dx^2}_{x=0}\frac{1}{2!}[\hat{x}^2,\hat{p}_{x}]+\frac{d^3F}{dx^3}_{x=0}\frac{1}{3!}[\hat{x}^3,\hat{p}_{x}]+\dots \\
=\frac{dF}{dx}_{x=0}i\hbar+\frac{d^2F}{dx^2}_{x=0}\frac{1}{2!}i\hbar2\hat{x}^1+\frac{d^3F}{dx^3}_{x=0}\frac{1}{3!}i\hbar3\hat{x}^2+\dots \\
=\frac{dF}{dx}_{x=0}i\hbar+\frac{d^2F}{dx^2}_{x=0}\frac{1}{1!}i\hbar \hat{x}+\frac{d^3F}{dx^3}_{x=0}\frac{1}{2!}i\hbar \hat{x}^2+\dots \\
=i\hbar\left(\frac{dF}{dx}_{x=0}+\frac{d^2F}{dx^2}_{x=0} \hat{x}+\frac{d^3F}{dx^3}_{x=0}\frac{1}{2!} \hat{x}^2+\dots\right) \\
=i\hbar \frac{dF}{dx} \hat{x}
\end{gather}
$$

##### c
$$
\begin{gather}
[\hat{H},p_{x}]=\left[ \frac{\hat{p}_{x}^2}{2m} + V(\hat{x}),\hat{p}_{x} \right]=\left[ \frac{\hat{p}_{x}^2}{2m} ,\hat{p}_{x} \right]+[V(\hat{x}),\hat{p}_{x}]=[V(\hat{x}),\hat{p}_{x}]=i\hbar \frac{dV}{dx}\hat{x} \\
\end{gather}
$$
$$
\begin{gather}
\frac{d\braket{  p_{x} } }{dt}=\frac{i}{\hbar}\bra{\psi} [\hat{H},\hat{p}_{x}] \ket{\psi}=\frac{i}{\hbar}i\hbar \bra{\psi} \frac{dV}{dx}\hat{x}\ket{\psi}=\braket{ -\frac{dV}{dx}   }     
\end{gather}
$$
#### 6.3

$$
\ket{\psi}\to \ket{\psi'}=\hat{T}(\delta x)\ket{\psi}
$$
$[\hat{x},\hat{T}(\delta x)]=\delta x$
$$
\begin{gather}
\braket{  x }'=\int_{-\infty}^\infty \bra{\psi} \hat{T}^*(\delta x) x\hat{T}(\delta x)\ket{\psi}dx=\int_{-\infty}^\infty \bra{\psi} \hat{T}^*(\delta x) \hat{T}(\delta x)x+\delta x\ket{\psi}dx \\
\int_{-\infty}^\infty\bra{\psi}x+  \delta x\ket{\psi} dx=
\int_{-\infty}^\infty\bra{\psi}x\ket{\psi}dx+\int_{-\infty}^\infty\bra{\psi}\delta x\ket{\psi}dx \\
=\braket{  x }+ \delta x
\end{gather}
$$

$[p_{x},\hat{T}(x)]=0$ 
$$
\begin{gather}
\braket{  p_{x} }'=\int_{-\infty}^\infty \bra{\psi} \hat{T}^*(\delta x) p_{x}\hat{T}(\delta x)\ket{\psi}dx=\int_{-\infty}^\infty \bra{\psi} \hat{T}^*(\delta x) \hat{T}(\delta x)p_{x}\ket{\psi}dx=\int_{-\infty}^\infty \bra{\psi} p_{x}\ket{\psi}dx \\
=\braket{  p_{x} } 
\end{gather}
$$
