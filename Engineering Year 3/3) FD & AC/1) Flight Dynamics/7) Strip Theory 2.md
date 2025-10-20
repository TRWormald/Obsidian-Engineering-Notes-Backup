### The Effect of Control Surface Deflection
Control surface deflection can give non-zero lift, even when the primary surface is still at zero incidence. 
![[Pasted image 20251003111439.png|centre]]
Note how:
1) The lower set of curves above for the lift coefficient show successive $C_L$ increases at $\alpha=0$ as the surface deflection $\delta$ increases.
2) The upper set of curves show successively greater negative hinge moments as $\delta$ increases, again at $\alpha=0$
3) Over the range of incidences $-5\degree<\alpha<5\degree$, both sets of curves appear linear with $\alpha$. What we need to do in addition is cross plot from the lower set, keeping $\alpha$ constant at $0\degree$ and see how the section lift is influenced by $\delta$ alone.
![[Pasted image 20251003111751.png|centre|400]]
The graph above shows the change in lift coefficient for a specific $\delta$ angle for a flap. The lines show the fraction of the total chord that the flap's chord is.
These variations show that for $\delta<15\degree$ or so, the change in lift coefficient due to relatively small control surface deflections appears linear and is proportional to $\delta$.

The more general approximation, allowing for aileron, elevator, and rudder, and using the general deflection angle $\delta$ to represent any one of $\xi,~\eta,~\text{and}~\zeta$, would show the following relationships between $\alpha$, $\delta$, and $C_L$.
![[Pasted image 20251003112256.png|centre|400]]
Within a reasonable range of both $\alpha$ and $\delta$ the slope is assumed to be constant at:
$$\huge{a_{1}=\left.\frac{\partial C_{L}}{\partial \alpha}\right|_{\delta=\text{constant}}}$$
We allow for initial aerofoil camber in the graph above too, by showing that $a_{0}\ne 0$ when both $\alpha$ and $\delta$ are zero.

### The Value of $\large{a_{1}}$
We can define the lift coefficient as:
$$\huge{C_{l}=a_{0}+a_{1}\alpha+a_{2}\delta}$$
Theoretical thin-aerofoil theory predicts that for a 2D wing, with a full-span control surface the value of $a_{1}$ is:
$$\huge{a_{1}=2\pi~~\text{for angles measured in radians}}$$
### Functions That Vary Across the Span
Sometimes it is convenient to make one or more of the coefficients variable. Take a simple tapered wing as shown below:
![[Pasted image 20251003113125.png|centre]]
One approximation to the spanwise distribution of lift, is to consider the product $a_{1}\alpha$ to give a reasonable variation of the product without trying to portray either factor accurately.
We might be able to estimate components of $\alpha$ other than due to downwash, whereas the spanwise variation of the loss in incidence due to downwash would be more difficult to describe.
In principle, $a_{1}$ is almost constant but we could shape it by using a function such as the one below:
$$\huge{a_{1}(\eta)=a_{10}(1-\eta^{2})^{\frac{1}{2}}}$$
![[Pasted image 20251003113357.png|centre]]
![[Pasted image 20251003113408.png|centre]]
### A Lift-Curve Slope for the Whole Wing
![[Pasted image 20251003113436.png|centre]]
### Other Aerodynamic Coefficients
The zero-lift angle is taken as $\alpha_{0}$, this is usually a negative value which indicates that the section would have to be rotated slightly nose-down to produce no lift.
$$\begin{align*}
C_{l}&= a_{1}(\alpha-\alpha_{0})\\
&= -a_{1}\alpha_{0}+a_{1}\alpha 
\end{align*}$$
Which gives:
$$a_{0}=-a_{1}\alpha_{0}$$
Which is probably a positive number.
![[Pasted image 20251003113726.png|centre]]
### Strip Theory Application
1) Define geometry and define "strip" boundaries
2) Develop an expression for dForce in general terms:
	pressure $\times$ area $\times$ coefficient
3) If necessary, develop a dMoment (with the required moment arm)
4) Determine spanwise functions as needed
5) Express the full integral with its proper limits and integrate
6) Differentiate to get an "aerodynamic derivative"

>Tips:
>- Work from the basics
>- Do not try to remember the developed expressions
>- Explain the assumptions you make and the approximations you use
>- Use neat diagrams

### Rolling Power
Lets now look at the steady-state response to an aileron deflection. This implies pure roll, i.e. no other responses but rotation around the x-axis. This becomes unreal after any significant bank angle develops, because then sideslip would develop also, and this would generate a yaw rate because of its pressures on the fin; then we would have three active variables.
In this example we will ignore all other responses and seek the roll rate $p$ that can be achieved by an aileron deflection of $\xi$.
#### Rolling Moment due to Ailerons
![[Pasted image 20251003114736.png|centre|400]]
The local lift coefficient on the strip can have the components:
$$\huge{C_{l}=a_{0}+a_{1}\alpha+a_{2}\xi}$$
And thus the expression for the differential lift on the strip becomes:
$$\huge{\text{dLift}=\frac{1}{2}\rho U^{2}\cdot c(y)\cdot dy\cdot C_{l}}$$
Differential rolling moment can be expressed as:
$$\huge{dL=-y\text{ dLift}}$$
Where the negative sign is necessary to display the fact that positive $\xi$ produces a negative rolling moment.

Just before the aircraft begins to roll, the only unbalancing components of the lift from $C_{l}$ which can produce a rolling moment are those from $\xi$.
Even the effect of camber ($a_{0}$) will be symmetric on the two sides and can therefore be left out of the lift expression.
As both $\xi$ and $y$ change sign from side to side we can integrate double the moment on one side:
$$\huge{L(\xi)=-2\int_{y_{i}}^{y_{0}} \frac{1}{2}\rho U^{2}~ y~c(y)~a_{2}(y) \xi \cdot dy}$$
