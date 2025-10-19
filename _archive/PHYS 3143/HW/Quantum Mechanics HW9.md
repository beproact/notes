##### 7.5
###### 7.56
$$
\begin{gather}
(\Delta x)^2=\frac{\hbar}{2m\omega}\bra{n} (\hat{a}+\hat{a}^{\dagger})^2\ket{n} = \frac{\hbar}{2m\omega}\bra{n} (\hat{a}^2)+(\hat{a}^{\dagger})^2+\hat{a}\hat{a}^{\dagger}+\hat{a}^{\dagger}\hat{a}\ket{n} \\
=\frac{\hbar}{2m\omega}\bra{n} \sqrt{ n }\sqrt{ n }+\sqrt{ n+1 }\sqrt{ n+1 } \ket{n}=\frac{\hbar(2n+1)}{2m\omega} =\left( n+\frac{1}{2} \right)\frac{\hbar}{m\omega} \\
\Delta x=\sqrt{ \left( n+\frac{1}{2} \right)\frac{\hbar}{m\omega} }
\end{gather}
$$
###### 7.57
$$
\begin{gather}
(\Delta p_{x})^2=-\frac{m\omega \hbar}{2}\bra{n} (\hat{a}-(\hat{a}^{\dagger}))^2\ket{n} =-\frac{m\omega \hbar}{2}\bra{n} \hat{a}^2+(\hat{a}^{\dagger})^2 -\hat{a}\hat{a}^{\dagger}-\hat{a}^{\dagger}\hat{a}\ket{n} \\
 =\frac{m\omega \hbar}{2}\bra{n} \sqrt{ n }\sqrt{ n }+\sqrt{ n+1 }\sqrt{ n+1 }\ket{n} =\left( n+\frac{1}{2} \right)m\omega \hbar \\
\Delta p_{x}=\sqrt{ \left( n+\frac{1}{2} \right)m\omega \hbar }
\end{gather}
$$
##### 7.7
$$
\begin{gather}
E_{n}=\hbar \omega\left( n+\frac{1}{2} \right) \\ 
\hat{p}_{x}=-i\sqrt{ \frac{m\omega \hbar}{2} }(\hat{a}-\hat{a}^{\dagger}) \\
\ket{\psi(0)}= \frac{1}{\sqrt{ 2 }}\ket{0}+ \frac{e^{i\theta}}{\sqrt{ 2 }}\ket{1}  \\
\hat{p}_{x}\ket{\psi(0)}= -i\sqrt{ \frac{m\omega \hbar}{2} }(\hat{a}-\hat{a}^{\dagger})\left(\frac{1}{\sqrt{ 2 }}\ket{0}+ \frac{e^{i\theta}}{\sqrt{ 2 }}\ket{1}\right)=-\frac{i\sqrt{ m\omega \hbar }}{2}(\hat{a}-\hat{a}^{\dagger})(\ket{0} +e^{i\theta}\ket{1} ) \\
=-\frac{i\sqrt{ m\omega \hbar }}{2}(\hat{a}\ket{0} -\hat{a}^{\dagger}\ket{0} +e^{i\theta}\hat{a}\ket{1}-e^{i\theta}\hat{a}^{\dagger}\ket{1} ) \\
=-\frac{i\sqrt{ m\omega \hbar }}{2}(-\ket{1}+e^{i\theta}\ket{0}-e^{i\theta}\sqrt{ 2 }\ket{2}   ) \\ 

