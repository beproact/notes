9### Jason Low
#### 3.6
$$
\hat{J}_{-}^{\dagger}=\hat{J}_{+}
$$
$$
\begin{align}
\bra{j,m} \hat{J}_{+}\hat{J}_{-}\ket{j,m} &=c^{*}c\braket{ j,m-1 | j,m-1 }   \\
\bra{j,m} \hat{J}^2-J_{z}^2+\hbar \hat{J}_{z}\ket{j,m}&= \\
\bra{j,m} (\hbar^2\lambda-\hbar^2m^2+\hbar^2 m \ket{j,m}&= \\
\bra{j,m} (\hbar^2(j(j+1)-m^2+ m)) \ket{j,m}&= \\
\hbar^2(j(j+1)-m(m-1))\bra{j,m}  \ket{j,m}&= \\
\hbar^2(j(j+1)-m(m-1))&=c^*c \\
\end{align}
$$
If we assume c is real then
$$
\begin{gather}
c=\hbar \sqrt{ j(j+1)-m(m-1) }\\
\hat{J}_{-}\ket{j,m}=\hbar \sqrt{ j(j+1)-m(m-1) }\ket{j,m-1}
\end{gather}
$$

#### 3.12
$$
\begin{align}
\hat{S}_{z}\ket{+z} = \frac{\hbar}{2}(\ket{+z}\bra{+z}-\ket{-z} \bra{-z})\ket{+z} = \frac{\hbar}{2}(\ket{+z}\braket{ +z | +z } -\ket{-z}\braket{ -z | +z }   ) =\frac{\hbar}{2}\ket{+z}  \\
\hat{S}_{z}\ket{-z} = \frac{\hbar}{2}(\ket{+z}\bra{+z}-\ket{-z} \bra{-z})\ket{-z} = \frac{\hbar}{2}(\ket{+z}\braket{ +z | -z } -\ket{-z}\braket{ -z | -z }   ) =\frac{\hbar}{2}\ket{-z} 
\end{align}
$$
This is what I would expect $\hat{S}_{z}$ to do.
$$
\begin{align}
\hat{S}_{+}\ket{-z}=\hbar \ket{+z}\braket{ -z |-z  }&=\hbar \ket{+z}    \\ 
\hat{S}_{+}\ket{+z}=\hbar \ket{+z}\braket{ -z |+z  }&=0     \\ \\
\hat{S}_{-}\ket{+z}=\hbar \ket{-z}\braket{ +z |+z  }&=\hbar \ket{-z} \\
\hat{S}_{-}\ket{-z}=\hbar \ket{-z}\braket{ +z |-z  }&=0      
\end{align}
$$
This is what I would expect $\hat{S}_{+}$ and $\hat{S}_{-}$ to do.

#### 3.13
$$
\begin{align}
[\hat{J}_{x},\hat{J}_{y}] &= \hat{J}_{x}\hat{J}_{y} -\hat{J}_{y}\hat{J}_{x} \\
&=\frac{\hbar^2}{2} \begin{pmatrix} 0 & 1 & 0\\ 1 & 0 & 1 \\0 & 1 & 0 \end{pmatrix}\begin{pmatrix} 0 & -i & 0\\ i & 0 & -i \\0 & i & 0 \end{pmatrix} -\frac{\hbar^2}{2}\begin{pmatrix} 0 & -i & 0\\ i & 0 & -i \\0 & i & 0 \end{pmatrix} \begin{pmatrix} 0 & 1 & 0\\ 1 & 0 & 1 \\0 & 1 & 0 \end{pmatrix} \\
&=\frac{\hbar^2}{2} \begin{pmatrix} i & 0 & -i \\ 0 & 0 & 0\\i & 0 & -i \end{pmatrix} -\frac{\hbar^2}{2}\begin{pmatrix}-i & 0 & -i\\0 & 0 & 0\\i & 0 & i \end{pmatrix} \\
&=\frac{\hbar^2}{2}\begin{pmatrix}2i & 0 & 0\\ 0 & 0 & 0\\0 & 0 & -2i\end{pmatrix} \\
&=\hbar i \cdot \hbar \begin{pmatrix}1 & 0 & 0\\0 & 0 & 0\\0 & 0 & -1\end{pmatrix} \\
&=i\hbar \hat{J}_{z}
\end{align}
$$
#### 3.14
We know eigenvalues of $\hat{S}_{z}$ are $\hbar$, $0$ and $-\hbar$. So in $S_{z}$ basis:
$$
\hat{S}_{z}\to\begin{pmatrix}\hbar & 0 & 0\\0 & 0 & 0\\0 & 0 & -\hbar\end{pmatrix}=\hbar\begin{pmatrix}
1 & 0 & 0\\0 & 0 & 0\\0 & 0 & -1
\end{pmatrix}
$$
$$
\hat{S}_{+}\to \begin{pmatrix}
\bra{1,1}S_{+}\ket{1,1}&\bra{1,1}S_{+}\ket{1,0} & \bra{1,1}S_{+}\ket{1,-1} \\
\bra{1,0}S_{+}\ket{1,1}&\bra{1,0}S_{+}\ket{1,0} & \bra{1,0}S_{+}\ket{1,-1} \\
\bra{1,-1}S_{+}\ket{1,1}&\bra{1,-1}S_{+}\ket{1,0} & \bra{1,-1}S_{+}\ket{1,-1}
\end{pmatrix}=\hbar \sqrt{ 2 }\begin{pmatrix}
0 & 1 & 0\\0 & 0 & 1\\0 & 0 & 0
\end{pmatrix}
$$
We know that $\hat{S}_{-}=\hat{S}_{+}^{\dagger}$ so
$$
\hat{S}_{-}\to \hbar \sqrt{ 2 }\begin{pmatrix}
0 & 0 & 0 \\1 & 0 & 0\\0 & 1 & 0
\end{pmatrix}
$$
$$
\begin{align}
\hat{S}_{y}=\frac{1}{2i}(S_{+}-S_{-})=\frac{\hbar \sqrt{ 2 }}{2i} \begin{pmatrix}
0 & 1 & 0 \\ -1 & 0 & 1 \\0 & -1 & 0 
\end{pmatrix} \\
\hat{S}_{x}=\frac{1}{2}(S_{+}+S_{-})=\frac{\hbar \sqrt{ 2 }}{2} \begin{pmatrix}
0 & 1 & 0 \\ 1 & 0 & 1 \\0 & 1 & 0 
\end{pmatrix}
\end{align}
$$
#### 3.15
$$
\hat{S}_{x}=\frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}0 & 1 & 0 \\ 1 &0 & 1\\0 & 1 & 0\end{pmatrix}
$$
We already know that the eigenvalues are $\hbar$, $0$ and $-\hbar$. This means the eigenvalues of $\sigma_{x}$ are $\pm\sqrt{ 2 }$  and 0.
For the eigenstate $\sqrt{ {2} }$
$$
\begin{align}
\begin{pmatrix}0-\sqrt{ 2 } & 1 & 0 \\ 1 &0-\sqrt{ 2 } & 1\\0 & 1 & 0-\sqrt{ 2 }\end{pmatrix} \begin{pmatrix}
x_{1} \\x_{2}\\x_{3}
\end{pmatrix}&=\begin{pmatrix}0\\0\\0\end{pmatrix} \\
\begin{pmatrix}-\sqrt{ 2 } & 1 & 0 \\ 1 &-\sqrt{ 2 } & 1\\0 & 1 & -\sqrt{ 2 }\end{pmatrix} \begin{pmatrix}
x_{1} \\x_{2}\\x_{3}
\end{pmatrix}&=\begin{pmatrix}0\\0\\0\end{pmatrix} \\ 
x_{1}-x_{2}\sqrt{ 2 }=0 \\
x_{1}=x_{2}\sqrt{ 2 } \\
x_{3}=x_{2}\sqrt{ 2 }
 \\ 

