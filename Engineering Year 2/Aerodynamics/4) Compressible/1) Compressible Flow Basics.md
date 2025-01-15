### What is Compressibility
Compressibility is effectively where density is a function of pressure.
![[Pasted image 20250114212300.png|centre]]
We can see how an increased Mach number changes the stagnation density (the density when the air is completely brought to a halt).
> Note that density is also a function of:
> - Temperature
> -> and therefore Energy
> -> and therefore Flight speed

### Navier-Stokes
The Navier-Stokes equations in a fixed Cartesian coordinate system describe unsteady, viscous, compressible flow with body forces. In 3D there are 7 different unknown quantities, and the equations are:
- Conservation of Mass (1 eqn)
- Conservation of Momentum in each coordinate direction (3 eqn)
- Conservation of total Energy (1 eqn)
- Two equations that come from the fundamental properties of the fluid
These equations determine the behaviour of all the flow quantities such as density, the three components of velocity, temperature, pressure, energy, and viscosity.
### Conservation of Energy
Energy cannot be created or destroyed, merely changed in form - therefore we need to balance:
1) Fluid energy
	1) Internal energy
	2) Kinetic Energy
	3) Potential energy
With
2) Heat transfer and work done
	1) Work done by body forces
	2) Work done by pressure forces
	3) Heat transfer
	4) Viscous dissipation

Which necessitates the 2 equations of state for specific internal energy $e$ and temperature $T$.

Typically these are the ideal gas law:
$$\boxed{p=\rho RT}$$
and the equation for a calorically perfect gas:
$$\boxed{e=c_{v}T}$$Where $c_{v}$ is the specific heat at constant volume.
### Basic Thermodynamics
We consider a thermally perfect gas, so:
$$p=\rho RT$$
Where $R$ is the gas constant (287 for air)
The gas is also calorically perfect therefore:
$$e=c_{v}T$$
Where $c_{v}$ is specific heat at constant volume (717 for air at standard conditions).

We will also need specific enthalpy $h$ which is defined as:
$$h=e+\frac{p}{\rho}$$
Which when simplified using $p=\rho RT$ and $e=c_{v}T$, and noting that $c_{v}+R=c_{p}$:
$$h=c_{p}T$$
Where $c_p$ is the specific heat at constant pressure (1004 for air at standard conditions)

The ratio of specific heats $\gamma$:
$$\gamma=\frac{c_{p}}{c_v}$$
Note that this is $\approx 1.4$ for air at standard conditions.
#### Entropy
Entropy $s$ represents the degree of disorder or in other words how spread out the energy is.
It determines the direction of the thermodynamic process - note that the actual value of $s$ is unimportant.
However it should be noted that entropy always increases.

It is defined as:
$$ds=\frac{\delta q_{rev}}{T}=\frac{\delta q}{T}+ds_{irrev}$$
Where:
- $\delta q$ is the amount of heat added to the system at room temperature $T$
- $ds_{irrev}$ is entropy increase due to dissipative phenomena (viscosity, thermal conductivity, and mass diffusion) occurring within the system - it is always positive.

#### Integrating the First Law of Thermodynamics
The first law is as follows:
$$de=\delta q+\delta w$$
We can substitute in $\delta q$ from the second law, giving:
$$T ds=de-\delta w$$
Then for a reversible process:
$$\delta w=-pdv$$
Where $v$ is specific volume 1/$\rho$, hence:
$$Tds=de+pdv$$
We can do some rearrangement and substitution to give us:
$$ds=c_{p}\frac{dT}{T}-R\frac{dp}{p}$$
Which can be integrated between two positions in the flow, resulting in:
$$s_{2}-s_{1}=c_{p}\ln\left(\frac{T_{2}}{T_{1}}\right)-R\ln\left(\frac{p_{2}}{p_{1}}\right)$$So for a reversible process where $s_{2}-s_{1}=0$:
$$\frac{c_{p}}{R}\ln\left(\frac{T_{2}}{T_{1}}\right)=\ln\left(\frac{p_{2}}{p_{1}}\right)$$
Resulting in:
$$\frac{p_{2}}{p_{1}}=\left(\frac{T_{2}}{T_{1}}\right)^{\frac{\gamma}{\gamma-1}}$$
And we can use the ideal gas law to relate this to density:
$$\boxed{\frac{p_{2}}{p_{1}}=\left(\frac{T_{2}}{T_{1}}\right)^{\frac{\gamma}{\gamma-1}}=\left(\frac{\rho_{2}}{\rho_{1}}\right)^{\gamma}}$$
This implies that:
$$p=const\cdot\rho^{\gamma}$$
Hence differentiating gives:
$$\frac{dp}{d\rho}=\frac{\gamma p}{\rho}$$