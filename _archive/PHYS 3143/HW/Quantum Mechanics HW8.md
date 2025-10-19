##### 6.12
$$
\begin{gather}
\psi(p)=\frac{1}{\sqrt{ 2\pi \hbar }}\int_{-\infty}^\infty e^{-ipx/\hbar}\psi(x)dx=\frac{1}{\sqrt{ 2\pi \hbar }}\int_{-a/2}^{a/2}e^{-ipx/\hbar}\sqrt{ \frac{2}{a} }\cos \frac{\pi x}{a}dx \\
=\frac{1}{\sqrt{ a\pi \hbar }}\int_{-a/2}^{a/2}e^{-ipx/\hbar}\cos \frac{\pi x}{a}dx  \\
=\frac{1}{\sqrt{ a\pi \hbar }}\left( \frac{-\frac{ip}{\hbar}e^{-ipx/\hbar}\cos \frac{\pi x}{a}+\frac{\pi}{a}e^{-ipx/\hbar}\sin \frac{\pi x}{a}}{\frac{p^2}{\hbar^2}+\frac{\pi^2}{a^2}} \right)\Big|_{-a/2}^{a/2} \\
=\frac{1}{\sqrt{ a\pi \hbar }}\left( \frac{-\frac{ip}{\hbar}e^{-ipa/2\hbar}\cos \frac{\pi}{2}+\frac{\pi}{a}e^{-ipa/2\hbar}\sin \frac{\pi}{2}+\frac{ip}{\hbar}e^{ipa/2\hbar}\cos \frac{-\pi}{2}-\frac{\pi}{a}e^{ipa/2\hbar}\sin \frac{-\pi}{2}}{\frac{p^2}{\hbar^2}+\frac{\pi^2}{a^2}} \right) \\
=\frac{1}{\sqrt{ a\pi \hbar }}\left( \frac{\frac{\pi}{a}e^{-ipa/2\hbar}+\frac{\pi}{a}e^{ipa/2\hbar}}{\frac{p^2}{\hbar^2}+\frac{\pi^2}{a^2}} \right) \\
=\frac{1}{\sqrt{ a\pi \hbar }}\left( \frac{\frac{\pi}{a}\cos\left( \frac{pa}{2\hbar} \right)}{\frac{p^2}{\hbar^2}+\frac{\pi^2}{a^2}} \right)\\
=\frac{1}{\sqrt{ a\pi \hbar }}\left( \frac{\frac{\pi}{a}\cos\left( \frac{pa}{2\hbar} \right)}{\frac{p^2h^2+\pi^2a^2}{h^2a^2}} \right) \\
=\frac{1}{\sqrt{ a\pi \hbar }}\left( \frac{\pi \hbar^2a\cos\left( \frac{pa}{2\hbar} \right)}{p^2h^2+\pi^2a^2} \right)
\end{gather}
$$
$$
\begin{gather}
|\psi(p)|^2dp=\frac{1}{ a\pi \hbar }\left( \frac{\pi \hbar^2a\cos\left( \frac{pa}{2\hbar} \right)}{p^2\hbar^2+\pi^2a^2} \right)^2dp=\frac{1}{ a\pi \hbar }\frac{\pi^2\hbar^4a^2\cos^2\left( \frac{pa}{2\hbar} \right)}{p^4\hbar^4+\pi^4a^4+2p^2\hbar^2\pi^4a^4}dp= \\
\frac{\pi\hbar^3a\cos^2\left( \frac{pa}{2\hbar} \right)}{p^4\hbar^4+\pi^4a^4+2p^2\hbar^2\pi^4a^4}dp
\end{gather}

$$


