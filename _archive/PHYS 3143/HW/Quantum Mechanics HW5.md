### Jason Low
#### 4.4
$$
\begin{gather}
\ket{+z=\frac{1}{\sqrt{ 2 }}\ket{+x} +\frac{1}{\sqrt{ 2 }}+\ket{-x} } \\
\hat{H}=w_{0}S_{x} \\
\hat{U}(t)=e^{-i\hat{H}t/\hbar} \\
\end{gather}
$$
$$
\begin{align}
\hat{U}(t)\ket{+z} &=\frac{1}{\sqrt{ 2 }}e^{-i\hat{H}t/\hbar}\ket{+x}+ \frac{1}{\sqrt{ 2 }}e^{-i\hat{H}t/\hbar}\ket{-x} \\ 
&=\frac{1}{\sqrt{ 2 }}e^{-iw_{0}t/2}\ket{+x} +\frac{1}{\sqrt{ 2 }}e^{iw_{0}t/2}\ket{-x} \\
&=\frac{1}{\sqrt{ 2 }}\ket{+x}+\frac{1}{\sqrt{ 2 }}e^{iw_{0}t}\ket{+x}    \\
&=\frac{1}{2}\ket{+z} +\frac{1}{2}\ket{-z} +\frac{e^{i\omega_{0}}}{2}\ket{+z}+ \frac{e^{i\omega_{0}}}{2}\ket{-z} \\
&=\frac{{1+e^{i\omega_{0}}}}{2}\ket{+z}+  \frac{{1-e^{i\omega_{0}}}}{2}\ket{-z} \\
 
\end{align}
$$
$$
\begin{gather}
|\bra{-z}\hat{U}\ket{+z}|^2=\left| \frac{1-e^{iw_{0}t}}{2} \right|^2=\frac{1}{4} \left({1-e^{iw_{0}t}}\right) \left({1-e^{-iw_{0}t}}\right) = \\
\frac{1}{2}-\frac{1}{2}\left( \frac{{e^{iw_{0}t}+e^{-iw_{0}t}}}{2} \right)=\frac{1}{2}-\frac{1}{2}\cos(w_{0}t)= \frac{1}{4
} \\
\cos(\omega_{0}t)=\frac{1}{2} \\
w_{0}t=\frac{\pi}{3} \\
t=\frac{\pi}{3\omega_{0}}

\end{gather}

$$

We ignore larger solutions because we want the least possible $t$ for the least possible $l_{0}$.
$$
\begin{align}
l_{0}=v_{0}t \\
l_{0}=\frac{v_{0}\pi}{3\omega_{0}}
\end{align}
$$
#### 4.5
$$
\begin{gather}
B=B_{0}(\sin \theta \hat{i}+\cos \theta \hat{z}) \\ 

\hat{H}=\omega_{0}S_{n}
\end{gather}
$$