\braket{ p_{x}  } =\bra{\psi(0)} \hat{p}_{x}\ket{\psi(0)} =-\frac{i\sqrt{ m\omega \hbar }}{2}\left(\frac{1}{\sqrt{ 2 }}\bra{0}+ \frac{e^{-i\theta}}{\sqrt{ 2 }}\bra{1}\right)(-\ket{1}+e^{i\theta}\ket{0}-e^{i\theta}\sqrt{ 2 }\ket{2}   ) \\
=\frac{\sqrt{ m\omega \hbar }}{2i}\frac{1}{\sqrt{ 2 }}(e^{i\theta}-e^{-i\theta})=\sqrt{ \frac{m\omega \hbar}{2} }\sin(\theta)=\sqrt{ \frac{m\omega \hbar}{2} } \\
sin(\theta)=1 \\
\theta=\frac{\pi}{2}
\end{gather}
$$
$$
\begin{gather} \\
E_{0}=\frac{\hbar\omega}{2} \\
E_{1}=\frac{3\hbar\omega}{2}\\
\ket{\psi(0)} =\frac{1}{\sqrt{ 2 }}\ket{0} +\frac{i}{\sqrt{ 2 }}\ket{1}  \\
\ket{\psi(t)} =e^{-iHt/\hbar}\ket{\psi(0)}= \frac{1}{\sqrt{ 2 }}e^{-i\omega t/2}\ket{0}+\frac{i}{\sqrt{ 2 }}e^{-3i\omega t/2}\ket{1} \\  
\ket{\psi(t)}=\frac{1}{\sqrt{ 2 }}\ket{0}+\frac{i}{\sqrt{ 2 }}e^{-i\omega t}\ket{1} \\
\hat{p}_{x}\ket{\psi(t)} =-i\sqrt{ \frac{m\omega \hbar}{2} }(\hat{a}-\hat{a}^{\dagger})  \left( \frac{1}{\sqrt{ 2 }}\ket{0}+\frac{i}{\sqrt{ 2 }}e^{-i\omega t}\ket{1} \right)=-\frac{i\sqrt{ m\omega \hbar }}{2}(\hat{a}-\hat{a}^{\dagger})(\ket{0} +ie^{-i\omega t}\ket{1} ) \\
=-\frac{i\sqrt{ m\omega \hbar }}{2}(-\ket{1}+ie^{-i\omega t}\ket{0}-i\sqrt{ 2 }e^{-i\omega t}\ket{2} ) \\
\braket{  \hat{p}_{x} } =\bra{\psi(t)}\hat{p}_{x}\ket{\psi(t)}=\left( \frac{1}{\sqrt{ 2 }}\bra{0}+\frac{-i}{\sqrt{ 2 }}e^{i\omega t}\bra{1}   \right)\left( -\frac{i\sqrt{ m\omega \hbar }}{2}(-\ket{1}+ie^{-i\omega t}\ket{0}-i\sqrt{ 2 }e^{-i\omega t}\ket{2} ) \right) \\
=\frac{\sqrt{ m\omega \hbar }}{2i}\frac{1}{\sqrt{ 2 }}(ie^{-i\omega t}+ie^{i\omega t}) =\sqrt{ \frac{m\omega \hbar}{2} }\cos(\omega t)
\end{gather}

$$
##### 5.9
$$
\ket{\psi(t)}=c_{n}\ket{n} +c_{n+1}e^{-i\omega t}\ket{n+1}  
$$
$$
\begin{gather}
\bra{\psi(t)} \hat{x}\ket{\psi(t)} =\sqrt{ \frac{\hbar}{2m\omega} }(c^*_{n}\bra{n} +c^*_{n+1}e^{i\omega t}\bra{n+1})(\hat{a}+\hat{a}^{\dagger})(c_{n}\ket{n} +c_{n+1}e^{-i\omega t}\ket{n+1} ) \\
=\sqrt{ \frac{\hbar}{2m\omega} }(c_{n}^* c_{n+1}e^{-i\omega t}\sqrt{ n+1 }\braket{ n | n } +c_{n+1}^*e^{i\omega t}c_{n}\sqrt{ n+1 }\braket{ n+1 | n+1 }  ) \\
=\sqrt{ \frac{\hbar(n+1)}{2m\omega} }(c_{n}^* c_{n+1}e^{-i\omega t} +c_{n+1}^*c_{n}e^{i\omega t} ) \\
=\sqrt{ \frac{\hbar(n+1)}{2m\omega} }(c_{n}^* c_{n+1}(\cos(\omega t)-i\sin(\omega t)) +c_{n+1}^*c_{n}(\cos(\omega t)+i\sin(\omega t)) ) \\
=\sqrt{ \frac{\hbar(n+1)}{2m\omega} }(c_{n}^* c_{n+1}+c_{n+1}^*c_{n})\cos(\omega t)+(c_{n+1}^*c_{n}-c_{n}^* c_{n+1})i\sin(\omega t) \\
=C\cos(\omega t)+D\sin(\omega t) \\
=A\cos(\omega t+\delta)
\end{gather}
$$
$$
\begin{gather}
\bra{\psi(t)} \hat{p}_{x}\ket{\psi(t)} =-i\sqrt{ \frac{m\omega \hbar}{2} }(c^*_{n}\bra{n} +c^*_{n+1}e^{i\omega t}\bra{n+1})(\hat{a}-\hat{a}^{\dagger})(c_{n}\ket{n} +c_{n+1}e^{-i\omega t}\ket{n+1} ) \\
=-i\sqrt{ \frac{m\omega \hbar}{2} }(-c_{n}^* c_{n+1}e^{-i\omega t}\sqrt{ n+1 }\braket{ n | n } +c_{n+1}^*e^{i\omega t}c_{n}\sqrt{ n+1 }\braket{ n+1 | n+1 }) \\
=-i\sqrt{ \frac{m\omega \hbar(n+1)}{2} }(c_{n+1}^*c_{n}e^{i\omega t}-c_{n}^* c_{n+1}e^{-i\omega t} ) \\
=-m\omega A\sin(\omega t+\delta)
\end{gather}

$$