x_{1}=\frac{1}{{ 2 }} \\
x_{2}=\frac{1}{\sqrt{ {2} }} \\
x_{3}=\frac{1}{{ 2 }} \\
 \\

\frac{1}{2}\ket{1,1} +\frac{1}{\sqrt{ 2 }}\ket{1,0}+\frac{1}{2}\ket{1,-1}   
\end{align}
$$
For the eigenstate $0$

$$
\begin{align}
\begin{pmatrix}0-0 & 1 & 0 \\ 1 &0-0& 1\\0 & 1 & 0-0 \end{pmatrix} \begin{pmatrix}
x_{1} \\x_{2}\\x_{3}
\end{pmatrix}&=\begin{pmatrix}0\\0\\0\end{pmatrix} \\
\begin{pmatrix}0 & 1 & 0 \\ 1 &0 & 1\\0 & 1 & 0\end{pmatrix} \begin{pmatrix}
x_{1} \\x_{2}\\x_{3}
\end{pmatrix}&=\begin{pmatrix}0\\0\\0\end{pmatrix} \\ 
x_{2}=0
 \\
x_{1}=-x_{3} \\
x_{1}=\frac{1}{\sqrt{ 2 }} \\ \\
\frac{1}{\sqrt{ 2 }}\ket{1,1} -\frac{1}{\sqrt{ 2 }}\ket{1,-1} 
\end{align}
$$

