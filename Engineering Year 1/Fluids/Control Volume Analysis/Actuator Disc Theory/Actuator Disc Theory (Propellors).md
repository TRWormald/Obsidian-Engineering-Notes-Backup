A propellor **does work** on the fluid (shaft work) and the increase in momentum gives thrust to the disc:
![[Pasted image 20240316162021.png|center|350]]
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
So the force on the propellor at the cut is equal to the difference in pressure times by the area of the disc being accelerated, note that this is also equal to the force on the air applied by the actuator disc (there is no difference in direction in this case).
Note how we now no longer have a constant pressure all the way around the boundary so we no longer have a zero term.
\
Using our previous equation:
$$(p_{3}-p_{2})=\rho V_d(V_{4}-V_{1})$$
We can then eliminate $p_{3}-p_{2}$ using our derivation using Bernoulli's equation:
$$V_{d}= \frac{1}{2}(V_{1}+V_{4})$$
\
For a stationary rotor (a fixed fan or helicopter in hover):
$$V_{1}=0 ~~~~\Rightarrow~~~~V_{4}+2V_d$$
$$F=\rho A_{d}V_{d}(2V_d-0)=2\rho A_{d}V_{d}^{2}$$
$$V_{d}=\sqrt{\frac{F}{2\rho A_{d}}}$$
And as a result we can relate the required force for the disc velocity.
\
For a propellor with a forward velocity $v$ into still air, and a final air velocity relative to the disc of $V_4$ we have (using the Galilean transformation):
$$V_{1}=v~~~~\Rightarrow~~~~V_{d} = \frac{1}{2}(V_{4}+v)$$
Hence:
$$F=\rho A_{d}V_{d}(V_{4}-v)= \frac{1}{2}\rho A_{d}(V_{4}^{2}-v^{2})$$
We can then rewrite this as:
$$F=2\rho A_{d}v^{2}a(1+a)$$
Where $a$ is the inflow factor and is equal to:
$$a=\frac{V_{d}-v}{v}$$
##### Power supplied to the Actuator Disc
The power supplied to the disc to produce the thrust (i.e. the ideal power input) is:
$$\begin{align*}
FV_{d}&= \rho Q (V_{4}-V_{1})V_{d}\\&= \frac{1}{2}\rho Q(V_4-V_{1})(V_4+V_{1})\\&= \frac{1}{2}\rho Q(V_4-V_{1})(V_4-V_{1})+\rho Q(V_4-V_{1})V_1
\end{align*}$$
\
So for a hovering rotor:
$$FV_{d}= F\sqrt{\frac{F}{2\rho A_{d}}}=\frac{F^{\frac{3}{2}}}{\sqrt{2\rho A_{d}}}$$
\
However the power put into the air (effective power output) is given by:
$$FV_{1}=\rho Q (V_{4}-V_{1})V_{1}$$
So for forward flight at a speed $v$:
$$Fv=\rho Q (V_{4}-v)v$$
\
The propulsive efficiency (for forward flight) is the ratio of power input and output:
$$\eta=\frac{\rho Q(V_{4}-V_{1})}{\rho Q(V_{4}-V_{1})}\frac{V_{1}}{\frac{1}{2}(V_{4}-V_{1})+V_{1}}=\frac{2V_{1}}{V_{4}+V_{1}}$$
