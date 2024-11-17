The **Fourier Transform** is a tool to analyse non-periodic signals, and systems.

To find the frequency content of an *arbitrary function* $f(t)$, we truncate the function to $- \frac{T}{2}<t<\frac{T}{2}$, frequency analyse with a regular Fourier series, and take the limit $T\rightarrow\infty$.

When doing this we will use an alternate form of the equation for a Fourier Series which uses complex exponents to represent the sines and cosines:
$$f(t)\sim\sum\limits_{n=-\infty}^{\infty}c_{n}e^{jn\omega t}$$
Where:
$$c_{n}=\frac{1}{2}(a_{n}-jb_{n})=\frac{1}{T}\int_{-T/2}^{T/2}~f(t)e^{-jn\omega t}~dt,~~c_{-n}=c_{n}$$
