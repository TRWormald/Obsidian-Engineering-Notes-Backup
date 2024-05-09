Control Volume (CV) analysis is a process where we draw an imaginary boundary, associated with a system, that encloses the desired CV. We then consider the rate at which the **mass**, **momentum** (linear and angular), and **energy** enter and leave the CV.
**Note that when drawing a CV boundary it must be perpendicular to the direction of flow at any point.**
### The Conservation of Mass for a Control Volume
The rate of change of mass inside a CV is equal to the mass flow rate in minus the mass flow rate out.
Take the following system:
![[Pasted image 20240305121156.png|center|500]]
For unsteady compressible and incompressible flow we can write:
$$\frac{dm_{CV}}{dt}=\dot{m}_i-\dot{m}_e=\rho_i V_i A_i -\rho_e V_e A_e$$
Note that the inlet and exit areas must be measured perpendicular to the velocities.
\
For steady problems:
$$\frac{dm_{cv}}{dt}=0~~~\Rightarrow~~~\rho_iV_iA_i=\rho_eV_eA_e$$
And hence for steady incompressible flow (where density = constant):
$$\boxed{V_iA_i=V_eA_e}$$
### The Conservation of Energy for a Control Volume
We know from [[The First Law of Thermodynamics]] that:
$$\delta E=\delta Q -\delta W$$
Where $\delta E$ is the change in energy, $\delta Q$ is the change in heat, and $\delta W$ is the work done by the CV.
\
We can further decompose the work term into "shaft", "viscous", and "pressure" terms:
$$\delta W=\delta W_s+\delta W_v+\delta W_p$$
Note - Shaft work isolates the pressure and viscous work done by pumps, fans & pistons.
\
The internal energy is dependant on temperature. Hence, for incompressible steady adiabatic flow we have:
$$\boxed{p_i+\frac{1}{2}\rho V_i^2+\rho g z_i=p_e+\frac{1}{2}\rho V_e^2+\rho g z_e +\rho w_s+\rho w_v}$$
Where:
$\rho w_s$ is the shaft work done by the fluid:
- So it is positive for turbines where work is being done by the fluid on the turbine
- So it is negative for pistons/pumps/propellors where work is done to the fluid
$\rho w_v$ is the viscous work done by the fluid (not included in the shaft work)
- Is positive and represents the viscous "losses" in the flow (i.e. $\Delta p_{loss}$)
### Conservation of Steady Flow Linear Momentum for a Control Volume
If we consider [[Newton's Second Law]] applied to a point mass in vector form we get:
$$\textbf{F}_{tot}=m\frac{d\textbf{V}}{dt},~~~\textbf{F}_{tot}=\begin{bmatrix}f_{tot_{x}}\\f_{tot_{y}} \\ f_{tot_{z}}\end{bmatrix},~~~\textbf{V}=\begin{bmatrix}V_x\\V_y\\V_z\end{bmatrix}$$
Where $\textbf{F}_{tot}$ is the vector sum of all forces acting on the mass.
If we consider a CV with initial momentum in $x$ of $M_x$:
![[Screenshot 2024-03-06 103411.png|center|300]]
Since we can treat each component of the momentum in each coordinate direction separately let us initially consider the momentum in the direction of $x$.
So over time $\delta t$, the masses $\delta m_i$ and $\delta m_e$ enter and exit the CV with velocities in the $x$ direction of $V_{ix}$ and $V_{ex}$ respectively.
So, for steady control volumes the change in momentum is only due to momentum flux so:
$$\delta M_x=(V_{ix}\delta m_i-V_{ex}\delta m_e)$$
Furthermore if the flow is steady:
$$\delta m_i=\delta m_e=\delta m$$
So (whilst also dividing through by $\delta t$):
$$\textbf{f}_{tot_{x}}=\dot {\textbf{M}}_x=\dot{ \textbf{m}}(\textbf{V}_{ix}-\textbf{V}_{ex})$$

$$\textbf{f}_{tot_{y}}=\dot {\textbf{M}}_y=\dot{ \textbf{m}}(\textbf{V}_{iy}-\textbf{V}_{ey})$$

$$\textbf{f}_{tot_{z}}=\dot {\textbf{M}}_z=\dot{ \textbf{m}}(\textbf{V}_{iz}-\textbf{V}_{ez})$$
This is the **force exerted by the control volume** (i.e. on objects in the flow), the total force exerted on a control volume is the negative of the above formulae (i.e. the exit and entry velocities switch places in the equation).
**The force exerted on the control volume (i.e. on the fluid)** can be calculated using the following equations:
$$
\boxed{\large
\begin{align*}
f_{tot_{x}}&= \dot{m}(V_{ex}-V_{ix})\\\\

f_{tot_{y}}&= \dot{m}(V_{ey}-V_{iy})\\
\\

f_{tot_{z}}&= \dot{m}(V_{ez}-V_{iz})
\end{align*}}$$
**Note that these are the equations that should be used in questions.**
When using these equations refer to the section below with regards to $f_{tot_{n}}$ as it is not just equal to the force exerted by objects in the flow.
### Forces on the Control Volume
Total/net force on the CV can be split into:
- Pressure forces acting normally to the external CV boundary. Note, a constant pressure integrates to zero so we can subtract/add a constant from/to the pressure (e.g. subtract atmospheric pressure and integrate gauge pressures.)
![[Pasted image 20240306104926.png|center|200]]
- Viscous shear forces acting tangentially to the external control surface boundary. Note that for pressure and viscous forces we are only interested in the boundary.
![[Pasted image 20240306104943.png|center|200]]
- Forces exerted on the fluid by solid objects. Whenever a solid surface cuts the CV boundary there is a net resultant force (e.g. if the drag on the body is D, the resultant force on the fluid is -D)
![[Pasted image 20240306104959.png|center|250]]
- Gravitational body forces are integrated over the whole control volume. All the other forces act on the CV surface only.
![[Pasted image 20240306105013.png|center|200]]
**This means that we can represent the total force on a control volume in a given axis n as:**
$$F_{tot_{n}}=F_p+F_{visc}+F_{cut}+F_g$$

