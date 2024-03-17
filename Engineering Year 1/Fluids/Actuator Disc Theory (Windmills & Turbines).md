Fluid **does work** on the turbine (shaft work) and the decrease in momentum gives thrust to the disk:
![[Pasted image 20240317130400.png|center|350]]
We make the assumptions that the flow is **frictionless** and **incompressible**, but the flow is also **steady** and **one dimensional** (and as a result we neglect the rotation and variation across the disc radius).
We assume that the disc is infinitely thin, so $A_{2}=A_{3}=A_{d}$ and that the velocity of the disc over the propellor is constant, so $V_{2}=V_{3}=V_{d}$.
We also assume that $p=p_{a}$ at all points on the slipstream boundary, at 1 and at 4.
\
##### Continuity
We can apply our continuity equation:
$$Q=V_{d}A_{d}$$
Where $Q$ is the volume flow rate, $V_{d}$ is the velocity of the disc, and $A_{d}$ is the area of the disc.
##### Applying Bernoulli's Equation
For the Control Volume between 1 and 2:
$$p_{1}+ \frac{1}{2}\rho V_{1}^{2}=p_{2}+ \frac{1}{2}\rho V_{d}^{2}$$
For the Control Volume between 3 and 4:
$$p_{3}+ \frac{1}{2}\rho V_{d}^{2}=p_{4}+ \frac{1}{2}\rho V_{4}^{2}$$
\
We know that $p_{1}=p_{4}=p_{a}$, so:
$$p_{3}-p_{2}= \frac{1}{2}\rho \left(V_{4}^{2}-V_{1}^{2}\right)$$
##### Applying Steady Flow Momentum
[[Control Volume Analysis Introduction#Conservation of Steady Flow Linear Momentum for a Control Volume|See this section on conservation of momentum in a Control Volume for more information.]]
For the control volume between 1 and 4:
$$0+F=\rho Q(V_{4}-V_{1})$$
Where $F$ is the force at the cut, and the $0$ is the representation of the lack of net force due to pressure.
\
For the control volume between 2 and 3:
$$(p_{2}-p_{3})A_{d}+F=\rho Q(V_{d}-V_{d})=0$$
$$F=(p_{3}-p_{2})A_{d}$$
**This is identical to the derivation in [[Actuator Disc Theory (Propellors)]], however the force is now in the opposite direction as $p_3$ is smaller than $p_2$.**
\
Using our previous equation:
$$(p_{3}-p_{2})=\rho V_d(V_{4}-V_{1})$$
We can then eliminate $p_{3}-p_{2}$ using our derivation using Bernoulli's equation:
$$V_{d}= \frac{1}{2}(V_{1}+V_{4})$$
##### Power Drawn by the Disc
The power drawn from the air by the disc is:
$$\begin{align*}
P_{disc}=-FV_{d}&= -\rho Q(V_{4}-V_{1})V_{d}\\&= \rho A_{d}V_{d}(V_{1}-V_{4})V_{d}\\&= \frac{1}{4}\rho A_{d}(V_{4}+V_{1})(V_{1}^{2}-V_{4}^{2})
\end{align*}$$
Calculating efficiency is slightly harder than with propellors and as such we have to consider the wind passing through the disc area as if the disc were not present (i.e. no change in area or velocity):
$$P_{wind}=\frac{1}{2}$$