##### 6.13
Outside the well $\psi(x)=0$
Inside the well $V(x)$
$$
\begin{align}
\left( \frac{-\hbar^2}{2m}\frac{d^2}{dx^2} +V(x) \right)\psi(x) &=E\psi(x) \\
\frac{-\hbar^2}{2m}\frac{d^2}{dx^2}\psi(x) &=E\psi(x) \\
\frac{d^2}{dx^2}\psi(x)&=-\frac{2mE}{\hbar^2}\psi(x)
\end{align}
$$
$$
\begin{gather}
\omega^2=\frac{2mE}{\hbar^2} \\
\psi(x)=A\sin(\omega x)+B\cos(\omega x) \\
\psi(0)=0=A\sin(\omega x)+B\cos(\omega x) \\
B=0 \\
\psi(x)=A\sin(\omega x) \\
\psi(L)=0=A\sin(\omega L) \\
\omega L=n\pi \\
\end{gather}
$$
$n=1,2,3,\dots$
$$
\begin{align}
\sqrt{ \frac{2mE_{n}}{\hbar^2} }&=\frac{n\pi}{L} \\
\frac{2mE_{n}}{\hbar^2} &=\frac{n^2\pi^2}{L^2} \\
E_{n}&=\frac{\hbar^2\pi^2n^2}{2mL^2}
\end{align}
$$
$$
\psi_{n}(x)=A\sin\left( \sqrt{ \frac{2mE}{\hbar^2} }x \right)=A\sin\left( \frac{n\pi x}{L} \right)
$$
Normalize 
$$
\begin{align}
\int_{0}^LA^2\sin^2\left( \frac{n\pi x}{L} \right)dx&=1 \\
A^2\left( \frac{L}{2}-\frac{\sin(2m\pi x)}{4} \right)&=1 \\
\frac{A^2L}{2}&=1 \\
A^2&=\sqrt{ \frac{L}{2} } \\
\psi_{n}(x)&=\sqrt{ \frac{L}{2} }\sin\left( \frac{n\pi x}{L} \right)
\end{align}
$$
##### 3.14
$$
\psi_{0}(x)=\sqrt{ \frac{2}{L} }\sin \frac{\pi x}{L}
$$
$$
\begin{gather}
\braket{  x } =\frac{L}{2} \\
\braket{  x^2 } =\int_{-\infty}^\infty |\psi_{0}(x)|^2x^2dx=\frac{2}{L}\int_{0}^L \sin^2\left( \frac{n\pi x}{L} \right)x^2dx=\left( \frac{1}{3}-\frac{1}{2\pi^2} \right)L^2 \\
\Delta x=\sqrt{ \braket{  x^2 } -\braket{ x } ^2 }=\sqrt{\left( \frac{1}{3}-\frac{1}{2\pi^2} \right)L^2-\frac{L^2}{4}   }=L\sqrt{ \frac{1}{12}-\frac{1}{2\pi^2} } \\ 
\end{gather}
$$

$\psi_{0}(x)$ is real so $\braket{  p_{x} }=0$
$$
\begin{gather}
\braket{  p_{x}^2 }=\int_{-\infty}^\infty \psi^*(x)\left( \frac{\hbar}{i} \right)^2\frac{d^2}{dx^2} \psi(x)dx= \\
-\hbar^2\int_{0}^L\sqrt{ \frac{2}{L} }\sin \frac{\pi x}{L}\left( -\sqrt{ \frac{2}{L} }\frac{\pi^2}{L^2}\sin \frac{\pi x}{L} \right)dx= \\
\frac{2\hbar^2}{L}\frac{\pi^2}{L^2}\int_{0}^L\sin^2\left( \frac{\pi x}{L} \right)dx= \\
\frac{2\hbar^2}{L}\frac{\pi^2}{L^2}\frac{L}{2}=\frac{\hbar^2\pi^2}{L^2} \\
\Delta p_{x}=\sqrt{ \braket{  p_{x}^2 }-\braket{  p_{x} }^2 }=\sqrt{ \frac{\hbar^2\pi^2}{L^2} }=\hbar \frac{\pi}{L} \\
\Delta x\Delta p_{x}=L\sqrt{ \frac{1}{12}-\frac{1}{2\pi^2} }\hbar \frac{\pi}{L}=\hbar \pi\sqrt{ \frac{1}{12}-\frac{1}{2\pi^2}}
\end{gather}
$$
##### 6.15
###### a
$$
\begin{gather}
\psi(x,t)=\hat{U}(t)\psi(x)=e^{-iEt/\hbar}\left( \frac{1+i}{2} \right) \sqrt{ \frac{2}{L} }\sin\left( \frac{\pi x}{L} \right)+e^{-iEt/\hbar}\left( \frac{1}{\sqrt{ 2 }} \right) \sqrt{ \frac{2}{L} }\sin\left( \frac{2\pi x}{L} \right)= \\
=e^{-i\hbar \pi^2t/2mL^2}\left( \frac{1+i}{2} \right) \sqrt{ \frac{2}{L} }\sin\left( \frac{\pi x}{L} \right)+e^{-2i\hbar \pi^2t/mL^2}\left( \frac{1}{\sqrt{ 2 }} \right) \sqrt{ \frac{2}{L} }\sin\left( \frac{2\pi x}{L} \right)
\end{gather}
$$
###### b
$$
\braket{  E } =\frac{1}{2}\frac{\hbar^2\pi^2}{2mL^2} +\frac{1}{2}\frac{\hbar^2\pi^24}{2mL^2}=\frac{5\hbar^2\pi^2}{4mL^2}
$$
###### c
$$
|\braket{ E_{1} | \psi(x) }|^2= \left| \frac{1+i}{2} \right|^2=\left( \frac{\sqrt{ 2 }}{2} \right)^2=\frac{1}{2}
$$
###### d
The local phase of $\psi(x,t)$ changes with time since it is made up of multiple eigenstates. This means the probabilities of $\psi(x,t)$ change with time. This causes $\braket{  x }$ to change.

