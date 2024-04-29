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
$$c_{p}=\underbrace{1-4\sin^{2}\theta}_{\text{basic cylinder flow}}- \underbrace{\frac{2\Gamma\sin\theta}{U_{\infty}\pi R}}_{\text{asymmetric swirl}}-\underbrace{\left(\frac{\Gamma}{2U_{\infty}\pi R}\right)^{2}}_{\text{constant swirl}}$$
The three terms of this equation can be seen in the following diagrams:
![[Pasted image 20240429113334.png|center]]
![[Pasted image 20240429113407.png|center]]
![[Pasted image 20240429113516.png|center]]
**Note that if the pressure distribution on a cylinder is symmetrical top to bottom then the lift coefficient is zero.
Whilst if the pressure distribution is symmetrical left to right the drag coefficient is equal to zero.**
This is because the pressure distributions being symmetrical means that there is no net force acting on the object.
### Finding the Stagnation Points
From the equations for the flow velocity we can rearrange both to get:
$$\sin\theta=- \frac{\Gamma}{4U_{\infty}\pi R}$$
This results in three possible cases:
\
**1) There are two symmetric values of $\theta$ :**
This occurs when:
$$\frac{\Gamma}{4U_{\infty}\pi R}<1$$
Which can be seen in the following diagram:
![[Pasted image 20240429114253.png|center|250]]
**2) There is a single stagnation point at -90 degrees:**
This occurs when:
$$\frac{\Gamma}{4U_{\infty}\pi R}=1 ~~~\rightarrow~~~\sin\theta=-1$$
Which can be seen in the following diagram:
![[Pasted image 20240429114509.png|center|250]]
**3) There is a single stagnation point below the cylinder:**
This occurs when:
$$\frac{\Gamma}{4U_{\infty}\pi R}>1$$
Which can be seen in the following diagram:
![[Pasted image 20240429114636.png|center|250]]
