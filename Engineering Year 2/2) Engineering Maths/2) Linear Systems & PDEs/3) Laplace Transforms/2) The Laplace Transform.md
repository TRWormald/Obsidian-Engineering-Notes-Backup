The Laplace transform takes a time domain function and generates an "s-domain" or "Laplace domain" function.
This function has a variable $s$ that corresponds to characteristic decay rates, in the same way that the variable $\omega$ in the Fourier transform corresponds to characteristic frequencies.
#### Definition
The Laplace transform of a function $f(t)$ is:
$$L[f(t)]=F(s)=\int_{0}^{\infty}e^{-st}f(t) \cdot dt$$
Where $L$ is an operator which maps a function of time $t$ to a function of a new variable $s$
The Laplace transform also has a well defined inverse:
$$F(s)=L[f(t)]~~~\Leftrightarrow~~~L^{-1}[F(s)]=f(t)$$
so $f(t)$ and $F(s)$ come in pairs, but there is no simple expression for $L^{-1}$.
![[Pasted image 20250421171941.png|centre]]
