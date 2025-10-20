For the cambered aerofoil $\frac{dz}{dx}\ne 0$ the Fundamental Thin Aerofoil Equation is:
$$\boxed{\boxed{V\left(\alpha-\frac{dz}{dx}\right)+w(x)=0}}$$
The solution is: 
$$\boxed{\gamma(\theta)=2V_{\infty}\left(A_{0}\frac{(1+\cos\theta)}{\sin\theta}+\sum\limits_{n=1}^{\infty}A_{n}\sin n\theta\right)}$$
where the definition of $\theta$ is the same as for the symmetric case:
$$A_{0}=\alpha-\frac{1}{\pi}\int_{0}^{\pi}\frac{dz}{dx}d\theta_{0}$$
$$A_{n}=\frac{2}{\pi}\int_{0}^{\pi} \frac{dz}{dx}\cos n\theta_{0}d\theta_{0}$$
The circulation can be shown to be:
$$\Gamma=\frac{c}{2}\int_{0}^{\pi}\gamma(\theta)\sin\theta~d\theta=cV_\infty\left(\pi A_{0}+\frac{\pi}{2}A_{1}\right)$$
(i.e. only the first two terms of the solution affect the lift)
Applying the Kutta-Joukowski theorem gives:
$$C_{L}=\frac{\rho_{\infty}V_{\infty}\Gamma}{\frac{1}{2}\rho_{\infty}V_{\infty}^{2}c}=\pi(2A_{0}+A_{1})$$
Substituting for the Fourier Coefficients the lift coefficient is:
$$\boxed{\boxed{C_{L}=a_{0}(\alpha-\alpha_{l=0})}}$$
**Which you need to know for the exam**
(Conceptually this means that when $\alpha=0$ there is still some lift generation due to camber)
The offset term $\alpha_{l=0}$ is the zero lift incidence:
$$\alpha_{l=0}=\left(- \frac{1}{\pi}\int_{0}^{\pi}\left(\frac{dz}{dx}\right)(\cos\theta_{0}-1)~d\theta_{0}\right)
$$
**Which will be given in the exam**