For eigenstate $\sqrt{ 2 }$  
We know that the eigenstate is orthogonal to the other eigenstates and can get the final eigenstate 
$$
\frac{1}{2}\ket{1,1} -\frac{1}{\sqrt{ 2 }}\ket{1,0} +\frac{1}{2}\ket{1,-1} 
$$
#### 3.16
$$
\begin{gather}
\left( \frac{1}{\sqrt{ 2 }}\bra{1,1}-\frac{1}{\sqrt{ 2  }} \bra{1,-1}  \right)(\ket{1,1} )=\frac{1}{\sqrt{ 2 }}
\end{gather}
$$
We square this value to get the probability $\frac{1}{2}$

#### 3.17
##### a
$$
\begin{align} 
\bra{\psi}S_{z}\ket{\psi} &=\frac{1}{\sqrt{ 14 }}\hbar\frac{1}{\sqrt{ 14 }}\begin{pmatrix}1 & 2 & -3i\end{pmatrix}\begin{pmatrix}
1 & 0 & 0\\0 & 0 & 0\\0 & 0 & -1
\end{pmatrix}\begin{pmatrix}1 \\ 2 \\ 3i\end{pmatrix} \\
&=\frac{\hbar}{14}\begin{pmatrix}1 & 2 & -3i\end{pmatrix}\begin{pmatrix}1 \\ 0 \\ -3i\end{pmatrix} \\
&=\frac{\hbar}{14}(1-9) \\
&=-\frac{4\hbar}{7}
\end{align}
$$
##### b
$$
\begin{align} 
\bra{\psi}S_{x}\ket{\psi} &=\frac{1}{\sqrt{ 14 }}\frac{\hbar}{\sqrt{ 2 }}\frac{1}{\sqrt{ 14 }}\begin{pmatrix}1 & 2 & -3i\end{pmatrix}\begin{pmatrix}
0 & 1 & 0\\1 & 0 & 1\\0 & 1 & 0
\end{pmatrix}\begin{pmatrix}1 \\ 2 \\ 3i\end{pmatrix} \\
&=\frac{\hbar}{14\sqrt{ 2 }}\begin{pmatrix}1 & 2 & -3i\end{pmatrix}\begin{pmatrix}2 \\ 1+3i \\ 2\end{pmatrix} \\
&=\frac{\hbar}{14\sqrt{ 2 }}(2+2(1+3i)-6i) \\
&=\frac{\hbar}{14\sqrt{ 2 }}(2+2+6i-6i) \\
&=\frac{2\hbar}{7\sqrt{ 2 }}
\end{align}
$$
##### c
$$
\begin{gather} \\
\left|\frac{1}{\sqrt{ 14 }}\begin{pmatrix}
\frac{1}{2}& \frac{1}{\sqrt{ 2 }} & \frac{1}{2}
\end{pmatrix} \begin{pmatrix}1\\2\\3i\end{pmatrix}\right|^2 = \frac{1}{14}\left|   \frac{1}{2}+\frac{2}{\sqrt{ 2 }}+\frac{3i}{2}
\right|^2=\frac{1}{14\cdot4}|1+2\sqrt{ 2 }+3i|^2=\frac{9+2\sqrt{ 2 }}{28}
\end{gather}
$$

#### 3.25
##### a
$$
\begin{align}
\hat{S}_{+}\to\begin{pmatrix}
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}}   \\ 

\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}}  \\ 

\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}}  \\ 

\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}} 

\end{pmatrix}  \\

\end{align}
$$
$$
\begin{align}
\bra{\frac{3}{2},\frac{3}{2}}J_{+}\ket{\frac{3}{2},\frac{1}{2}}&= \hbar \sqrt{ \frac{3}{2}\left( \frac{3}{2}+1 \right)-\frac{1}{2}\left( \frac{1}{2}+1 \right) } \\
&=\hbar\sqrt{ 3 } \\
\bra{\frac{3}{2},\frac{1}{2}}J_{+}\ket{\frac{3}{2},-\frac{1}{2}}&= \hbar \sqrt{ \frac{3}{2}\left( \frac{3}{2}+1 \right)+\frac{1}{2}\left( -\frac{1}{2}+1 \right) } \\&=2\hbar \\
\bra{\frac{3}{2},-\frac{1}{2}}J_{+}\ket{\frac{3}{2},-\frac{3}{2}}&= \hbar \sqrt{ \frac{3}{2}\left( \frac{3}{2}+1 \right)-\frac{3}{2}\left( -\frac{3}{2}+1 \right) } \\ &=\hbar\sqrt{ 3 }
\end{align}
$$
$$
\begin{align}
\hat{S}_{+}\to\begin{pmatrix}
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}}   \\ 

