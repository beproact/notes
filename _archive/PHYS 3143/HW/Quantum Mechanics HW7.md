### Jason Low
##### 6.5
###### a
$$
1=\braket{ \psi | \psi } =\int_{-\infty}^\infty \braket{ \psi | p } \braket{ p | \psi } dp=\int_{-\infty}^\infty |\braket{ p | \psi } |^2dp=\int_{-P/2}^{P/2}|N|^2dp=|N|^2P=1
$$
$$
N=\frac{1}{\sqrt{ P }}
$$
###### b
$$
\begin{gather}
\psi(x)=\frac{1}{\sqrt{ 2\pi \hbar }}\int_{-\infty}^\infty e^{ipx/\hbar}\psi(p)dp 
=\frac{1}{\sqrt{ 2\pi \hbar }}\int_{-P/2}^{P/2} e^{ipx/\hbar}Ndp=\frac{1}{\sqrt{ 2\pi \hbar }}\frac{\hbar}{ix}(e^{iPx/2\hbar}-e^{-iPx/2\hbar})N \\
=\frac{1}{\sqrt{ 2\pi \hbar }}\frac{\hbar}{ix}2i\sin\left( \frac{Px}{2\hbar} \right)\frac{1}{\sqrt{ P }}=\frac{\sqrt{ 2 \hbar}}{x\sqrt{ \pi P }}\sin\left( \frac{Px}{2\hbar} \right)
\end{gather}
$$

##### 6.6
###### a
$$
\begin{gather}
\frac{d}{dx}g(x)^2=2g'(x)g(x)   \\
\frac{d}{dx}\frac{1}{2}g(x)^2=g(x)\frac{d}{dx} g(x)
\end{gather}

$$
If $\braket{ x | \psi }$ is real then, $\braket{ x | \psi }=\braket{ \psi | x }$
$$
\begin{gather}
\braket{  p_{x} } =\bra{\psi} p_{x}\ket{\psi} =\int_{-\infty}^\infty  \braket{ \psi | x } p_{x}\braket{ x | \psi }dx \\
= \int_{-\infty}^\infty \psi(x)\frac{\hbar}{i}\frac{d}{dx} \psi(x)dx=\frac{\hbar}{i}\int_{-\infty}^\infty \psi(x)\frac{d}{dx}\psi(x)dx=\frac{\hbar}{2i}\int_{-\infty}^\infty \frac{d}{dx}\psi(x)^2
\end{gather}
$$
$\psi(x)^2$ is even. The derivative of an even function is odd. This means:
$$
\braket{  p_{x} }= \int_{-\infty}^\infty \frac{d}{dx}\psi(x)^2=0
$$
###### b
$[e^{ip_{0}x/\hbar},x]=0$
$$
\begin{gather}
\braket{  x }'=\bra{\psi}x\ket{\psi}=\int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar} xe^{ip_{0}x/\hbar}\braket{ x | \psi } dx= 
\int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar} e^{ip_{0}x/\hbar}\braket{ x | \psi }x dx   \\
=\int_{-\infty}^\infty \braket{ \psi | x } x\braket{ x | \psi } dx=\braket{  x } 
\end{gather}
$$
$$
\begin{align}
\braket{  p_{x} }'&=\bra{\psi} p_{x}\ket{\psi}  \\
&=\int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar} p_{x}e^{ip_{0}x/\hbar}\braket{ x | \psi } dx \\
&=\frac{\hbar}{i} \int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar} \frac{d}{dx} (e^{ip_{0}x/\hbar}\braket{ x | \psi }) dx \\
&=\frac{\hbar}{i} \int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar}  
 \left( \frac{ip_{0}}{\hbar}e^{ip_{0}x/\hbar}\braket{ x | \psi } +e^{ip_{0}x/\hbar}\frac{d}{dx} \braket{ x | \psi }  \right) dx \\
&=\frac{\hbar}{i}\int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar}  \frac{ip_{0}}{\hbar}e^{ip_{0}x/\hbar}\braket{ x | \psi } dx+\frac{\hbar}{i}\int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar}e^{ip_{0}x/\hbar}\frac{d}{dx} \braket{ x | \psi }dx \\
&=\int_{-\infty}^\infty \braket{ \psi |x }e^{-ip_{0}x/\hbar}  p_{0}e^{ip_{0}x/\hbar}\braket{ x | \psi } dx+\int_{-\infty}^\infty \braket{ \psi |x }\frac{\hbar}{i}\frac{d}{dx} \braket{ x | \psi }dx \\
&=\int_{-\infty}^\infty \braket{ \psi |x }  p_{0}\braket{ x | \psi } dx+\int_{-\infty}^\infty \braket{ \psi |x }p_{x} \braket{ x | \psi }dx \\
&=\braket{  p_{x} } +p_{0}
\end{align}
$$
