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
