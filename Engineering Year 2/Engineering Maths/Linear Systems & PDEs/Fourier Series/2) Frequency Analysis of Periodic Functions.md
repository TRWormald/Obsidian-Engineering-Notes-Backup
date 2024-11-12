To analyse a periodic function we find its **Fourier series.** To do this we write it as a sum of periodic building blocks - sines and cosines.

**Theorem**
A periodic function $f(t)$, with period $T$, can be represented as a Fourier Series:
$$f(t)\approx \frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}a_{n}\cos(n\omega t)+b_{n}\sin(n\omega t)$$
where $\omega=\frac{2\pi}{T}$. The Fourier coefficients $a_{n}$ and $b_{n}$ are given by integrals over one period of $f$:
$$\begin{align*}
a_{n}&= \frac{2}{T}\int_{-T/2}^{T/2}~f(t)\cos(n\omega t)~dt\\
b_{n}&= \frac{2}{T}\int_{-T/2}^{T/2}~f(t)\sin(n\omega t)~dt
\end{align*}$$
