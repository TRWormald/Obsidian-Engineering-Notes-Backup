Turbines extract work from the hot high pressure combustion products to drive the compressor. Cycle calculations define an overall temperature drop & pressure drop at a given level of isentropic efficiency.
> The rotational speed must be equal to that of the compressor, which is on the same shaft.
> However multi-shaft arrangements are common to optimise rotational speeds.

### Comparison of a Pure Impulse & an Impulse/Reaction Turbine
![[Pasted image 20260311120813.png|525]]
The diagram above shows the difference between impulse and impulse/reaction turbines. The difference is driven by the turbine blade geometry.

In an impulse turbine the rotation is driven by the impulse of the gas flow only and there is no convergence between the turbine blades.

In an impulse/reaction turbine the turbine blades converge and accelerate the gas flow as it passes through the turbine.

### Turbine Velocity Triangles
**Note that NGV stands for Nozzle Guide Vane**
![[Pasted image 20260311121314.png]]
![[Pasted image 20260311121328.png]]
### The Axial Flow Turbine Stage
![[Pasted image 20260311122429.png]]
If we assume constant axial velocity:
$$C_{a1}=C_{a2}=C_{a3}=C_{a}$$
So:
$$\frac{U}{C_{a}}=(\tan\alpha_{2}-\tan\beta_{2})=(\tan\beta_{3}-\tan\alpha_{3})$$
The stage work per unit mass flow is: $U\cdot\text{ Change in whirl velocity inlet to outlet}$
$$=U\cdot(C_{w2}+C_{w3})$$
$$= U\cdot C_{a}\cdot(\tan\alpha_{2}+\tan\alpha_{3})$$
Therefore:
$$\Delta h_{os}=C_{p}\cdot \Delta T_{os}=U\cdot C_{a}\cdot (\tan\beta_{2}+\tan\beta_{3})$$
Where $\Delta T_{os}$ is the stagnation temperature drop in the stage.

When the inlet and outlet velocities are the same:
$$C_{1}=C_{3}, \text{hence} ~~\Delta T_{os}=\Delta T_{s} $$
And the stagnation pressure ratio, $P_{01}/P_{03}$ can be found from $$\Delta T_{os}=\eta_{s}T_{01}\left[1-\left(\frac{1}{p_{01}/p_{03}}\right)^{\frac{\gamma-1}{\gamma}}\right]$$
### Turbine Characteristics
![[Pasted image 20260311124101.png|300]]
The efficiency over most of the operating range of a turbine is constant. There is no change in flow function with speed once the flow is choked, and most HP turbines operate in a choked condition. LP turbines will have more of their turbines in the non choked region.

### Turbine Cooling
![[Pasted image 20260311124314.png]]
As time has passed the demands for gas temperature has increased due to higher temperatures giving higher thermodynamic efficiency. Therefore blades must be cooled.
Blades are typically actively cooled using a combination of convection and film cooling:
![[Pasted image 20260311124425.png]]
A typical turbine cooling system is as follows:
![[Pasted image 20260311124520.png]]
![[Pasted image 20260311124543.png|403]]
The cooling effectiveness of a blade can be calculated as:
$$C.E.=\frac{T_{b}-T_{cr}}{T_{g~rel}-T_{cr}}$$
Note that C.E. should be around 0.5 for modern engines.
Where $T_{b}$ is the mean blade metal temperature, $T_{cr}$ is the cooling air temperature coming from the HP compressor, and $T_{g~rel}$ is the mean gas temperature coming from the combustor or previous stages.
$T_b$ needs to be kept well below the melting point to increase lifespan.

In high performance engines, HP turbines NGV's & Blades are nearly always cooled.
Intermediate pressure and low pressure turbines may sometimes be cooled depending on the cycle.
The designer will try and ensure as few stages as possible are cooled, as cooled turbine NGV's and blades are much more expensive than uncooled ones.

For simple cycles and/or gas turbines the cycle may not demand cooled blades.