Eigenvectors: $\ket{+n} \to\begin{pmatrix}\cos \frac{\theta}{2} \\ \sin \frac{\theta}{2}\end{pmatrix}$ and $\ket{-n} \to\begin{pmatrix}\sin \frac{\theta}{2} \\ -\cos \frac{\theta}{2}\end{pmatrix}$
$$
\begin{gather}
\ket{+z}= C_{1}\ket{+n}+C_{2}\ket{-n} \\
\begin{pmatrix}
1\\0
\end{pmatrix}=C_{1}\begin{pmatrix}\cos \frac{\theta}{2} \\ \sin \frac{\theta}{2}\end{pmatrix}+C_{2}\begin{pmatrix}\sin \frac{\theta}{2} \\ -\cos \frac{\theta}{2}\end{pmatrix} \\
C_{1}=\cos \frac{\theta}{2} \\
C_{2}=\sin \frac{\theta}{2} \\
\ket{+z} =\cos \frac{\theta}{2}\ket{+n}+\sin \frac{\theta}{2}\ket{-n}  
\end{gather}
$$
$$
\hat{U}\ket{+z} = e^{-i\omega_{0}S_{n}T/\hbar}\left( \cos \frac{\theta}{2}\ket{+n}+\sin \frac{\theta}{2}\ket{-n} \right)=e^{-i\omega_{0}T/2}\cos \frac{\theta}{2}\ket{+n}+ e^{iw_{0}T/2}\sin \frac{\theta}{2}\ket{-n} 
$$
Remove global phase
$$
\hat{U}\ket{+z}=\cos \frac{\theta}{2}\ket{+n}+e^{2iw_{0}T }\sin \frac{\theta}{2 } \ket{-n}  
$$
$$
\begin{gather}
\braket{ +y | +n }=\frac{1}{\sqrt{ 2 }}\cos \frac{\theta}{2}+\frac{-i}{\sqrt{ 2 }}\sin \frac{\theta}{2} \\
\braket{ +y | -n }=\frac{1}{\sqrt{ 2 }}\sin \frac{\theta}{2}+\frac{i}{\sqrt{ 2 }}\cos \frac{\theta}{2} 
\end{gather}
$$
$$
\begin{gather}
\bra{+y} \hat{U}\ket{+z}=\cos \frac{\theta}{2} \left( \frac{1}{\sqrt{ 2 }}\cos \frac{\theta}{2}+\frac{-i}{\sqrt{ 2 }}\sin \frac{\theta}{2} \right) + e^{iw_{0}T }\sin \frac{\theta}{2 }\left( \frac{1}{\sqrt{ 2 }}\sin \frac{\theta}{2}+\frac{i}{\sqrt{ 2 }}\cos \frac{\theta}{2}  \right) \\
=\frac{1}{\sqrt{ 2 }}\left( \cos^2\frac{\theta}{2} -\frac{i}{2}\sin \theta +e^{i\omega_{0}T}\sin^2 \frac{\theta}{2}+e^{i\omega_{0}T}\frac{i}{2}\sin \theta\right)
\end{gather}
$$
$$
\begin{gather}
|\bra{+y} \hat{U}\ket{+z}|^2=\frac{1}{2}|\cos^2\frac{\theta}{2} -\frac{i}{2}\sin \theta +e^{i\omega_{0}T}\sin^2 \frac{\theta}{2}+e^{i\omega_{0}T}\frac{i}{2}\sin \theta|^2= \\
\frac{1}{2}(1-\sin \omega_{0}T\sin \theta)
\end{gather}
$$



For $\theta=0$ Probability is $\frac{1}{2}$. This makes sense, as if B points in the same direction as Z the only thing that changes is global phase.
For $\theta=\frac{\pi}{2}$ Probability is $\frac{1}{2}(1-\sin \omega_{0}T)$

#### 4.8
$$
\begin{gather}
\ket{+n}=\cos \frac{\theta}{2}\ket{+z}+\sin \frac{\theta}{2}\ket{-z} \\
\hat{H}=\omega_{0}S_z \\
\hat{U}(t)=e^{-i\hat{H}t/\hbar} \\
\hat{U}(t)\ket{+n}=\cos \frac{\theta}{2}e^{-i\hat{H}t/\hbar}\ket{+z}+\sin \frac{\theta}{2}e^{-i\hat{H}t/\hbar}\ket{-z}= \\
e^{-i\omega_{0}t/2}\cos  \frac{\theta}{2}\ket{+z}+e^{i\omega_{0}t/2}\sin \frac{\theta}{2}\ket{-z}= \\
\cos \frac{\theta}{2}\ket{+z} +e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{-z}= \ket{\psi(t)} \\
\bra{\psi(t)} =\bra{+n} \hat{U}(t)=\cos \frac{\theta}{2}\bra{+z}+  e^{-i\omega_{0}t}\sin \frac{\theta}{2} \bra{-z}  \\ 
\end{gather}
$$
$$
\begin{gather}
S_{z}\ket{\psi(t)}=  S_{z}\left( \cos \frac{\theta}{2}\ket{+z} +e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{-z} \right)=\frac{\hbar}{2}\left( \cos \frac{\theta}{2}\ket{+z} -e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{-z}  \right) \\
\bra{\psi(t)} S_{z}\ket{\psi(t)}=\left( \cos \frac{\theta}{2}\bra{+z}+  e^{-i\omega_{0}t}\sin \frac{\theta}{2} \bra{-z}  \right)\frac{\hbar}{2}\left( \cos \frac{\theta}{2}\ket{+z} -e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{-z}  \right)= \\
\frac{\hbar}{2}\left( \cos^2\frac{\theta}{2}-\sin^2\frac{\theta}{2} \right)=\frac{\hbar}{2}\cos(\theta)
\end{gather}
$$

