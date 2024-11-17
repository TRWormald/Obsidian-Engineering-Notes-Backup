The only stipulation for a function to have a Fourier transform is that it contains a "finite amount of energy":
$$\int_{-\infty}^{\infty}|f(t)|~dt<\infty$$
Which implies that we need $f\rightarrow 0$ as $t\rightarrow\pm\infty$. (For example, $f(t)=\sin(t)$ won't work, nor will any other periodic function)

For technical reasons we also require that $f$ has at most a finite number of maxima and minima, and a finite number of discontinuities in a finite interval. For example $f(t)=\sin\left(\frac{1}{t}\right)$ won't work.