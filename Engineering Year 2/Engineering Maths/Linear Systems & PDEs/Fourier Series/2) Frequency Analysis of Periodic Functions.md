To analyse a periodic function we find its **Fourier series.** To do this we write it as a sum of periodic building blocks - sines and cosines.
##### Theorem
A periodic function $f(t)$, with period $T$, can be represented as a Fourier Series:
$$f(t)\sim \frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}a_{n}\cos(n\omega t)+b_{n}\sin(n\omega t)$$
where $\omega=\frac{2\pi}{T}$. The Fourier coefficients $a_{n}$ and $b_{n}$ are given by integrals over one period of $f$:
$$\begin{align*}
a_{n}&= \frac{2}{T}\int_{-T/2}^{T/2}~f(t)\cos(n\omega t)~dt\\
b_{n}&= \frac{2}{T}\int_{-T/2}^{T/2}~f(t)\sin(n\omega t)~dt
\end{align*}$$
*Note that the $\frac{a_{0}}{2}$ is the "DC offset" or the constant value around which the function oscillates. This can be seen in the way that it does not vary with time.*

The $n$th term in the sum is called the $n$th harmonic component of $f$:
$$a_{n}\cos(n\omega t)+b_{n}\sin(n\omega t)$$
It has frequency $n\omega$ and period $T/n$.
$a_{n}$ and $b_{n}$ together tell us how much of frequency $n\omega$ is in $f$, with the power in the $n$th harmonic being:
$$\frac{1}{2}(a_{n}^{2}+b_{n}^{2})$$
##### Visualisation
To visualise a Fourier series, we plot a line spectrum (also called the magnitude spectrum), which is a graph of energy (on the y-axis) against frequency (on the x-axis). 
At each frequency $n\omega$ ($n\ge 0$) we plot a line with height $\frac{1}{2}\sqrt{a_{n}^{2}+b_{n}^{2}}$, note that line heights at frequency $-n\omega$ and $n\omega$ are the same (symmetric in the y-axis).
![[Pasted image 20241112094416.png|centre]]

##### Worked Example 1.2
![[Pasted image 20241112100553.png]]