\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}}  \\ 

\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{1}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}}  \\ 

\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{3}{2}} & 
\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{1}{2}} & 
\bra{\frac{3}{2},-\frac{3}{2}}S_{+}\ket{\frac{3}{2},-\frac{3}{2}} 

\end{pmatrix}&  \\
=\hbar\begin{pmatrix}
0 & \sqrt{ 3 } & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & \sqrt{ 3 } \\
0 & 0 & 0 & 0 
\end{pmatrix}
\end{align}
$$
$$
\hat{S}_{-}=\hat{S}_{+}^{\dagger}=\hbar\begin{pmatrix}
0 & \sqrt{ 3 } & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & \sqrt{ 3 } \\
0 & 0 & 0 & 0 
\end{pmatrix}^{\dagger}=\hbar\begin{pmatrix}
0 & 0 & 0 & 0 \\
\sqrt{ 3 } & 0 & 0 & 0 \\
0 & 2 & 0 & 0 \\
0 & 0 & \sqrt{ 3 } & 0 
\end{pmatrix}
$$
$$
\hat{S}_{y}=\frac{1}{2i}(S_{+}-S_{-})=\frac{\hbar}{2i}\begin{pmatrix}
0 & \sqrt{ 3 } & 0 & 0 \\
-\sqrt{ 3 } & 0 & 2 & 0 \\
0 & -2 & 0 & \sqrt{ 3 } \\
0 & 0 & -\sqrt{ 3 } & 0 
\end{pmatrix}
$$
##### b
The eigenvalue is $\frac{3}{2}\hbar$. For the $\sigma _y$ the eigenvalue is $3i$
$$
\begin{gather}
\begin{pmatrix}
-3i & \sqrt{ 3 } & 0 & 0\\ 
-\sqrt{ 3 } & -3i & 2 & 0 \\
0 & -2 & -3i & \sqrt{ 3 } \\
0 & 0 & -\sqrt{ 3 }&-3i
\end{pmatrix} \begin{pmatrix}
x_{1}\\x_{2} \\ x_{3}\\ x_{4}
\end{pmatrix}=\begin{pmatrix}
0\\0\\0\\0
\end{pmatrix} \\
-3i x_{1} + \sqrt{ 3 }x_2 = 0 \\
\sqrt{ 3 }x_{2}=3i x_{1} \\
x_{2}=\sqrt{ 3 }i x_{1} \\
 \\

-\sqrt{ 3 }x_{3}-3i x_{4}=0 \\
x_{3}=-\sqrt{ 3 } i x_{4} \\
\end{gather}
$$
$$
\begin{gather}
-\sqrt{ 3 }x_{1}-3ix_{2}+2x_{3}=0 \\
-\sqrt{ 3 }-3i^2\sqrt{ 3 }x_{1}=-2x_{3} \\
-\sqrt{ 3 }x_{1}+3\sqrt{ 3 }x_{1}=-2x_{3} \\
2\sqrt{ 3 }x_{1}=-2x_{3} \\
x_{3}=-\sqrt{ 3 }x_{1} \\
 \\
-\sqrt{ x_{3} }-3ix_{4}=0 \\
-3ix_{4}=\sqrt{ 3 }x_{3} \\
-\sqrt{ 3 }ix_{4}=x_{3} \\
-\sqrt{ 3 }ix_{4}=-\sqrt{ 3 }x_{1} \\
-ix_{4}=x_{1} \\
x_{4}=-ix_{1}
\end{gather}
$$
$$
x_{1}\begin{pmatrix}
1\\\sqrt{ 3 }i\\-\sqrt{ 3 }\\-i
\end{pmatrix} =\frac{1}{\sqrt{ 8 }}\begin{pmatrix}
1\\\sqrt{ 3 }i\\-\sqrt{ 3 }\\-i
\end{pmatrix}
$$
##### C
For $S_z=\frac{3}{2}\hbar$ the probability is $\left| \frac{1}{\sqrt{ 8 }} \right|^2=\frac{1}{8}$
For $S_z=\frac{1}{2}\hbar$ the probability is $\left| \frac{\sqrt{ 3 }i}{\sqrt{ 8 }} \right|^2=\frac{3}{8}$
For $S_z=-\frac{1}{2}\hbar$ the probability is $\left| \frac{-\sqrt{ 3 }}{\sqrt{ 8 }} \right|^2=\frac{3}{8}$
For $S_z=-\frac{3}{2}\hbar$ the probability is $\left| \frac{-i}{\sqrt{ 8 }} \right|^2=\frac{1}{8}$
