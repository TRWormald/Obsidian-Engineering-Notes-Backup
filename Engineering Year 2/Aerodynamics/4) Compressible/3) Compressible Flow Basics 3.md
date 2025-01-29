### Isentropic Relationships Between Pressure, Density and Speed
We can make the additional assumption of an isentropic process:
$$\frac{p_{1}}{p_{2}}=\left(\frac{\rho_{2}}{\rho_{1}}\right)^{\gamma}=\left(\frac{T_{2}}{T_{1}}\right)^{\frac{{\gamma}}{\gamma-1}}$$
Which we can substitute into the total temperature equation to give:
$$p_{0}=p\left\{1+ \frac{\gamma-1}{2}M^{2}\right\}^ \frac{{\gamma}}{\gamma-1}$$
$$\rho_{0}=\rho\left\{1+ \frac{\gamma-1}{2}M^{2}\right\}^ \frac{{1}}{\gamma-1}$$
*The ratios $T_{0}/T$, $p_{0}/p$, and $\rho_{0}/\rho$ are given in compressible flow tables, so we use tables to solve most questions rather than the equations.*
### Flow Tables
![[Pasted image 20250129102434.png|centre]]
### Compressible Flow Relations
The graph below shows the relationship between flow parameters and Mach number:
![[Pasted image 20250129102543.png|centre]]
## Choked Flow
### Recall - 1D Euler Equation
Recalling from earlier that we simplified the Navier-Stokes equations to obtain the steady Euler equations, and hence obtained that along a streamline:
$$dp=-\rho V~dV$$
### 1D Isentropic Duct Flow (or along a streamline)
Let's model flow in a duct with slowly changing area $A$, therefore:
- The angle between streamlines is small
- The impact of the boundary layer is small
Flow is therefore inviscid and effectively one dimensional - so let's assume inviscid, steady flow, with negligible height variation.

The momentum equation is the 1D Euler Equation from earlier:
$$dp=-\rho V~dV~~~~\Rightarrow~~~~\frac{dp}{\rho}+V~dV=0$$
And the continuity equation is given by the derivative of mass flow:
$$\dot{m}=\rho AV~~~ \Rightarrow~~~ \frac{dV}{V}+ \frac{dA}{A}+ \frac{d\rho}{\rho}=0$$
From which we can obtain:
$$\frac{dV}{V}+ \frac{dA}{A}- \frac{V^{2}}{a^{2}} \frac{dV}{V}=0$$
### Area Velocity Variation (Adiabatic Flow)
We can take the equation:
$$\frac{dV}{V}+ \frac{dA}{A}- \frac{V^{2}}{a^{2}} \frac{dV}{V}=0$$
And substitute to get:
$$\frac{dA}{A}=(M^{2}-1) \frac{dV}{V}$$
*Note that this only applies for adiabatic flow.*
Which is a direct relation between area variation and velocity variation.
We can now introduce the element of length along the duct or streamline $dx$:
$$(M^{2}-1) \frac{1}{V} \frac{dV}{dx}=\frac{1}{A} \frac{dA}{dx}$$
Consider an accelerating flow $dV/dx>0$:
- M<1 then $dA/dx<0$ therefore a converging duct
- M>1 then $dA/dx>0$ therefore a diverging duct
- M=1 then $dA/dx=0$ therefore minimum area (i.e. a throat)
### Area Ratio
Sonic duct flow can only occur at a throat (i.e. where the area is a local minimum)
When $M=1$ here, this area is also the "critical" area $A^{*}$.
The critical area is often used as a reference area in compressible flow.
Use isentropic equations to relate local area $A$ and Mach number to $A^{*}$:
$$\rho A V=\rho^{*}A^{*}V^{*}$$
$$V=Ma\Rightarrow V^{*}=a^{*}$$
Hence:
$$\rho AMa=\rho^{*}A^{*}a^{*}$$
Leading to:
$$\frac{A}{A^{*}}=\frac{\rho^{*}}{\rho} \frac{a^{*}}{a} \frac{1}{M}$$
Then using the relations:
$$\frac{\rho^{*}}{\rho}=\frac{\rho^{*}}{\rho_{0}}\frac{\rho_{0}}{\rho}$$
And a similar one for the speed of sound, we can obtain:
$$\frac{A}{A^{*}}=\frac{1}{M}\left\{ \frac{2}{\gamma+1}\left(1+ \frac{\gamma-1}{2} M^{2}\right)\right\}^{\frac{\gamma+1}{2(\gamma-1)}}$$
Which has two solutions, M>1 and M<1.
![[Pasted image 20250129104331.png|centre]]
### The Laval Nozzle