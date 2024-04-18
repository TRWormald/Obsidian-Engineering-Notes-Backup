### Pipe Flow Losses - The Effect of Viscosity
Pressure loss due to friction in a straight pipe can be accurately calculated in terms of length $L$, diameter $D$, and average velocity (or centreline velocity) $V$, via the Darcy-Weisbach equation:
$$\Delta p_{loss}=f_{D} \frac{{L}}{{D}} \frac{1}{2}\rho V^{2}$$
Where $f_{D}$ is the friction factor - which is plotted on a Moody Diagram as a function of Reynolds Number, $Re_{D}=\frac{VD}{v}$ and relative roughness $\frac{\varepsilon}{D}$.
We can then apply this to [[Bernoulli's Equation]] to represent the change in pressure as a result of friction:
$$p_{1}+ \frac{1}{2}\rho V_{1}^{2}+\rho gz_{1}=p_{2}+ \frac{1}{2}\rho V^{2}_{2}+\rho g z_{2}+\Delta p_{loss}$$
If we solve this for the pressure loss:
$$\Delta p +\rho g \Delta z=f_{D} \frac{L}{D} \frac{1}{2}\rho V^{2}$$
As the velocity at 1 and 2 must be the same, and therefore the dynamic pressures cancel out.
We can also represent this using an 'equivalent height' or pressure head in the fluid:
$$\Delta p+\rho g\Delta z=\rho g \Delta h$$
Where $\Delta h$ is the change in height relative to a fixed point, allowing us to show how the viscous effects have changed.
This leads into the idea of the 'grade line', GL.
For inviscid flow we get the following:
![[Pasted image 20240417093641.png]]
Note how there is the energy grade line which is in line with the top of the fluid in the tank (this is equal to the sum of static, hydrostatic, and dynamic pressures) and also the **hydraulic grade line** which varies from the energy GL as it is only the sum of the static and hydrostatic pressures, resulting in a difference of $\frac{1}{2}\rho V^{2}$.
\
If we no longer assume that the fluid is inviscid we get the following grade line:
![[Pasted image 20240417092931.png|center]]
The grade line decreases along the length as the viscous losses increase with distance.
Note the presence of the $\Delta h_{ent}$ (sometimes called 'minor losses'), this is the change in height of the grade line due to the viscous effects of the entry to the pipe along with the losses associated with going from a static fluid to one with velocity.
As we move along the pipe we see a greater decrease in height $\Delta h$ which is a result of the viscous effects. 
### Finding the Friction Factor
This year we will be given a single value or a formula to calculate it in the question.
\
For laminar flow in pipes:
$$f_{D}=64 Re_{D}^{-1}$$
For turbulent flow in smooth pipes:
$$f_{D}\approx0.316 Re_{D}^{-0.25}$$
In general cases, if the Reynold's Number is less than two thousand ($Re_{D}<2000$) then the flow is laminar, and if it is greater than or equal to two thousand ($Re_{D}\ge 2000$) then the flow is turbulent.
\
Note that for non circular pipes $D$ is replaced by the hydraulic diameter $D=4\cdot \frac{\text{Area}}{\text{Diameter}}$.
### Minor Losses
These are the losses associated with junctions, expansions, contractions, and bends - despite their name they can be very large.
They are defined in terns of the local dynamic pressure and a loss coefficient $k$:
$$\boxed{\text{Loss Coefficient}=k=  \frac{{\Delta p_{loss}}}{\frac{1}{2}\rho V^{2}}}$$
If there is more than one local dynamic pressure, then use the highest value.
The values of loss coefficient are found from testing, however we can derive some from control volume analysis.
Below we can see some of the losses experienced in a pipe system:
![[Pasted image 20240417105527.png|center|400]]
#### Example 1 - Loss at an abrupt enlargement
**Assumptions -** Straight streamlines at inlet and outlet, so uniform conditions at 1 and 2. The flow is steady, frictionless, and incompressible. We also assume that there is low curvature at the enlargement and that there is low velocity flow in the recirculation regions.
![[Pasted image 20240417190352.png|center|450]]
From our assumptions we know that:
$$p_{C}=p_{B}\approx p_{1}$$
**Applying the continuity equation:**
$$Q=A_{1}V_{1}=A_{2}V_{2}$$
**Applying Bernoulli's Equation Between 1 and 2:**
$$p_{1}+ \frac{1}{2}\rho V_{1}^{2}=p_{2}+ \frac{1}{2}\rho V^{2}_{2}+\Delta p_{loss}$$
**Using the steady flow momentum equation in the x-direction:**
$$p_{1}A_{1}+p_{1}(A_{2}-A_{1})-p_{2}A_{2}=\rho Q(V_{2}-V_{1})$$
$$\begin{align*}
\Rightarrow (p_{1}-p_{2})A_{2}&= \rho Q(V_{2}-V_{1})\\
&= \rho V_{1}A_{1}\left(V_{1} \frac{A_{1}}{A_{2}}-V_{1}\right)\\
\end{align*}$$
$$\Rightarrow(p_{1}-p_{2})=\rho V_{1}^{2} \frac{A_{1}}{A_{2}}\left(\frac{A_{1}}{A_{2}}-1\right)$$
**Substituting this into Bernoulli's Equation solved for $\Delta p_{loss}$ we get:**
$$\begin{align*}
\Delta p_{loss}&= \rho V_{1}^{2} \frac{A_{1}}{A_{2}}\left(\frac{A_{1}}{A_{2}}-1\right)+ \frac{1}{2}\rho V_{1}^{2}\left(1-\left(\frac{A_{1}}{A_{2}}\right)^{2}\right)\\
&= \frac{1}{2}\rho V_{1}^{2}\left[2 \frac{A_{1}}{A_{2}}\left(\frac{A_{1}}{A_{2}}-1\right)\right]
\end{align*}$$

#### Example 2 - Loss at an abrupt contraction
