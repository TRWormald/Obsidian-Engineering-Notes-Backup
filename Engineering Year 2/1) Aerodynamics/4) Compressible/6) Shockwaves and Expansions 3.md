### Mach Waves
We've previously learnt that Mach Waves are the building blocks for larger disturbances.
We start with supersonic flow along a straight surface, and then introduce an isolated perturbation on the surface to generate disturbances in the flow.
There as several assumptions that we make:
- Straight surface, hence the upstream and downstream conditions are equal
- Infinitesimal pressure wave propagating at Mach Angle $\mu$ 
- Point perturbations generate conical 3D Mach waves
![[Pasted image 20250314114745.png|centre]]
### Small Flow Deflection
Now lets consider a case where the surface (and hence the flow) are deflected by a small angle $d\theta$
![[Pasted image 20250314114908.png|centre]]
- Obviously there is no effect of the deflection felt upstream due to the fluid traveling faster than the speed of sound.
- In 2D flow the flow properties are constant along the wave, therefore there is no pressure gradient parallel (tangential) to the wave.
- There is no change in tangential velocity component across the wave, therefore we only need to deal with the changes in the normal velocity component, just like in oblique shock wave analysis.

The image below shows how when the inflow velocity is greater than Mach 1 , we actually get an acceleration:
![[Pasted image 20250314115222.png|centre]]
$$\boxed{\frac{dV}{d\theta}=\frac{V}{\sqrt{M^2-1}}}$$
![[Pasted image 20250314115430.png|centre]]
We can then rearrange using the steps above to get:
$$\boxed{\frac{dp}{d\theta}=\frac{-\gamma M^{2}}{\sqrt{M^{2}-1}}p}$$
Which is negative for M>1 therefore an expansion results in a pressure drop. We need to integrate for finite deflection angle (Prandtl-Meyer expansion).
### Prandtl-Meyer Expansion
Consider a large positive deflection angle $\theta$:
![[Pasted image 20250314115654.png|centre]]
The flow expands through a series of infinitesimal expansions $d\theta$, resulting in an isentropic "expansion fan".
To see the impact of this deflection on the flow velocity we need to integrate the equation:
$$\boxed{\frac{dV}{d\theta}=\frac{V}{\sqrt{M^2-1}}}$$
From 0 to the deflection angle $\theta$.
This results in:
$$\boxed{\boxed{\theta=v(M_{2})-v(M_{1})}}$$
Where $v$ is the "Prandtl Meyer Function (or angle)", which is equal to:
![[Pasted image 20250314120010.png|centre]]
**Which we won't be using :)**
Instead we will use tables and linear interpolation.

The Prandtl-Meyer angle $v$ is the fictitious angle through which sonic flow (i.e. at a Mach number of 1) would have to be turned to accelerate to give downstream Mach Number $M$. 
It is a function of downstream Mach Number only:
$$v(M)\equiv\theta (M_{1}=1,M_{2}=M)$$
For $M_{1}>1$, $\theta(M_{1}, M_{2})$ is the difference of expansion angles for $M_1$ and $M_2$.
![[Pasted image 20250314122635.png]]
![[Pasted image 20250314123638.png|centre]]
Given the upstream Mach number $M_1$ and the expansion angle, how do we find the downstream Mach number $M_{2}$
- If we know $\theta$ we can calculate $v(M_{1})$
- Therefore we must find $M_{2}$ such that $v(M_{2})=\theta+v(M_{1})$
- As long as the flow remains isentropic the expansion path can be ignored.
![[Pasted image 20250314123908.png|centre]]
### The Double Wedge Aerofoil
![[Pasted image 20250314125344.png]]
In the image we can see where the flow is accelerating.
![[Pasted image 20250314125413.png|centre]]
### Wave Reflections
>Mach Waves (expansion and compression) and oblique shock waves are reflected at flow boundaries
>  -  Flow tangency for solid boundaries
>  -  Pressure equilibrium for jet boundaries

For solid walls the type of reflection depends on the wall inclination (e.g. oblique shock can be reflected as a shock, as an expansion fan, or be absorbed.)
#### Solid Surface Reflections
![[Pasted image 20250314141159.png|centre]]
#### Fluid Boundary Reflections
For a fluid boundary (i.e. the edge of a jet) pressure equilibrium gives alternating compression and expansion waves, resulting in:
- Shock diamonds
- Viscosity smears our effect
![[Pasted image 20250314141621.png|centre]]
### Shocks in Convergent-Divergent Nozzles
![[Pasted image 20250314141646.png|centre]]
### Supersonic Intakes
Conventional engines require subsonic flow at the fan face (<0.4M)
This implies the shock system at supersonic speeds, the shock provides compression - but at a price (the shock means compression, and pressure rise (and hence speed drop), but the total pressure drops and that means that the available mechanical energy drops, and hence the thrust).
**The Basic Pitot Intake:**
![[Pasted image 20250314141922.png|centre]]
This has a **Normal Shock** at the lip, and has 2-stage compression.
It is, however, inefficient above 1.5M

**The External Compression Intake**
![[Pasted image 20250314142109.png|centre]]
This has an **External Oblique Shock**
and then a **Normal Shock** at the lip. So we have 3 stage compression.
This results in a reduced pressure loss, and variable geometry is desirable.

## Revision Objectives
![[Pasted image 20250314142245.png|centre]]
![[Pasted image 20250314142258.png|centre]]
