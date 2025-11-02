All of the 12 equations shown in [[2) Equations of Motion 1#The 12 Equations of Motion for General Atmospheric 6-DoF flight|the previous note]] are first-order differential equations that can be expressed in nonlinear state-space form as:
$$\dot{x}=f(x,\delta)$$
Where:
$$x=[U,V,W,p,q,r,\psi,\theta,\phi,x_{E},y_{E},z_{E}]$$
Is the state vector, and $\delta$ is the vector of input parameters of interest. These are often aerodynamic or propulsion system inputs such as aileron, elevator, rudder deflection or thrust.

The motions that are described are as a consequence of the applied forces and moments from outside the body, being:
- Aerodynamic
- Propulsive
- Gravitational
The list above must be all inclusive, including things like drag due to lowered undercarriage, or lift, drag, and pitching moment change due to flaps.
Aerodynamic forces are typically modelled using tables, to allow us to quickly simulate - rather than using CFD.
### The Formal Equations
With the gravitational forces separated from the aerodynamic/propulsive forces, the translational equations can be written as follows:
![[Pasted image 20250926112439.png|centre|400]]
Similarly the rotational equations are expressed in their complete form as:
![[Pasted image 20250926112517.png|centre|400]]

