### Momentum Theory with Swirl
Let us again consider the **Actuator Disc Theorem**:

For a propeller or axial fan:
Mechanical energy (in the form of rotating blades) is used to accelerate a mass of air. Newton's law (every action has an equal and opposite reaction), states $F=ma$, where $F$ is the propeller thrust.
![[Pasted image 20260209110516.png|centre]]
![[Pasted image 20260209110536.png|centre]]
**Momentum Analysis based on the Actuator Disk Theorem can be extended to include swirl, though strictly speaking it can no longer be referred to as an Actuator Disk.**

$$\frac{\bar{P}}{\rho} + \frac{1}{2}\bar{V}^{2}+\frac{K^{2}}{A}=constant,~~~~where~~K=\frac{\tau}{\dot{m}}$$
Where $K$ is a swirl parameter based on a free vortex and $\tau$ is fan torque and $\dot{m}$ is the mass flow rate.

### Swirl Power
The swirl power is supplied directly to the air by the fan:
$$\text{Swirl Power}=\frac{\dot{m}K^{2}}{A}$$
For the real flow applications that follow in the Blade Element Analysis, the swirl is shown to be the result of combined *blade viscous effects* and in plane contributions from the *lift induced velocity at the rotor plane.*

It should be noted that the swirl only exists in the downstream wake. Upstream of the rotor the flow is irrotational for reasons explained later.

This is of course why in wind tunnel design the working section is (almost) always upstream of a non-contra-rotating fan.

![[Pasted image 20260209111100.png|centre|500]]

### Blade Element Analysis
In reality **Ideal** propellers don't exist, so we need to consider real propellers. In analysis and predicting propeller/rotor performance we need to consider:
- Viscosity of the fluid
- Rotor blade tip effects
- Non-uniform inflow
- Blade vortex interaction
$$\eta_{p}=\frac{TV}{P}\left(=\frac{TV}{T(V+v)+\text{Losses}}\right)$$
Needless to say, these result in energy loss and therefore reduced efficiency.
In order to obtain a more detailed knowledge of the behaviour of a rotor:
- It is necessary to analyse the forces on the rotor blades
- The blade has to be considered as a number of separate aerofoil elements
- Elements are then integrated to represent the characteristics of the whole propeller.

This is achieved by **Blade Element Analysis** (sometimes called Strip Analysis)

