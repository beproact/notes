Ket Vector
$$
\begin{gather}
\ket{+Z} \to S_{z}=\frac{\hbar}{2}\ \\
\ket{-Z} \to S_{z}=-\frac{\hbar}{2} \\
\ket{\psi} =C_{+}\ket{+Z} +C_{-}\ket{-Z} 
\end{gather}
$$
$C_{+}$ and $C_{-}$ are probability amplitudes.
$$
\begin{gather}
\mathbb{P}\ket{+Z}=|C_{+}|^2 \\
\mathbb{P}\ket{-Z}=|C_{-}|^2 
\end{gather}
$$
Bra Vector
$$
\bra{+Z}  
$$
To multiply 2 vectors you have to multiply a bra by a ket.
$$
\begin{gather}
\braket{+Z|+Z}=1  \\
\braket{ +Z | -Z } =0 \\
\braket{ -Z | +Z } =0  \\
\braket{ -Z | -Z } =1
\end{gather}
$$
The bra can be though of as the vector in which you are measuring.
$$
\begin{gather} \\ \\

\ket{\psi} =C_{+}\ket{+Z} +C_{-}\ket{-Z} \\
\braket{ +Z | \psi } =C_{+}\braket{ +Z | +Z } + \braket{ +Z | -Z }  \\
 C_{+}=\braket{ +Z | \psi } \\
\ket{\psi} =\braket{ +Z | \psi } \ket{+Z} +\braket{ -Z | \psi } \ket{-Z} \\ 
\end{gather}

$$
$$
\begin{gather}
\ket{\psi}= C_{+}\ket{+Z} +C_{-}\ket{-Z} \\
\bra{\psi} =C'_{+}\bra{+Z} +C'_{-}\bra{-Z}   \\
\braket{ \psi | \psi } = 1  \\
=(C_{+}\ket{+Z} +C_{-}\ket{-Z})(C'_{+}\bra{+Z} +C'_{-}\bra{-Z}) \\
=C'_{+}C_{+}\braket{ +Z | +Z } +C'_{+}C_{-}\braket{ +Z | -Z } +C'_{-}C_{+}\braket{ -Z | +Z } +C'_{-}C_{-}\braket{ -Z | -Z } \\
=C'_{+}C_{+}+C'_{-}C_{-}=1 \\ 
\end{gather}
$$
Bra is found with complex conjugate of $C_{+}$ and $C_{-}$ so
$$
\begin{gather}
C'_{+}=C^*_{+} \\
C'_{-}=C^*_{-} \\
\bra{\psi} =C^*_{+}\bra{+Z} +C^*_{-}\bra{-Z}  \\
C^*_{+}=\braket{ \psi | +Z } 
\end{gather}
$$
Swapping the term in the bra and ket gives the complex conjugate
$$
\braket{ \psi | \varphi }=\braket{ \varphi | \psi }^*  
$$
Expectation Value/Mean $\braket{ S_{Z} }$
$$
\braket{ S_{Z} }=\frac{\hbar}{2}\cdot|C_{+}|^2+\left( -\frac{\hbar}{2} \right)|C_{-}|^2
$$
Uncertainty $\Delta S_{Z}$
$$
\begin{gather}
(\Delta S)^2=\braket{ |S_{Z}-\braket{  S_{Z} } |^2 }=\braket{ S_{Z}^2}-\braket{  S_{Z} }   ^2 \\
\braket{ S_{Z}^2  } =\left( \frac{\hbar}{2} \right)^2=\frac{\hbar^2}{4} \\
\Delta S_{Z}=\sqrt{ \left( \frac{\hbar^2}{4} \right)-\braket{  S_{Z} }^2  }
\end{gather}

$$
