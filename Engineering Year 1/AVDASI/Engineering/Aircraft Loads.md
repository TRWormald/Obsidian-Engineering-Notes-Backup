#### What materials should we use?
Exact requirements are quite complex, however we can assume that high stiffness and ultimate tensile strength are required. However for aircraft we also want to get the best stiffness and strength for our weight (as the plane still needs to take off).
These are the main considerations but cost, machineability, thermal expansion, fatigue, corrosion, and many other factors can influence material choice.
When we take all of this into account it becomes clear why composites and Al-alloys are used so much as they meet most of these requirements.
#### Loads
A **worst case load** is assessed, this is sometimes known as the limit load, when designing an aircraft. Margins of safety (typically of 1.5) are applied to this value to give the **ultimate load**.
Loads applied between the worst case load and the ultimate load can result in permanent damage and fatigue.
##### Load Cases
It isn't known in advance what the critical load cases are, although there are some common recurring ones. During design there are thousands of different configurations that are considered - for different load and fuel distributions, flap/slat settings, undercarriage up/down/transit, thrust settings and manoeuvres. Each of these needs to be assessed to see if any component reaches its critical load.
There are many cases that the aircraft type probably won't experience during its service life.
##### Gusts/Turbulence/Manoeuvring
This is a common critical case for lifting surfaces, we can calculate the maximum load:
$$L_{max}=C_{L_{max}} \frac{1}{2}\rho V^{2}_{max}S$$
There is a speed where the aircraft stalls just as it is reaching maximum load. This is known as the manoeuvre speed. Below this speed it is not possible to break the aircraft through use of full control inputs, because the lifting surfaces will stall first, limiting the maximum load.
#### Finding Loads
An ultimate load test verifies the structural response (usually buckling), but what are the loads? Sometimes they are easy to estimate, sometimes very hard.
If you overestimate loads you aircraft will be unnecessarily heavy and therefore not be able to fly as far/carry as many passengers etc.

#### Scale Modelling of Loads
When modelling ditching at scale the Froude number ($Fr$) must be matched to compare your results to the full scale. This is a [[Dimensionless Number]] and for the correct simulated damage we must also have the correct ratio of maximum stress to dynamic pressure of the water.
We calculate the Froude number as follows:
$$Fr=\frac{u}{\sqrt{gL}}$$
Where $u$ is the speed of the aircraft/model, $g$ is the acceleration due to gravity, and $L$ is a characteristic length (probably the chord length or something similar).
So we would compare in the following way:
$$\frac{u_{1}}{\sqrt{gL_{1}}}=\frac{u_{2}}{\sqrt{gL_{2}}}$$
Hence if we want to find the speed ($u_{1}$) at which the model ditches:
$$u_{1}= \frac{u_{2}\sqrt{gL_{1}}}{\sqrt{gL_{2}}}$$
$$u_{1}=u_{2}\sqrt{\frac{L_{1}}{L_{2}}}$$