##### 6.16
##### a
Old ground state: $\sqrt{ \frac{2}{L} }\sin\left( \frac{\pi x}{L} \right)$ for 0 to L
New ground state: $\sqrt{ \frac{1}{L} }\sin\left( \frac{\pi x}{2L} \right)$ for 0 to 2L
$$
\begin{gather}
\braket{ \psi_{new} | \psi_{old} } =\int_{-\infty}^\infty \psi_{new}^*(x)\psi_{old}(x)dx=\int_{0}^L\sqrt{ \frac{1}{L} }\sin\left( \frac{\pi x}{2L} \right)\sqrt{ \frac{2}{L} }\sin\left( \frac{\pi x}{L} \right)dx= \\
\frac{\sqrt{ 2 }}{L}\int_{0}^L\sin\left( \frac{\pi x}{2L} \right)\sin\left( \frac{\pi x}{L} \right)dx=\frac{\sqrt{ 2 }}{2L}\int_{0}^L\cos\left( \frac{\pi x}{L}-\frac{\pi x}{2L} \right)-\cos\left( \frac{\pi x}{L}+\frac{\pi x}{2L} \right)dx \\
=\frac{1}{\sqrt{ 2 }L}\int_{0}^L\cos\left( \frac{\pi x}{2L} \right)-\cos\left( \frac{3\pi x}{2L} \right)=\frac{1}{\sqrt{ 2 }L}\left( \sin\left( \frac{\pi}{2} \right)\frac{2L}{\pi}-\sin\left( \frac{3\pi}{2} \right)\frac{2L}{3\pi} \right) \\
=\frac{1}{\sqrt{ 2 }L}\left( \frac{2L}{\pi}+\frac{2L}{3\pi} \right)=\frac{8}{3\sqrt{ 2 }\pi}
\end{gather}
$$
###### b
I would split the old ground state into multiple eigenstates of the new eigenstates. Then multiple each by the $e^{-iEt/\hbar}$ and use their eigenvalues. This is not a stationary system as it is made up of many eigenstates.
##### 6.19
###### a
$V(x)=\frac{-\lambda \hbar^2}{2mb}\delta(x)$
$$
\begin{align}
\left( \frac{-\hbar^2}{2m}\frac{d^2}{dx^2} +\frac{-\lambda \hbar^2}{2mb}\delta(x) \right)\psi(x) &=E\psi(x)  \\
\frac{d^2\psi}{dx^2}dx &=\left( E\psi(x)-\frac{-\lambda \hbar^2}{2mb}\delta(x) \right)\frac{-2m}{\hbar^2} \\
\int_{-\epsilon}^\epsilon \frac{d^2\psi}{dx^2}&=\int_{-\epsilon}^\epsilon-E\psi(x)\frac{-2m}{\hbar^2}+\frac{-\lambda \hbar^2}{2mb}\delta(x)\psi(x)\frac{-2m}{\hbar^2}dx \\
\frac{d\psi}{dt}_{0^+} -\frac{d\psi}{dt}_{0^-} &=-\frac{2m}{\hbar^2}\frac{-\lambda \hbar^2}{2mb}\psi(0)=-\frac{\lambda}{b}
\psi(0)\end{align}
$$
###### b
For $x\neq0$ $V(x)=0$ 
$$
\begin{gather}
\frac{d^2}{dx^2}\psi(x)=-\frac{2mE}{\hbar^2}\psi(x) \\
q^2=-\frac{2mE}{\hbar^2} \\
\psi(x)=Ae^{qx}+Be^{-qx} \\
\end{gather}
$$
We know that psi converges so:
For $x>0$ then $\psi(x)=Be^{-qx}$
For $x<0$ then $\psi(x)=Ae^{qx}$
We know $\psi(x)$ is continuous so:
$$\begin{gather}
\psi(0)=\psi(x)=Be^0=Ae^0 &B=A \\

\end{gather}
$$



$$
\begin{gather}
\frac{d\psi}{dt}_{0^+} -\frac{d\psi}{dt}_{0^-} =-\frac{\lambda}{b}
\psi(0) \\
-qA-qA=-\frac{\lambda}{b}A \\
-2q=-\frac{\lambda}{b} \\
q=\frac{\lambda}{2b} \\
q^2=\frac{\lambda^2}{4b^2} \\
-\frac{2mE}{\hbar^2}=\frac{\lambda^2}{4b^2} \\
E=-\frac{\lambda^2\hbar^2}{8mb^2}
\end{gather}
$$
![[sketch.jpg]]
