We have previously looked at [[Actuator Disc Theory (Propellors)|actuator disk theory]].
The **lifting rotor** in its most simplistic form is a propeller: mechanical energy is used to accelerate a mass of air to generate a lifting force.
### Actuator Disc (Momentum) Theory
Newton's law, states that $F=ma$ where $F$ is the rotor thrust $T$.
![[Pasted image 20250120143825.png|centre|250]]
In the above diagram we apply Bernoulli's equation to either side of the actuator disk to get:
$$H_{0}=P_{0}+ \frac{1}{2}\rho V^{2}=P_{1}+ \frac{1}{2}\rho (V+v)^{2}$$
$$H_{1}=P_{0}+ \frac{1}{2}\rho (V+v_{1})^{2}=P_{1}+P'+ \frac{1}{2}\rho (V+v)^2$$
Subtracting $H_{0}$ from $H_{1}$ results in:
$$H_{1}-H_{0}=\frac{1}{2}\rho(2Vv_{1}+v_{1}^{2})=P'$$
However, the Thrust is equal to the change in axial momentum per unit time:
$$\frac{T}{A}=P'=\rho(V+v)v_{1}$$
Which can be obtained from [[Control Volume Analysis Introduction|control volume analysis]]. Where $A$ is the rotor disc area.


Therefore we have:
$$H_{1}-H_{0}=\frac{1}{2}\rho(2Vv_{1}+v_{1}^{2})=P'$$
$$\frac{T}{A}=P'=\rho(V+v)v_{1}$$
From which we can get:
$$\frac{v_{1}}{2}=v~~~~\text{or}~~~~v_{1}=2v$$
$$\text{Thrust:}~~~T=2\rho A(V+v)v$$
$$\text{Power:}~~~P=T(V+v)$$
### Momentum Theory in Hover
For a rotor in hover, when the onset velocity $V=0$, we get that the induced velocity is:
$$v_{h}=\sqrt{\frac{T}{2\rho A}}$$
With the induced power being:
$$P=Tv_{h}~~~~\text{hence,}~~~~P_{h}=\frac{T^{\frac{2}{3}}}{\sqrt{2\rho A}}$$
### Induced Velocity in Axial Flight
> How does the induced velocity change in steady state axial (vertical) flight?

Firstly, steady state means that the vertical acceleration of the helicopter is zero. This means that the helicopter is:
- In a climb at constant speed
- In a descent at constant speed
- In hover condition

Starting from:
$$T_{Hover}=T_{AxialFlight}=T,$$
$$2\rho Av_{h}^{2}=2\rho A(V+v)v$$
If we then divide both sides by $v_{h}^{2}$, and plot the variation of $\frac{v}{v_{h}}$ as a function of $\frac{V}{v_{h}}$:
$$\frac{v}{v_{h}}=\frac{-V_{c}}{2v_{h}}$$