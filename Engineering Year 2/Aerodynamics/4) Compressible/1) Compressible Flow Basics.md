### What is Compressibility
Compressibility is effectively where density is a function of pressure.
![[Pasted image 20250114212300.png|centre]]
We can see how an increased Mach number changes the stagnation density (the density when the air is completely brought to a halt).
> Note that density is also a function of:
> - Temperature
> - Energy
> - Flight speed

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
$$p=\rho RT$$
and the equation for a calorically perfect gas:
$$e=c_{v}T$$Where $c_{v}$ is the specific heat at constant volume.
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
