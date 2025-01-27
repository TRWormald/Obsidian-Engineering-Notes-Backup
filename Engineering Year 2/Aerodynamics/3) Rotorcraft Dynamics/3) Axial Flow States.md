There are three main regimes in axial flight:
- Hover
- Climb
- Descent
We have [[2) Fundamentals of Vertical Flight#The Universal Induced Velocity Diagram|previously]] seen the "Universal Induced Velocity Diagram":
![[Pasted image 20250127153610.png|centre]]
Which compares the normalised induced velocity $v$ to the normalised vertical velocity of the craft $V$.
### Axial Flow States
The vertical climb and hover states (and to a certain extent the slow descent) are easily analysed by momentum considerations, as already discussed.
Higher rates of descent can be problematic, both analytically (as the stream tube no longer exists) and in piloting the craft.
Following a total engine failure the helicopter pilot will descend the aircraft into the upper region of the turbulent wake state.
![[Pasted image 20250127154044.png|centre]]
#### The Operating States
A note on sign conventions and notation:
![[Pasted image 20250127154220.png|centre]]
##### The Normal Working State
This is for when the rotor is in climb:
![[Pasted image 20250127154320.png|centre]]
This is for when the rotor is in hover:
![[Pasted image 20250127154354.png]]
##### Vortex Ring State
This is for when the rotor is in very slow descent:
![[Pasted image 20250127154448.png|centre]]
And when it is in slow descent:
![[Pasted image 20250127154525.png|centre]]
##### Turbulent Wake State
This is for when the rotor is in moderate descent:
![[Pasted image 20250127154627.png]]
*Also sometimes known as Ideal Autorotation*
This is for when the rotor is in high descent rate:
![[Pasted image 20250127154727.png]]
##### Windmill Brake State
This is when the rotor is in very high descent rate:
![[Pasted image 20250127154809.png|centre]]
And when it is in extreme descent rate:
![[Pasted image 20250127154833.png|centre]]
### Analysing Axial Flow States
The vertical climb and hover states are easily analysed by momentum considerations - and to a certain extent so can the slow descent states.

However higher rates of descent can be problematic, both in analysis and in piloting the craft.
We can summarise the data we've got in the Universal Induced Velocity Curve.
Note that the dark area is literally a "grey area" as it cannot be solved analytically, and therefore comprises of empirical results obtained by flight tests.
![[Pasted image 20250127155117.png|centre]]
*Note as well that the induced velocity ($y$) and the rotors vertical velocity ($x$) have been non-dimensionalised by the rotor induced velocity in the hover.*
### Helicopters in Autorotation
**It is important to design for low autorotation rates.**
In general (*Note that this very much depends upon rotor diameter and helicopter weight*), helicopters settle upon an autorotational descent rate such that:
$$\boxed{\frac{V}{v_{h}}\approx-1.7}$$
In a steady autorotative descent, $T=$ thrust in hover, so:
$$T=2\rho Av_{h}^{2}$$
The rotor has no net flow through it, so it can be likened to a solid disc of area $A$. Which means that it has *Flat Plate Drag*:
$$D=\frac{1}{2}\rho V^{2}A C_{D}$$
The drag is equal to the thrust as there are no other forces acting upon the rotor, therefore we can equate the equations:
$$\frac{1}{2}\rho V^{2}A C_{D}=2\rho Av_{h}^{2}$$
So:
$$C_{D}=\frac{4}{\left(\frac{V}{v_{h}}\right)^{2}}$$
Now for $V/v_{h}=-1/7$, $C_{D}=1.38$ which is effectively the drag coefficient of a parachute.
#### The Effect of Horizontal Speed on Autorotation
The graph below shows the impact of horizontal speed on the rate of descent during autorotation:
![[Pasted image 20250127160002.png|centre]]
Note how greater levels of horizontal speed results in a greater rate of descent.