The only mechanisms we have for transmitting forces (and hence lift) to a body is via pressure and shear stress on the body surface.
The potential flow over a rotating cylinder will give us some insight into how lift is generated.
We will form our model using the doublet and uniform flow from [[Flow over a Cylinder]] and add to it a [[Point Vortex Flow]] at the centre:
![[Pasted image 20240429111301.png|center]]
This results in:
![[Pasted image 20240429111320.png|center|250]]
The velocity conditions at the surface are now very interesting, if the fluid was truly inviscid the rotation of the body would not change the flow - however this is not the case here; the speed on the surface equals the inviscid speed plus the true viscous speed.
### Calculating the Velocities and the Pressure Coefficient
Previously we found that:
$$\begin{align*}
u&= 2U_{\infty}\sin^{2}\theta\\
v&=-2U_{\infty}\cos\theta\sin\theta 
\end{align*}$$
The velocities for vortex flow are:
$$\begin{align*}
u&= \frac{\Gamma}{2\pi} \frac{y}{x^{2}+y^{2}}\\
&=\frac{\Gamma}{2\pi} \frac{R\sin\theta}{R^{2}}\\
&= \frac{\Gamma\sin\theta}{2\pi R}\\
&\text{And similarly:}   \\
v&=\frac{-\Gamma\cos\theta}{2\pi R}
\end{align*}$$
Hence adding the components:
$$u=2U_{\infty}\sin^{2}\theta+\frac{\Gamma\sin\theta}{2\pi R}$$
$$v=2U_{\infty}\cos\theta\sin\theta-\frac{\Gamma\cos\theta}{2\pi R}$$
We know that the [[The Coefficient of Pressure - From Bernoulli's Equation|coefficient of pressure]] can be found using:
$$C_{p}=1-\frac{V^{2}}{U_{\infty}^{2}}$$
So:
$$c_{p}=1-\frac{u^{2}+v^{2}}{U_{\infty}^{2}}$$
Which when substituted and simplified fully gives:
$$c_{p}=\underbrace{1-4\sin^{2}\theta}_{\text{basic cylinder}\par\text{}}- \frac{2\Gamma\sin\theta}{U_{\infty}\pi R}-\left(\frac{\Gamma}{2U_{\infty}\pi R}\right)^{2}$$