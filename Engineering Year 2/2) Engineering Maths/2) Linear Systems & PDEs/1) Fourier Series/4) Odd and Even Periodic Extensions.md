We have looked at how to analyse a *periodic function*, but what about non-periodic functions, how do we analyse them?
There are two different types to consider:
1) $f(t)$ is non-periodic, defined for all $t\in \mathbb{R}$
	- We solve these using a **Fourier Transform**
2) $f(t)$ is non-periodic, but defined only for a finite interval $0\le t\le L$
	- We can solve these by constructing a periodic function by repetition - the odd and even periodic extensions.
	- This leads to a **Fourier Half-Range Series**
### Generating the Odd and Even Functions
Let $f(t)$ be some function defined in the region $0\le t\le L$:
![[Pasted image 20241117124057.png|centre]]
To make it an even function $f_{e}(t)$ we need to reflect it in the y-axis:
![[Pasted image 20241117124145.png|centre]]
So that $f(t)=f(-t)$.

However to make it an odd function $f_{o}(t)$ we need to reflect it in the x- and y-axes:
![[Pasted image 20241117124300.png|centre]]
So that $f(-t)=-f(t)$.
Having done this we have effectively constructed two periodic functions with period $2L$:
![[Pasted image 20241117124442.png|centre]]
### Definitions
Let $f(t)$ be a function defined on the interval $0\le t\le L$

The **even periodic extension** of $f$ is the function $f_{e}$ defined for $-\infty\lt t \lt \infty$, which satisfies $f_{e}(-t)=f_{e}(t)$ and $f_{e}(t+2L)=f_{e}(t)$ for all $t$.
The Fourier Series of the even periodic extension is called the half-range cosine series.

The **odd periodic extension** of $f$ is the function $f_{0}$ defined for $-\infty\lt t \lt \infty$, which satisfies $f_{o}(-t)=-f_{o}(t)$ and $f_{o}(t+2L)=f_{o}(t)$ for all $t$.
The Fourier Series of the odd periodic extension is called the half-range sine series.

**Note that the odd and even periodic extensions both have period $T=2L$ and frequency $\omega=\frac{2\pi}{T}=\frac{\pi}{L}$**
### The Half-Range Cosine Series
The half-range cosine series of a function$f(t)$ given on an interval $0\le t\le L$ is the Fourier series of its even periodic extension:
$$f(t)\sim \frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}a_{n}\cos\left(\frac{n\pi t}{L}\right) $$
where:
$$a_{n}=\frac{2}{L}\int_{0}^{L}f(t)\cos\left(\frac{n\pi t}{L}\right)~dt$$
### The Half-Range Sine Series
The half-range sine series of a function$f(t)$ given on an interval $0\le t\le L$ is the Fourier series of its odd periodic extension:
$$f(t)\sim \sum\limits_{n=1}^{\infty}b_{n}\sin\left(\frac{n\pi t}{L}\right) $$
where:
$$b_{n}=\frac{2}{L}\int_{0}^{L}f(t)\sin\left(\frac{n\pi t}{L}\right)~dt$$
### Worked Example 1.4
![[Pasted image 20241117125348.png|centre]]
$$\frac{1}{T}\int_{0}^T f(t)dt\ne0$$
