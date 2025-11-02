We have previously looked at the equations of motion for general atmospheric 6-DoF flight. They are all first-order differential equations that can be expressed in nonlinear form as:
$$\dot{x}=f(x,\delta)$$
Where:
$$x=[U,V,W,p,q,r,\psi,\theta,\phi,x_{E},y_{E},z_{E}]$$ is the state vector, and $\delta$ is the vector of input parameters of interest. These are often aerodynamic or propulsion system inputs such as aileron, elevator, rudder deflection, or thrust.
The purpose of these equations are to simulate the aircraft, allowing us to predict how the aircraft will respond to control inputs.
**But how do we define a trimmed condition?**
For a trimmed condition the state vector will be constant with a specific flight regime (i.e. steady level flight).

![[Pasted image 20251024100818.png|centre]]
### Trimming
>The object of trimming is to bring the forces and moments acting on the aircraft into a state of equilibrium. That is the condition when the axial, normal, and side forces, and the roll, pitch, and yaw moments are all zero.
>Provided that the aircraft is stable it will then stay in equilibrium until it is disturbed by pilot control inputs or by external influences such as turbulence.

### Linearisation
The equations of motion (of an aircraft) are non-linear and their solution by analytical means is not generally practicable. In order to proceed with the development of the equations of motion for analytical purposes, they must be linearised.
![[Pasted image 20251024101150.png|centre]]
For an explanation of the numerical (MATLAB) method for trim look at the information on [[Flight Dynamics Lecture 13 - Trimming and Linearisation.pdf#page=15|Flight Dynamics Lecture 13 - Trimming and Linearisation, p.15]].