$$
\begin{gather}
S_{x}\ket{\psi(t)}=  S_{x}\left( \cos \frac{\theta}{2}\ket{+z} +e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{-z} \right)=\frac{\hbar}{2}\left( \cos \frac{\theta}{2}\ket{-z} +e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{+z}  \right) \\
\bra{\psi(t)} S_{x}\ket{\psi(t)}=\left( \cos \frac{\theta}{2}\bra{+z}+  e^{-i\omega_{0}t}\sin \frac{\theta}{2} \bra{-z}  \right)\frac{\hbar}{2}\left( \cos \frac{\theta}{2}\ket{-z} +e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{+z}  \right)= \\
\frac{\hbar}{2}\left( e^{-i\omega_{0}t}\sin \frac{\theta}{2} \cos \frac{\theta}{2}  +  e^{i\omega_{0}t}\sin \frac{\theta}{2} \cos \frac{\theta}{2} \right)=\frac{\hbar}{2}\sin \frac{\theta}{2}\cos \frac{\theta}{2}(e^{i\omega_{0}t}+e^{-i\omega_{0}t})= \\
\frac{\hbar}{2}\sin \frac{\theta}{2}\cos \frac{\theta}{2}\cos \omega_{0}t = \frac{\hbar}{2}\sin \theta \cos \omega_{0}t
\end{gather}
$$

$$
\begin{gather}
S_{y}\ket{\psi(t)}=  S_{y}\left( \cos \frac{\theta}{2}\ket{+z} +e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{-z} \right)=\frac{\hbar}{2}\left( i\cos \frac{\theta}{2}\ket{-z} -ie^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{+z}  \right) \\
\bra{\psi(t)} S_{y}\ket{\psi(t)}=\left( \cos \frac{\theta}{2}\bra{+z}+  e^{-i\omega_{0}t}\sin \frac{\theta}{2} \bra{-z}  \right)\frac{\hbar}{2}\left( i\cos \frac{\theta}{2}\ket{-z} -ie^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{+z}  \right)= \\
\left( \cos \frac{\theta}{2}\bra{+z}+  e^{-i\omega_{0}t}\sin \frac{\theta}{2} \bra{-z}  \right)\frac{i\hbar}{2}\left( \cos \frac{\theta}{2}\ket{-z} -e^{i\omega_{0}t}\sin \frac{\theta}{2}\ket{+z}  \right)=  \\
\frac{i\hbar}{2}\left( e^{-iw_{0}t}\sin \frac{\theta}{2}\cos \frac{\theta}{2}-e^{i\omega_{0}t}\sin \frac{\theta}{2}\cos \frac{\theta}{2} \right)= \\
\frac{i\hbar}{2}\left( e^{-iw_{0}t}-e^{i\omega_{0}t} \right)\sin \frac{\theta}{2}\cos \frac{\theta}{2}= \\
\frac{i\hbar}{2}(-2i\sin \omega_{0}t)\sin \frac{\theta}{2}\cos \frac{\theta}{2}=\frac{\hbar}{2}\sin(w_{0}t)\sin(\theta)
\end{gather}
$$
#### 4.11
$$
\begin{gather}
\hat{H}=\omega_{0}\hat{S}_{z} \\  
\hat{U}(t)=e^{-i\omega_{0}\hat{S}_{z}t/\hbar}\\

