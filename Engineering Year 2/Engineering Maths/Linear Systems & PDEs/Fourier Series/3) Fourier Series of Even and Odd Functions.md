Functions that are even or odd have simpler Fourier series.
If $f(t)$ is an **even function** - i.e. if $f(-t)=f(t)$ for all $t$ then:
$$f(t)\sim \frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty} a_{n}\cos(n\omega t)$$
So $b_{n}=0$ for all $n$ and $a_{n}=\frac{4}{T}\int_{0}^{\frac{T}{2}}f(t)\cos(n\omega t)~dt$.

If $f(t)$ is an **odd function** - i.e. if $f(-t)=-f(t)$ for all $t$ then:
$$f(t)\sim \sum\limits_{n=1}^{\infty} b_{n}\sin(n\omega t)$$
So $a_{n}=0$ for all $n$ and $b_{n}=\frac{4}{T}\int_{0}^{\frac{T}{2}}f(t)\sin(n\omega t)~dt$.

##### Worked Example 1.3
![[Pasted image 20241112100618.png]]


Note how the convergence is much slower than in [[2) Frequency Analysis of Periodic Functions#Worked Example 1.2|Worked Example 1.2]]. Even with 500 terms in the Fourier series there is significant overshoot and high frequency oscillation near $t=\pm L$ - this is called the Gibbs Phenomenon. This relates to **the specific behaviour of functions showing over- and under-shoots around a jump discontinuity**.
In short - a discontinuity in $f$ results in high frequency oscillation about the actual value near it. This is what causes fringing in compressed images where one colour shifts to another, very different, colour.
