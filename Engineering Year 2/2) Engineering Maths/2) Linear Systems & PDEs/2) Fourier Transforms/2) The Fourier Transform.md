The *Fourier Transform* of a function $f(t)$ is given by:
$$\mathcal{F}[f(t)]=F(\omega)=\int_{-\infty}^{\infty}f(t)e^{-j\omega t}~dt$$
Where $\mathcal{F}$ means "take the Fourier transform of". $\mathcal{F}$ transforms a function of time $f(t)$ to a function of frequency $F(\omega)$.
It is also possible to go back the other way:
The *Inverse Fourier Transform* of $F(\omega)$ is given by:
$$\mathcal{F}^{-1}[F(\omega)]=f(t)=\frac{1}{2\pi}\int_{-\infty}^{\infty}F(\omega)e^{j\omega t}~dt$$
Sometimes $f(t)$ and $F(\omega)$ are called a **Fourier Transform Pair** and are written as:
$$f(t)\leftrightarrow F(\omega)$$