\ket{1,1}_{y}=\frac{1}{2}\ket{1,1}+\frac{i\sqrt{ 2 }}{2}\ket{1,0}-\frac{1}{2}\ket{1,-1} \\
\hat{U}(t)\ket{1,1}_{y}=\frac{1}{2}e^{-i\omega_{0}\hat{S}_{z}t/\hbar}\ket{1,1}+\frac{i\sqrt{ 2 }}{2}e^{-i\omega_{0}\hat{S}_{z}t/\hbar}\ket{1,0}-\frac{1}{2}e^{-i\omega_{0}\hat{S}_{z}t/\hbar}\ket{1,-1}= \\
\frac{1}{2}e^{-i\omega_{0}t}\ket{1,1}+i\frac{\sqrt{ 2 }}{2}\ket{1,0}-\frac{1}{2}e^{i\omega_{0}t}\ket{1,-1}=\ket{\psi(t)}  \\
\bra{\psi(t)}=\frac{1}{2}e^{i\omega_{0}t}\bra{1,1}-\frac{i\sqrt{ 2 }}{2}\bra{1,0}-\frac{1}{2}e^{-i\omega_{0}t}\bra{1,-1}    
\end{gather}
$$
$$
\begin{gather}
S_{z}\ket{\psi(t)}= \hbar\left( \frac{1}{2}e^{-i\omega_{0}t}\ket{1,1}+\frac{1}{2}e^{i\omega_{0}t}\ket{1,-1} \right)   \\
\braket{  S_{z} }= \bra{\psi(t)} S_{z}\ket{\psi(t)}=  \\
\left( \frac{1}{2}e^{i\omega_{0}t}\bra{1,1}-\frac{i\sqrt{ 2 }}{2}\bra{1,0}-\frac{1}{2}e^{-i\omega_{0}t}\bra{1,-1} \right)\hbar\left( \frac{1}{2}e^{-i\omega_{0}t}\ket{1,1}+\frac{1}{2}e^{i\omega_{0}t}\ket{1,-1}  \right)     = \\
\frac{1}{4}-\frac{1}{4}=0
\end{gather}
$$
$$
\begin{gather}
S_{x}\to \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
0 & 1 & 0\\1 & 0 & 1\\0 & 1 & 0
\end{pmatrix} \\
S_{x}\ket{\psi(t)}= \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
0 & 1 & 0\\1 & 0 & 1\\0 & 1 & 0
\end{pmatrix}\begin{pmatrix}
\frac{1}{2}e^{-i\omega_{0}t}\\ \frac{i\sqrt{ 2 }}{2}\\-\frac{1}{2}e^{i\omega_{0}t}
\end{pmatrix}=\frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
\frac{i\sqrt{ 2 }}{2} \\
\frac{1}{2}e^{-i\omega_{0}t}-\frac{1}{2}e^{i\omega_{0}t} \\
\frac{i\sqrt{ 2 }}{2}
\end{pmatrix}  \\
=\frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
\frac{i\sqrt{ 2 }}{2} \\
-i\sin(\omega_{0}t) \\
\frac{i\sqrt{ 2 }}{2}
\end{pmatrix} \\
\bra{\psi(t)}S_{x}\ket{\psi(t)} =\begin{pmatrix}
\frac{1}{2}e^{i\omega_{0}t} & -\frac{i\sqrt{ 2 }}{2} & \frac{1}{2}e^{-i\omega_{0}t}
\end{pmatrix} \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
\frac{i\sqrt{ 2 }}{2} \\
-i\sin(\omega_{0}t) \\
\frac{i\sqrt{ 2 }}{2}
\end{pmatrix}= \\
\hbar\left( \frac{1}{4}e^{i\omega_{0}t}+\frac{-\sin \omega_{0}t}{2}+\frac{1}{4}e^{-i\omega_{0}t} \right)=\hbar\left( \frac{-\sin(\omega_{0}t)}{2} +\frac{-\sin(\omega_{0}t)}{2} \right)=\hbar(-\sin(\omega_{0}t))=-\hbar \sin(\omega_{0}t)
\end{gather}
$$

