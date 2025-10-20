Laplace and Fourier transforms have lots of similarities:
$$\text{Fourier: }F[f(t)]=\int_{-\infty}^{\infty}e^{-j\omega t}f(t)\cdot dt$$$$\text{Laplace: }L[f(t)]=\int_{0}^{\infty}e^{-st}f(t)\cdot dt$$
Where Fourier has an oscillating exponential Laplace replaces it with a decaying one - which means that Laplace transforms can deal with signals that don't have finite energy.

The lower limit of the integration is changed from negative infinity to zero - as the Laplace transform is for processes that occur forward in time from t=0.

And the Laplace transform has no real equivalent of Fourier spectra.