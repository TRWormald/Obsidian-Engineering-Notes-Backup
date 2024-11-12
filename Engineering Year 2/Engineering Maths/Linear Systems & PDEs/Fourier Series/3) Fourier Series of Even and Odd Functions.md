Functions that are even or odd have simpler Fourier series.
If $f(t)$ is an **even function** - i.e. if $f(-t)=f(t)$ for all $t$ then:
$$f(t)\sim \frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty} a_{n}\cos(n\omega t)$$
So $b_{n}=0$ for all $n$ and $a_{n}=\frac{4}{T}\int_{0}^{\frac{T}{2}}f(t)\cos(n\omega t)~dt$.

If $f(t)$ is an **odd function** - i.e. if $f(-t)=-f(t)$ for all $t$ then:
$$f(t)\sim \sum\limits_{n=1}^{\infty} b_{n}\sin(n\omega t)$$
So $a_{n}=0$ for all $n$ and $b_{n}=\frac{4}{T}\int_{0}^{\frac{T}{2}}f(t)\sin(n\omega t)~dt$.

##### Worked Example 1.3