$$
\begin{gather}
S_{y}\to \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
0 & 1 & 0\\1 & 0 & 1\\0 & 1 & 0
\end{pmatrix} \\
S_{y}\ket{\psi(t)}= \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
0 & -i & 0\\i & 0 & -i\\0 & i & 0
\end{pmatrix}\begin{pmatrix}
\frac{1}{2}e^{-i\omega_{0}t}\\ \frac{i\sqrt{ 2 }}{2}\\-\frac{1}{2}e^{i\omega_{0}t}
\end{pmatrix}=\frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
\frac{1}{\sqrt{ 2 }}\\ \frac{i}{2}e^{-i\omega_{0}t}+\frac{i}{2 }e^{i\omega_{0}t} \\
-\frac{1}{\sqrt{ 2 }}
\end{pmatrix}= \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
\frac{1}{\sqrt{ 2 }}\\ i\cos \omega_{0}t \\
-\frac{1}{\sqrt{ 2 }}
\end{pmatrix}\\
\bra{\psi(t)}S_{x}\ket{\psi(t)} =\begin{pmatrix}
\frac{1}{2}e^{i\omega_{0}t} & -\frac{i\sqrt{ 2 }}{2} & \frac{1}{2}e^{-i\omega_{0}t}
\end{pmatrix} \frac{\hbar}{\sqrt{ 2 }}\begin{pmatrix}
\frac{1}{\sqrt{ 2 }}\\ i\cos \omega_{0}t \\
-\frac{1}{\sqrt{ 2 }}
\end{pmatrix}  \\
=\hbar\left( \frac{1}{4}e^{-i\omega_{0}t}+ \frac{\cos \omega_{0}t}{2}+\frac{1}{4}e^{-i\omega_{0}t}\right)=\hbar \cos \omega_{0} t
\end{gather}
$$
#### 4.12
$$
\begin{gather}
\hat{H} = \omega_{0}\hat{S}_{x} \\
\hat{U}(t)=e^{-i\omega_{0}\hat{S}_{x}t/\hbar} \\
\ket{1,1}= \frac{1}{2}\ket{1,1}_{x} +\frac{1}{\sqrt{ 2 }}\ket{1,0}_{x}+\frac{1}{2}\ket{1,-1}_{x}  \\ 
\bra{1,-1}=\frac{1}{2}\ket{1,1} -\frac{1}{\sqrt{ 2 }}\ket{1,0} +\frac{1}{2}\ket{1,-1}  \\
\hat{U}(t)\ket{1,1}=\frac{1}{2}e^{-i\omega_{0}t}\ket{1,1}+\frac{1}{\sqrt{ 2 }}\ket{1,0}  +\frac{1}{2}e^{i\omega_{0}t}\ket{1,-1}     \\
\bra{1,-1}\hat{U}(t)\ket{1,1}=\left( \frac{1}{2}\bra{1,1} -\frac{1}{\sqrt{ 2 }}\bra{1,0} +\frac{1}{2}\bra{1,-1}   \right)\left( \frac{1}{2}e^{-i\omega_{0}t}\ket{1,1}+\frac{1}{\sqrt{ 2 }}\ket{1,0}  +\frac{1}{2}e^{i\omega_{0}t}\ket{1,-1} \right) \\
=\frac{1}{4}e^{-i\omega_{0}t}+\frac{1}{4}e^{i\omega_{0}t}-\frac{1}{2}=\frac{1}{2}\cos(\omega_{0}t)-\frac{1}{2}=\frac{1}{2}(\cos(\omega_{0}t)-1) \\
|\bra{1,-1}\hat{U}(t)\ket{1,1}|^2=\frac{1}{4}(\cos(\omega_{0}t)-1)^2
\end{gather}
$$
#### 4.13
##### a
$$
\begin{gather}
\ket{\psi(t)}=\hat{U}(t)\ket{2}=e^{-i\omega_{0}\hat{H}/\hbar}\ket{2}=e^{-i\omega_{0}2/\hbar}\ket{2}   
\end{gather}
$$
##### b
$$
\begin{gather}
\ket{\psi(t)}= \hat{U}(t)\ket{3}=e^{-i\omega_{0}\hat{H}/\hbar}\ket{3}=e^{-i\omega_{0}3/\hbar}\ket{3}   
\end{gather}
$$