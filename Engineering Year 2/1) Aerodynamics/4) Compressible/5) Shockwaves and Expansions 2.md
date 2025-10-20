## Last Time
We learned that a shockwave is a discontinuity in velocity, temperature, pressure, total pressure, density, and total density, but not in total temperature. It is an adiabatic, but nonisentropic process that reduces flow speed. A normal shock takes the flow irreversibly from supersonic to subsonic.

For a normal shock, a number of equations relating quantities on either side of the shock were derived by considering conservation of mass, momentum, and energy:
$$\boxed{\boxed{M_{2}^{2}=\frac{2+(\gamma-1)M_{1}^{2}}{2\gamma M_{1}^{2}-(\gamma-1)}}}$$
$$\boxed{\begin{matrix} \frac{p_{2}}{p_{1}}=\frac{2\gamma M_{1}^{2}-(\gamma-1)}{\gamma+1}\\ \frac{T_{2}}{T_{1}}=\frac{(2+(\gamma-1)M_{1}^{2})(2\gamma M_{1}^{2}-(\gamma-1))}{(\gamma+1)^{2}M_{1}^{2}}\\ \frac{\rho_{2}}{\rho_{1}}=\frac{(\gamma+1)M_{1}^{2}}{2+(\gamma-1)M_{1}^{2}}\end{matrix}}$$
These equations are tabulated in the normal shock tables. These will be used to answer most questions, using linear interpolation as required.
## Today
We will be looking at:
1) Oblique shocks (i.e. normal shocks at an angle)
2) Detached shocks (a cross between oblique and normal shocks)
### 2D Supersonic Flow - Mach Waves
Lets imagine supersonic flow along a straight surface. Isolated perturbations on the surface generate disturbances in the flow. (these could be scratches, rivets, panel edges etc.).
This results in the following assumptions:
- The surface is straight hence the upstream and downstream conditions are equal
- Infinitesimal pressure wave propagating at Mach Angle $\mu$ 
- Point perturbations generate conical Mach Waves
![[Pasted image 20250228152118.png|centre]]
Note how the Mach Angle $\mu$ is equal to:
$$\mu =\arcsin \frac{1}{M}$$
There is a slightly different situation if the perturbation is a 2D corner where deflection turns into the flow (we get a larger disturbance)
These Mach Waves are the building blocks for larger disturbances.
### Oblique Shocks
For "large" negative deflection angle $\theta$, Mach Waves coalesce to form an oblique shock wave which is a nonisentropic compression wave.
![[Pasted image 20250228155901.png|centre]]
We can use normal shock relations for the normal velocity component:
$$M_{1n}=M_{1}\sin\beta,~~~M_{2n}=M_{2}\sin(\beta-\theta)$$
There is no change in tangential velocities.
Then $M_{2n}$ and ratios $p_{2}/p_{1}$, $T_{2}/T_{1}$, $\rho_{2}/\rho_{1}$ can be tabulated vs. $M_{1n}$.
#### Oblique Shock Angle
![[Pasted image 20250228163356.png|centre]]
Considering the geometry above:
- The inflow velocity $V_{1}$ is split into components $u_{1}$ normal to the shock and $v_{1}$ tangential to the shock.
- Similarly we do the same for the velocity on the other side of the shock.
$$\tan(\beta)=\frac{u_{1}}{v_{1}}$$
$$\tan(\beta-\theta)=\frac{u_{2}}{v_{2}}$$
- So since $v_{2}=v_{1}$, $\beta$ is the angle of the shock to the inflow velocity and $\theta$ is the angle the flow vector has been turned through.
From  continuity:
$$\rho_{1}u_{1}=\rho_{2}u_{2}~~~~\Rightarrow~~~~ \frac{u_{1}}{u_{2}}=\frac{\rho_{2}}{\rho_{1}}$$
With $v_{1}=v_{2}$:
$$\frac{u_{1}/v_{1}}{u_{2}/v_{2}}=\frac{\rho_{2}}{\rho_{1}}~~~~\Rightarrow~~~~\frac{\tan{\beta}}{\tan(\beta-\theta)}=\frac{\rho_{2}}{\rho_{1}}$$
We can then use normal shock relations for flow normal to the shock wave:
$$\frac{\rho_{2}}{\rho_{1}}=\frac{(\gamma+1)M_{1n}^{2}}{2+(\gamma-1)M_{1n}^{2}}=\frac{\tan\beta}{\tan(\beta-\theta)}$$
Which we can rearrange to get:
$$\tan(\beta-\theta)=\frac{(2+(\gamma-1)M_{1n}^{2})\tan\beta}{(\gamma+1)M_{1n}^{2}}$$
And eventually:
$$\tan\theta=\frac{((M_{1}\sin\beta)^{2}-1)\cot\beta}{\left(\frac{\gamma+1}{2}\right)M_{1}^{2}-((M_{1}\sin\beta)^{2}-1)}$$
Which gives us variation of $\beta$ with $\theta$ for upstream Mach Number.
This is usually solved either graphically, or by an iterative scheme, for $\beta$ for a given $\theta$. Tabulated solutions are in the oblique shock tables.
![[Pasted image 20250228173633.png|centre]]![[Pasted image 20250228173855.png|centre]]
### Strong, Weak & Detached Shocks
For a given wedge angle, $\theta$, and onset Mach number, $M_I$ there are two solutions to the equations:
- "Weak" shock occurs in external flows ($\beta_{weak}<\beta_{strong}$)
- "Strong" shock can occur in internal flows with high back pressure
$M_{2}$ is supersonic for weak shocks, except for a small region near $\theta_{max}$.

For $\theta>\theta_{max}$ the pressure rise is too great and the shock "detaches":
- The curved shock "stands off" ahead of a wedge
- Effectively normal near the wedge - with a subsonic region behind the shock
- The curved shock generates vorticity
![[Pasted image 20250228174311.png|centre]]
#### Weak/Strong Shock
If a weak shock exists, and then the downstream pressure is increased (perhaps by a gauze or some other external mechanism), the solution can switch to the strong shock.
Unfortunately, some abuse of terminology takes place - weak shocks are sometimes called "strong" if they have a big change in pressure across them.
### Oblique Shock Relationships
In terms of the normal component of the Mach number:
![[Pasted image 20250228174505.png|centre]]
And in terms of the Mach number:
![[Pasted image 20250228174525.png|centre]]
### Oblique Shock and a Detached Bow Shock for M=2
![[Pasted image 20250228174612.png|centre]]
### Schlieren Images of Cone Shock System
![[Pasted image 20250228174638.png]]
### Revision Objectives
![[Pasted image 20250228174722.png|centre]]
![[Pasted image 20250228174733.png|centre]]
