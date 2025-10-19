### Jason Low

####  3.1
##### (a)
$$
\begin{align}
[\hat{A},\hat{B}+\hat{C}]
=& \hat{A}(\hat{B}+\hat{C}) - (\hat{B}+\hat{C})\hat{A}  \\ =&\hat{A}\hat{B}+\hat{A}\hat{C}-\hat{B}\hat{A}-\hat{C}\hat{A}\\
=&\hat{A}\hat{B}-\hat{B}\hat{A}+\hat{A}\hat{C}-\hat{C}\hat{A} \\
=&[\hat{A},\hat{B}]+[\hat{A},\hat{C}]
\end{align}
$$
##### (b)
$$
\begin{align}
[\hat{A},\hat{B}\hat{C}]
&=\hat{A}\hat{B}\hat{C}-\hat{B}\hat{C}\hat{A} \\
&=\hat{A}\hat{B}\hat{C}-\hat{B}\hat{A}\hat{C}+\hat{B}\hat{A}\hat{C}-\hat{B}\hat{C}\hat{A} \\
&=(\hat{A}\hat{B}-\hat{B}\hat{A})\hat{C}+\hat{B}(\hat{A}\hat{C}-\hat{C}\hat{A}) \\
&=[\hat{A},\hat{B}]\hat{C}+\hat{B}[\hat{A},\hat{C}] \\
&=\hat{B}[\hat{A},\hat{C}]+[\hat{A},\hat{B}]\hat{C}
\end{align}
$$
##### (c)
$$
\begin{align}
[\hat{A}\hat{B},\hat{C}] 
&=\hat{A}\hat{B}\hat{C}-\hat{C}\hat{A}\hat{B} \\
&=\hat{A}\hat{B}\hat{C}-\hat{A}\hat{C}\hat{B}+\hat{A}\hat{C}\hat{B}-\hat{C}\hat{A}\hat{B} \\
&=\hat{A}(\hat{B}\hat{C}-\hat{C}\hat{B})+(\hat{A}\hat{C}-\hat{C}\hat{A})\hat{B} \\
&=\hat{A}[\hat{B},\hat{C}]+[\hat{A},\hat{C}]\hat{B}
\end{align}
$$
#### 3.2
$$
\begin{gather}
\hat{S}_{z}=\frac{\hbar}{2}\begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix} 
  
& \hat{S}_{x} = \frac{\hbar}{2} \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix} \

& \hat{S}_{y}=\frac{\hbar}{2} \begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix}
\end{gather}
$$
$$
\begin{align}
\hat{S_{n}}=& \hat{S} \cdot n \\
&=(\hat{S}_{x}i+\hat{S}_{y}j+\hat{S}_{z}k)\cdot(\sin \theta \cos \phi i+\sin \theta \sin \phi j+\cos \theta k) \\
&=\sin \theta \cos \phi \frac{\hbar}{2} \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix} +\sin \theta \sin \phi \begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix} +\cos \theta\begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix}  \\
&=\frac{\hbar}{2}\begin{pmatrix}
\cos \theta & \sin \theta \cos \phi-i\sin \theta \sin \phi \\
\sin \theta \cos \phi+i\sin \theta \sin \phi & -\cos \theta
\end{pmatrix} \\
&=\frac{\hbar}{2}\begin{pmatrix}
\cos \theta & \sin \theta(\cos \phi-i\sin \phi) \\
\sin \theta(\cos \phi+i\sin \phi) & -\cos \theta
\end{pmatrix} \\
&=\frac{\hbar}{2}\begin{pmatrix}
\cos \theta & \sin \theta(\cos \phi-i\sin \phi) \\
\sin \theta(\cos \phi+i\sin \phi) & -\cos \theta
\end{pmatrix}  \\
&=\frac{\hbar}{2}\begin{pmatrix}
\cos \theta & \sin \theta e^{-i\phi} \\
\sin \theta e^{i\phi} & -\cos \theta
\end{pmatrix}
\end{align}
$$
Now we find eigenvalues
$$
\begin{align}
0&=|\hat{S}_{n}-\lambda I| \\
&=\begin{vmatrix}
\cos \theta-\lambda & \sin \theta e^{-i\phi} \\
\sin \theta e^{i\phi} & -\cos \theta-\lambda
\end{vmatrix}  \\
&=(\cos \theta-\lambda)(-\cos \theta-\lambda)-(\sin \theta e^{-i\phi})(\sin \theta e^{i\phi}) \\
&=-\cos^2\theta+\lambda^2-\sin^2\theta \\
&=\lambda^2-1 \\
\lambda&=\pm 1
\end{align}
$$
Now find eigenstates
$$
\begin{gather}
\lambda_{+}=1 \\
\begin{pmatrix}
\cos \theta -1 & \sin \theta e^{-i\phi} \\
\sin \theta e^{i\phi} & -\cos \theta-1
\end{pmatrix} \begin{pmatrix}
\lambda_{1} \\
\lambda_{2}
\end{pmatrix} = \begin{pmatrix}
\lambda_{1} \\
\lambda_{2}
\end{pmatrix} \\
\lambda_{1}(\cos \theta-1)+\lambda_{2}\sin \theta e^{-i\phi}=\lambda_{1} \\
-2\sin^2{\frac{\theta}{2}}\lambda_{1}+2\sin{\frac{\theta}{2}}\cos{\frac{\theta}{2}}e^{-i\phi}\lambda_{2}=0 \\
-\sin{\frac{\theta}{2}}\lambda_{1}+\cos{\frac{\theta}{2}}e^{-i\phi}\lambda_{2}=0 \\
\lambda_{1}=\cos{\frac{\theta}{2}} \\
\lambda_{2}=\sin{\frac{\theta}{2}e^{i\phi}} \\
\ket{+n}= \lambda_{+}=\begin{pmatrix}
\cos{\frac{\theta}{2}} \\
\sin{\frac{\theta}{2}e^{i\phi}}
\end{pmatrix}
\end{gather}
$$
Because $|\braket{ +n | +n }|^2=(\lambda_{+}^T\lambda_{+})^2=|\cos^2\theta+\sin^2\theta|^2=1$ we know that $\lambda_{+}$ is properly normalized.
$\lambda_{-}$ is orthogonal to $\lambda_{+}$ so:
$$
\begin{align}
0&=\lambda_{-}\lambda_{+} \\
&=\begin{pmatrix}
\lambda_{1-} \\
\lambda_{2-}
\end{pmatrix}\cdot \begin{pmatrix}
\cos{\frac{\theta}{2}} \\
\sin{\frac{\theta}{2}e^{i\phi}}
\end{pmatrix} \\
&=\lambda_{1-}\cos \frac{\theta}{2}+\lambda_{2-}\sin{\frac{\theta}{2}e^{i\phi}} \\ 
\ket{-n}&=\lambda_{-}= \begin{pmatrix}
\sin{\frac{\theta}{2}} \\
-\cos{\frac{\theta}{2}e^{i\phi}}
\end{pmatrix}
\end{align}
$$
From these we get that:
$$
\begin{align}
\ket{+n}=\cos \frac{\theta}{2}\ket{+z}+e^{i\phi}\sin \frac{\theta}{2}\ket{-z} \\
\ket{+n}=\sin \frac{\theta}{2}\ket{+z}-e^{i\phi}\cos \frac{\theta}{2}\ket{-z} \\
\end{align}
$$

