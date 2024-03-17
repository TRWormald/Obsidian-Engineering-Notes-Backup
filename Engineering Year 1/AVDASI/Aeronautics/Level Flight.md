**NOTE - The equations in boxes (like this: $\boxed{F=ma}$) may be required to be derived in the exam**
\
There are four main forces that act on an aircraft:
![[Pasted image 20240305105231.png|center|400]]
These are:
$W$ - weight $[N]$ (Level flight so also perpendicular to motion)
$L$ - lift $[N]$ (Perpendicular to the motion)
$T$ - thrust $[N]$ (Assumed to act in flight direction - i.e. there is a small $\alpha$)
$D$ - drag $[N]$ (Opposing the motion)
\
For simplicity we will treat the aircraft as a point mass rather than as a rigid body.
### Lift and Speed in Level Flight
We know that $L=W$ in level flight (as altitude isn't being gained), hence the [[Coefficient of Lift]] can be written as:
$$\boxed{C_L= \frac{L}{\frac{1}{2}\rho V^2S}=\frac{W}{\frac{1}{2}\rho V^2S}=\frac{w}{q}}$$
Where $w$ is the wing loading (See [[Civil Aircraft Design#Wing Loading at Landing and Cruise]]) and $q$ is the dynamic pressure.
The corresponding flight speed $V$ is then:
$$\boxed{V=\sqrt{\frac{W}{\frac{1}{2}\rho S C_L}}=\sqrt{\frac{w}{\frac{1}{2}\rho C_L}}}$$

So the minimum possible level flight speed occurs at $C_{L_{max}}$ (i.e. at stall)
Note that reducing density $\rho$ (i.e. increasing altitude) increases flight speed.
### The Various Air Speeds
The variation of aerodynamic forces with density (altitude) makes performance calculations awkward.
We know that we can estimate the pressure from [[Atmosphere#ISA Density]] where $\sigma$ is the ratio of the density at the current altitude and the density at sea level.
#### True Air Speed (TAS)
True air speed is the speed of the aircraft relative to the air-mass in which it is flying.
So for example if you had a following wind (i.e. it is blowing from behind you) then your true air speed would be your ground speed minus the wind speed:
![[Pasted image 20240305111827.png|center|400]]
#### The Equivalent Air Speed (EAS)
This is the speed $V_E$ at standard sea level density ($\rho_{SL}$ or $\rho_0$) which will give the same aerodynamic loads.
So:
$$\boxed{L=\frac{1}{2}\rho V^2 S C_L=\frac{1}{2}\rho_0V_E^2SC_L}$$
Hence:
$$\boxed{V_E=V\sqrt{\frac{\rho}{\rho_0}}=V\sqrt{\sigma}}$$
We use equivalent air speed because:
- It is useful in calculations
	- We can often work only in terms of sea level conditions and then convert to the required altitude.
- It is useful in flight
	- EAS is close to IAS (Indicated Air Speed) which is read from the airspeed indicator (which uses a pitot tube to measure dynamic pressure and hence find the speed using [[Bernoulli's Equation]]- however it doesn't take into account changes in density and as a result can differ from the TAS)

\
The pilot is most concerned with forces on the aircraft (which depend on $q$ (the dynamic pressure)):
- Stall will **always** occur at the same EAS
- Structural limits are also defined in terms of EAS
\
In most cases:
$$\rho<\rho_0~~~\Rightarrow~~~V_{EAS}<V_{TAS}$$

### Drag on the Aircraft
For an aircraft in equilibrium we know that $T=D$
Therefore we can write the [[Coefficient of Drag]] as:
$$C_D=\frac{D}{\frac{1}{2}\rho V^2 S}=\frac{T}{\frac{1}{2}\rho V^2 S}$$
However the drag of the wings are not the only source of drag for the whole aircraft, there are a multitude of other sources.
\
We can therefore assume that drag consists of:
- A part independent of incidence
	- The zero lift drag coefficient
- A part proportional to $C_L^2$
	- The induced drag plus the part of the form drag that varies with incidence (the drag due to lift)

Hence:
$$\boxed{C_D=C_{D_0}+KC_L^2}$$
Where we can also write it as:
$$C_D=C_{D_0}+\frac{C_L^2}{\pi e AR}$$
Where:
$$K=\frac{1}{\pi e AR}$$
And $e$ is the **Oswald efficiency factor**, with $AR$ being the aspect ratio.
Note that this looks similar to the equation for the drag of a wing, however $e$ has been redefined from the span efficiency factor to the Oswald efficiency factor.

### The Drag Polar
For a general aircraft with a cambered wing, minimum drag no longer necessarily occurs at zero lift. So the drag equation becomes:
$$C_D=C_{D_{min}}+K(C_L-C_{L_0})^2$$
Which is sometimes plotted as $C_L$ vs $C_D$:
![[Screenshot 2024-03-07 150049.png|center|400]]
Where the slope of a line connecting any point on the curve and the origin gives the lift/drag ratio at those conditions.
The maximum lift to drag ratio is found as the point on the curve which a tangent to the curve passing through the origin passes through.
### Expanding on the Drag Equation
If we take the basic lift and drag equations and rearrange them to obtain an equation in velocity V for drag D:
$$C_D=C_{D_0}+KC_L^2$$
$$C_L=\frac{W}{\frac{1}{2}\rho V^2S}$$
So:
$$\boxed{D=AV^2+\frac{B}{V^2}}$$
Where $A$ and $B$ are functions of altitude/density:
$A$ is the zero-lift drag term:
$$\boxed{A=\frac{1}{2}C_{D_0}\rho S}$$
$B$ is the induced drag term:
$$\boxed{B=\frac{KW^2}{\frac{1}{2}\rho S}}$$
Plotting this relationship on a graph gives:
![[Pasted image 20240307151203.png|center|400]]
With the black line representing the total drag.
We can see that:
- At low speeds the induced drag dominates
- At high speeds the profile drag dominates
### Drag at Altitude
Due to the fact that the drag is influenced by the density of the air the greater your altitude the lower the drag you experience at a given speed:
![[Pasted image 20240307151457.png|center|400]]
Note that the stall speed and minimum drag speed ($V_{stall}$ and $V_{MD}$) increase with altitude, whilst the minimum drag remains constant.
Also if plotted in terms of equivalent air speed (EAS) then the variation with altitude disappears.
We can see this in the fact that if we substitute $V_{E}$ and $\rho_0$ into the drag equation:
$$D=A_1V_E^2+\frac{B_1}{V_E^2}$$
Where $A$ and $B$ are now constants:
$$A_1=\frac{1}{2}C_{D_0}\rho_0 S~~~,~~~ B_1=\frac{KW^2}{\frac{1}{2}\rho_0S}$$
As $\rho_0$ is a constant.
Resulting in the graph below:
![[Pasted image 20240307152627.png|center|400]]
### Minimum Drag
The drag is given by:
$$D=L\times\left(\frac{D}{L}\right)=W\times\left(\frac{C_D}{C_L}\right)$$
So the minimum drag occurs at the minimum $C_D/C_L$
$$\frac{C_D}{C_L}=\frac{C_{D_0}+KC_L^2}{C_L}=\frac{C_{D_0}}{C_L}+KC_L \Rightarrow \frac{d(C_D/C_L)}{dC_L}=-\frac{C_{D_0}}{C_L^2}+K$$
At the minimum the differential is equal to zero (i.e. when $C_{D_0}=KC_L^2$)
So:
$$\boxed{C_{D_{min}}=2C_{D_0}=2KC_L^2}$$
$$\boxed{C_{L_{MD}}=\sqrt{C_{D_0}/K}}$$
Hence:
$$\boxed{\frac{C_{D_{min}}}{C_{L_{MD}}}=\left(\frac{C_D}{C_L}\right)_{min}=\frac{2C_{D_0}}{\sqrt{C_{D_0}/K}}=2\sqrt{C_{D_0}/K}}$$
### Minimum Drag Speed
The lift at minimum drag is:
$$C_{L_{MD}}=\sqrt{\frac{C_{D_0}}{K}}$$
Which when substituted into the speed equation gives us the speed we need to be flying at for minimum drag:
$$\boxed{V_{MD}=\left(\frac{2W}{\rho S}\right)^{\frac{1}{2}}\left(\frac{K}{C_{D_0}}\right)^{\frac{1}{4}}}$$
### Effect of Weight on Drag
The following graph shows the relationship between drag and equivalent air speed with differing weight values:
![[Pasted image 20240307154125.png]]
An increase in weight increases the stall speed, and also the induced drag at low speeds, however it results in a very minor increase in drag at higher speeds (i.e. when the total drag is dominated by zero lift drag).
## Summary
The absolute key things to know are:
\
In steady flight:
$$L=W~~~~~~,~~~~~~T=D$$
The equivalent air speed is equal to:
$$V_E=V\sqrt{\frac{\rho}{\rho_0}}=V\sqrt{\sigma}$$
The drag polar is plotted from the equation:
$$ C_D=C_{D_0}+KC_L^2$$
The minimum drag condition is given by:
$$C_{D_{min}}=2C_{D_0}=2KC_L^2$$

