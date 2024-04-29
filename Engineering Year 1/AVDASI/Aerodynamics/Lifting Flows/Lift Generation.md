To evaluate lift it is easiest to work it out from first principles, we are effectively evaluating the forces on an element of surface formed by and angle $\delta\theta$ at $\theta$ from $x$:
![[Pasted image 20240429115004.png|center|250]]
So the pressure $p(\theta)$ is exerted over an area $R\delta\theta=\delta s$, however the force exerted contains both lift and drag components:
![[Pasted image 20240429115228.png|center|300]]
So resolving gives us that the lift is equal to:
$$\delta L =-p(\theta)\cdot R \delta\theta\cdot\sin\theta$$
Hence integrating this around the circle gives:
$$\begin{align*}
L&= -\int_{0}^{2\pi}p(\theta)R\sin\theta\cdot d\theta\\
&= -\int_{0}^{2\pi}(p(\theta)-p_{\infty}+p_{\infty})R\sin\theta\cdot d\theta\\\\
&= -\int_{0}^{\infty}(p(\theta)-p_{\infty})R\sin\theta\cdot d\theta-\int_{0}^{2\pi}p_{\infty}R\sin\theta\cdot d\theta
\end{align*}$$