#### 3.8
$$

\begin{align} \\
[\hat{A},\hat{B}] &= i\hat{C} \\
\hat{A}\hat{B}-\hat{B}\hat{A}&=i\hat{C} \\
\bra{\varphi} \hat{A}\hat{B}\ket{\psi}  - \bra{\varphi} \hat{B}\hat{A}\ket{\psi}  &=i\bra{\varphi} \hat{C}\ket{\psi}   \\
\bra{\psi}\hat{A}\hat{B} \ket{\varphi}^*- \bra{\psi}\hat{B}\hat{A} \ket{\varphi}^* &=i\bra{\varphi} \hat{C}\ket{\psi} \\
\bra{\psi} \hat{A}\hat{B}-\hat{B}\hat{A}\ket{\varphi}^*&= i\bra{\varphi} \hat{C}\ket{\psi} \\
\bra{\psi} [\hat{A},\hat{B}]\ket{\varphi}^*&= i\bra{\varphi} \hat{C}\ket{\psi} \\
i\bra{\psi} \hat{C}\ket{\varphi}^*&= i\bra{\varphi} \hat{C}\ket{\psi} 
 \\
\bra{\psi} \hat{C}\ket{\varphi}^*&= \bra{\varphi} \hat{C}\ket{\psi} 
\end{align}
$$
Therefore $\hat{C}$ is hermitian.

#### 3.9
$$
\begin{gather}
\braket{ S_x } &= \bra{+z}S_{x}\ket{+z} = 0 &
\braket{ S_y } &= \bra{+z}S_{y}\ket{+z} = 0  &
\braket{ S_z } &= \bra{+z}S_{z}\ket{+z} = \frac{\hbar}{2}
\end{gather}
$$
$$
\begin{gather}
\Delta S_{x}=\sqrt{ \frac{\hbar^2}{4}- \braket{ S_x }}=\frac{\hbar}{2} &
\Delta S_{y}=\sqrt{ \frac{\hbar^2}{4}- \braket{ S_{}y }}=\frac{\hbar}{2}
\end{gather}

$$
$$
\Delta S_{x}\Delta S_{y}=\frac{\hbar^2}{4}\geq \frac{{\hbar \braket{  S_{z} } }}{2}=\frac{\hbar^2}{4}
$$
The relation is satisfied.
$$
\begin{gather}
\braket{ S_x } &= \bra{+x}S_{x}\ket{+x} = \frac{\hbar}{2} &
\braket{ S_y } &= \bra{+x}S_{y}\ket{+x} = 0  &
\braket{ S_z } &= \bra{+x}S_{z}\ket{+x} = 0
\end{gather}
$$
$$
\begin{gather}
\Delta S_{x}=\sqrt{ \frac{\hbar^2}{4}- \braket{ S_x }}=0 &
\Delta S_{y}=\sqrt{ \frac{\hbar^2}{4}- \braket{ S_{}y }}=\frac{\hbar}{2}
\end{gather}
$$
$$
\Delta S_{x}\Delta S_{y}=0\geq \frac{{\hbar \braket{  S_{z} } }}{2}=0
$$
The relation is satisfied.

#### 3.10
$$
\begin{align}
[\hat{S}_{x},\hat{S}_{y}]&=\hat{S}_{x}\hat{S}_{y}-\hat{S}_{y}\hat{S}_{x} \\
&=\frac{\hbar^2}{4} \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix} \begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix}-\frac{\hbar^2}{4} \begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix} \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix} \\
&=\frac{\hbar^2}{4}\begin{pmatrix}
i & 0 \\
0 & -i
\end{pmatrix}-\frac{\hbar^2}{4}\begin{pmatrix}
-i & 0 \\
0 & i
\end{pmatrix} \\
&=\frac{\hbar^2}{4}\begin{pmatrix}
2i & 0  \\
0 & 2i
\end{pmatrix} \\
&=\frac{\hbar^2}{4}2i\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} \\
&=\hbar i \cdot \frac{\hbar}{2}\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} \\
&=i\hbar \hat{S}_{z}
\end{align}
$$
