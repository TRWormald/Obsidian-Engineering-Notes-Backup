### Last Time:
For adiabatic flow along a streamline - with no assumption on entropy:
$$h_{0}=h+ \frac{1}{2}V^{2}$$
$$C_{p}T_{0}=C_{p}T + \frac{1}{2}V^{2}$$
$$T_{0}=T\left(1+ \frac{(\gamma-1)M^{2}}{2}\right)$$
Note that the equation above is ADIABATIC, and therefore valid for use across shockwaves.
The we also looked at isentropic and non-isentropic cases, for isentropic flow $T_0$, $p_{0}$, and $\rho_{0}$ are all constant:
$$p_{0}=p\left(1+\frac{\gamma-1}{2}M^{2}\right)^{\frac{\gamma}{\gamma-1}}$$
$$\rho_{0}=\rho\left(1+\frac{\gamma-1}{2}M^{2}\right)^{\frac{1}{\gamma-1}}$$
Note that the two equations above are ISENTROPIC and therefore are not valid across shockwaves - only between them.

**In a non-isentropic (but adiabatic) process only $T_{0}$ is constant e.g. through a shockwave.**
## Shock Waves and Expansions
We will be looking at:
- Normal Shock Waves
	- Extension of sound wave analysis
	- Change in properties through shock
- 2D supersonic flow
	- Mach waves
	- Prandtl-Meyer expansion
	- Oblique shock waves
- Shocks in ducts
	- Intakes and nozzles
	- Supersonic pitot-static
### The Difference Between Soundwaves and Shockwaves
Soundwaves are pressure waves of infinitesimal strength:
![[Pasted image 20250218130332.png|centre]]
Whereas shockwaves are finite pressure waves, and as a result the flow is no longer isentropic:
![[Pasted image 20250218130408.png|centre]]
### What is a Shockwave

> A shockwave is a discontinuity in:
> - Velocity
> - Temperature
> - Pressure
> - Density
> - Total Density

**But not in total temperature - why is this?**
Its because it is an adiabatic process.

A shockwave is the line along which downstream purturbations coalesce when they meet a supersonic upstream zone.
![[Pasted image 20250218130742.png|centre]]
![[Pasted image 20250218130750.png|centre]]
The shockwave is ~60 molecular mean free paths (MFP) wide, so <<< thinner than anything else. We do not need to use models on this scale - the Euler equations are still satisfactory.

Similar to a breaking wave on a beach - what we are interested in is the pressure behind the shock (analogous to the height of the water) related to its Mach number (the speed of the wave hitting the beach). We are not interested in the frothing white region near the front (since its ~60MFP).

A normal shock takes the flow irreversibly from > Mach 1 (supersonic) to < Mach 1 (subsonic).

For oblique shocks the flow is irreversibly reduced in speed with two solutions called strong (always takes flow from supersonic to subsonic) and weak (for most cases the flow is taken from supersonic to slower supersonic, but can be just subsonic near maximum deflection).

**Continuing the Hydraulic Analogy:**
Surface water waves travel at a set speed - the Froude Number (Fr) is the ratio between the speed of the water and the speed of these waves. It is analogous to Mach number.

So if we get some water moving at Fr>1 we should see behaviour similar to shockwaves.
![[Pasted image 20250218131343.png|centre]]
## Normal Shock Waves
![[Pasted image 20250218131448.png|centre]]
As mentioned before, shockwaves are a discontinuity in supersonic flow, due to a "large disturbance".
There is compression and deceleration of the air.

We take a similar approach to a sound wave:
- We have a control volume moving up with the shock
- With station numbers 1&2 up-/down-stream

The shock has finite strength, hence:
- The process is adiabatic - i.e. the changes are too rapid for heat transfer
- The process is non-isentropic - but still inviscid
- Changes in fluid properties $p$, $\rho$, and $u$ are "large".

We apply momentum, continuity, and energy equations to flow through the control volume:
- And rewrite in terms of Mach number $M$ and speed of sound $a$.
