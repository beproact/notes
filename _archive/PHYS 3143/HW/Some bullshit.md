
$$
\ket{\psi}\to \ket{\psi'}=\hat{T}(\delta x)\ket{\psi}=\hat{T}(\delta x)\int_{-\infty}^\infty \ket{x} \braket{ x | \psi } dx=\int_{-\infty}^\infty \ket{x+\delta x}\braket{ x | \psi } dx
$$
$$
\psi'(x)=\psi(x-\delta x)=\braket{ x | \psi }-\delta x\frac{d}{dx}\braket{ x | \psi }   
$$
$$
\begin{gather}
\braket{  x }'=\bra{\psi'(x)}x\ket{\psi'(x)} =\int_{-\infty}^\infty \psi'(x)x\psi'(x)dx \\
=\int_{-\infty}^\infty \psi^*(x-\delta x)x\psi(x-\delta x)dx \\ 
=\int_{-\infty}^\infty \left( \braket{ \psi |x }-\delta x\frac{d}{dx}\braket{ \psi |x } \right)   x\left( \braket{ x | \psi }-\delta x\frac{d}{dx}\braket{ x | \psi } \right)dx \\
=\int_{-\infty}^\infty \braket{ \psi |x }x\braket{ x | \psi }dx+\delta x\int_{-\infty}^\infty \braket{ \psi |x }\braket{ x | \psi }dx \\
=\braket{  x }+\delta x 
\end{gather}
$$

#### 

$$
\begin{gather}
\braket{  p_{x} }'=\bra{\psi'(x)}p_{x}\ket{\psi'(x)} =\int_{-\infty}^\infty \psi'(x)p_{x}\psi'(x)dx \\
=\int_{-\infty}^\infty \psi^*(x-\delta x)p_{x}\psi(x-\delta x)dx \\
=\int_{-\infty}^\infty \left( \braket{ \psi |x }-\delta x\frac{d}{dx}\braket{ \psi |x } \right)   p_{x}\left( \braket{ x | \psi }-\delta x\frac{d}{dx}\braket{ x | \psi } \right)dx \\
=\int_{-\infty}^\infty \left( \braket{ \psi |x }-\delta x\frac{d}{dx}\braket{ \psi |x } \right)   \frac{\hbar}{i}\frac{d}{dx} \left( \braket{ x | \psi }-\delta x\frac{d}{dx}\braket{ x | \psi } \right)dx \\
=\int_{-\infty}^\infty \braket{ \psi |x }p_{x}\braket{ x | \psi }dx \\
=\braket{  p_{x} }
\end{gather}
$$



$$
\begin{gather}
\begin{pmatrix}
\bra{\frac{1}{2}}\hat{J}^+\ket{\frac{1}{2}}   &  
\bra{\frac{1}{2}}\hat{J}^+\ket{-\frac{1}{2}}   \\
\bra{-\frac{1}{2}}\hat{J}^+\ket{\frac{1}{2}}   &  
\bra{-\frac{1}{2}}\hat{J}^+\ket{-\frac{1}{2}}  
\end{pmatrix} = \\
\begin{pmatrix}
0 & \bra{\frac{1}{2}}\hat{J}^+\ket{-\frac{1}{2}} \\
\bra{-\frac{1}{2}}\hat{J}^+\ket{\frac{1}{2}} & 0
\end{pmatrix} = \\
\begin{pmatrix}
0 & {\hbar} \\
\bra{-\frac{1}{2}}\hat{J}^+\ket{\frac{1}{2}}  & 0
\end{pmatrix}
\end{gather}
$$

$$
J_{z}J_{_+}\ket{j,m}= J_{z}J_{+}\ket{j,(m+1)mod m|} 
$$

I'm not doing this generally actually

$$
\begin{align}
&\bra{\frac{1}{2},\frac{1}{2}} J_{-}J_{+} \ket{\frac{1}{2},\frac{1}{2}} \\
&=|C|^2\braket{ \frac{1}{2}, -\frac{1}{2} | \frac{1}{2}, -\frac{1}{2} }   \\
&=|C|^2
\end{align}

$$




$$
\begin{align}
J_{+}J_{-}=J^2-J_{z}^2+\hbar J_{z} \\
J_{-}J_{+}=J^2-J_{z}^2-\hbar J_{z}
\end{align}
$$This is what we used to find $j$ in class.
Lets call $j$ the highest possible value. Lets call $j'$ the lowest value.
$$
\begin{gather}
J_{+}J_{-}\ket{\lambda,j'} =(J^2-J_{z}^2+\hbar J_{z})\ket{\lambda,j'} =\hbar^2(\lambda-j'^2+j')\ket{\lambda,j'}  \\
J_{-}J_{+}\ket{\lambda,j} =(J^2-J_{z}^2-\hbar J_{z})\ket{\lambda,j} =\hbar^2(\lambda-j^2-j)\ket{\lambda,j}
\end{gather}
$$
I made two assumptions here. I assumed $j=-j'$ and assume the constant in front should equal.
