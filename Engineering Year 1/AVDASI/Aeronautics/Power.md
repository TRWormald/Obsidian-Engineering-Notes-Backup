### Power Required in Steady Level Flight
For the power produced is equal to the thrust times the velocity, and as we know that for level flight (see [[Level Flight#Summary]]) the thrust is equal to the drag so:
$$P=TV=DV$$
Therefore, using the equation for drag on an aircraft in steady level flight (see [[Level Flight#Expanding on the Drag Equation]]):
$$ P=\left(AV^2+\frac{B}{V^2}\right)V=AV^3+\frac{B}{V}$$
So with the equation above we can plot a graph of Required Power against True Air Speed at sea level:
![[Power Required vs TAS Polar (For Steady Level Flight).png|center|400]]
And we can see that it is very similar to the drag diagrams we saw in [[Level Flight]], with power required increasing exponentially with speed.
### Power Required with Altitude
As we increase altitude and hence decrease the air density term in our drag equation the power plot changes:
![[Power Required against TAS Polar (Variation with Altitude & Steady Level Flight).png|center|400]]
We note that as we increase our altitude that the graph shifts to the right and that at higher altitudes the amount of power required for the same speed is much lower, especially at high speeds.
The stall and minimum power speeds ($V_{MP}$ and $V_{stall}$) increase with altitude along with the actual minimum power.
Note that if plotted in terms of $P\sqrt{\sigma}$ and $V_{EAS}$ then the variation with altitude disappears.
#### Power Equation in Terms of $V_{EAS}$ and $\sigma$
If we substitute equivalent air speed $V_E$ and (constant) density $\rho_0$ into the power equations we get:
$$P\sqrt{\sigma}=V_E\left(A_1V_E^2+\frac{B_1}{V_E^2}\right)$$
Where $A_1$ and $B_1$ are constants (as defined previously in [[Level Flight#Drag at Altitude]]):
$$A_1=\frac{1}{2}C_{D_0}\rho_0 S~~~,~~~ B_1=\frac{KW^2}{\frac{1}{2}\rho_0S}$$
If we plot **Power** against Equivalent Air Speed:
![[Pasted image 20240307162652.png|center|400]]
However if we plot Power times the square root of sigma:
![[Pasted image 20240307162738.png|center|400]]
We again get a single curve where there is no variation with altitude.
### Minimum Power Required
Using the facts that weight is equal to lift for steady level flight:
$$P=DV=W\times\left(\frac{D}{L}\right)\times V=W\left(\frac{C_D}{C_L}\right)\sqrt{\frac{W}{\frac{1}{2}\rho SC_L}}$$
Therefore:
$$P\propto \frac{C_D}{C_L^{3/2}}$$
Therefore we need to find the minimum $C_D/C_L^{3/2}$:
$$\frac{C_D}{C_L^{3/2}}=\frac{C_{D_0}+KC_L^2}{C_L^{3/2}}=\frac{C_{D_0}}{C_L^{3/2}}\Rightarrow\frac{d(C_D/C_L^{3/2})}{dC_L}=-\frac{3}{2}\frac{C_{D_0}}{C_L^{5/2}}+\frac{1}{2}\frac{K}{C_L^{1/2}}$$
So at the minimum point:
$$3C_{D_0}=KC_L^2$$
Hence the coefficients of lift and drag at minimum power are:
$$\boxed{C_{D_{MP}}=4C_{D_0}}$$
$$\boxed{C_{L_{MP}}=\sqrt{3C_{D_0}/K}}$$
If we substitute the latter into the speed equation we can calculate the minimum power required speed:
$$\boxed{V_{MP}=\left(\frac{2W}{\rho S}\right)^{\frac{1}{2}}\left(\frac{K}{3C_{D_0}}\right)^{\frac{1}{4}}}$$
If we compare again to the [[Power#Power Required in Steady Level Flight]] graph:
![[Screenshot 2024-03-07 164947.png|center|500]]

### Minimum Power vs Minimum Drag
We can compare minimum power required and the velocity for minimum drag. The minimum power required occurs at a lower speed than for minimum drag:
$$\frac{V_{MP}}{V_{MD}}=\frac{\left(\frac{2W}{\rho S}\right)^{\frac{1}{2}}\left(\frac{K}{3C_{D_0}}\right)^{\frac{1}{4}}}{\left(\frac{2W}{\rho S}\right)^{\frac{1}{2}}\left(\frac{K}{C_{D_0}}\right)^{\frac{1}{4}}}=\frac{1}{3^{\frac{1}{4}}}=0.76$$
This means that the lift coefficient for minimum power must be greater than the one for minimum drag:
$$C_{L_{MP}}=\sqrt{\frac{3C_{D_0}}{K}}~~~~~~vs~~~~~~C_{L_{MD}}=\sqrt{\frac{C_{D_0}}{K}}$$
