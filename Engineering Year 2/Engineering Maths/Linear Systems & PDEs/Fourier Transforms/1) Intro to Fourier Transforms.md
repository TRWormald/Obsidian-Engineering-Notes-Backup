The **Fourier Transform** is a tool to analyse non-periodic signals, and systems.

To find the frequency content of an *arbitrary function* $f(t)$, we truncate the function to $- \frac{T}{2}<t<\frac{T}{2}$, frequency analyse with a regular Fourier series, and take the limit $T\rightarrow\infty$.

When doing this we will use an alternate form of the equation for a Fourier Series which uses complex exponents to represent the sines and cosines:
$$f(t)\sim\sum\limits_{n=-\infty}^{\infty}c_{n}e^{jn\omega t}$$
Where:
$$c_{n}=\frac{1}{2}(a_{n}-jb_{n})=\frac{1}{T}\int_{-T/2}^{T/2}~f(t)e^{-jn\omega t}~dt,~~c_{-n}=c_{n}$$
### Example in Pictures
Say we have a signal $f(t)$:
![[Pasted image 20241117141826.png|centre|300]]
We will then truncate it over a period $T$:
![[Pasted image 20241117141900.png|centre|300]]
Note how we have limited the curve and how that effects its geometry.
And then frequency analyse it:
![[Pasted image 20241117141922.png|centre|300]]
Let us now increase $T$:
![[Pasted image 20241117142121.png|centre]]
And increase it even further:
![[Pasted image 20241117142141.png|centre]]
Eventually at the limit these points on the frequency diagram become infinitesimally far apart from each other and therefore we become interested in the line representing them:
![[Pasted image 20241117142331.png|centre]]
