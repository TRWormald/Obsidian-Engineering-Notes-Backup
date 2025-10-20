>"Flight dynamics in aviation and spacecraft, is the study of the performance, stability, and control of vehicles flying through the air or in outer space. It is concerned with how forces acting on the vehicle determine its velocity and attitude with respect to time."

>All axes that we use follow the **Right Hand Rule**
### Reference Axes - Earth
Movements of a point mass do not require a local set of axes attached to the mass. *However movements of a rigid body having distributed mass do require a local set attached to the body, with the second set for reference.* 
For most cases we use the earth axis as the reference frame - typically this is a point on the surface for a fixed wing aircraft - with x and y being along the surface at 90 degrees to each other, and z being down towards the centre of the earth.
### Reference Axes - Body
![[Pasted image 20250923111100.png|centre|400]]
Typically the x-axis is defined along the axis of the fuselage, with the y-axis pointing to the right along the chord of the wing, and the z-axis perpendicular to the plane of the wings.
Body axes are attached with the orientation often being chosen for the convenience of defining inertias.
The CG could be chosen for the origin of the body axes, but the CG position may vary.
>Generally the Body Axes will be displaced and rotated from the Reference Axes, and we need to be able to describe this difference.
![[Pasted image 20250926101837.png|centre]]
![[Pasted image 20250926101854.png|centre]]
![[Pasted image 20250926101905.png|centre]]
![[Pasted image 20250926101913.png|centre]]
### Axes Notation
The following notation is to be used:

| Name                   |        |          |        |
| ---------------------- | ------ | -------- | ------ |
| Axes                   | x      | y        | z      |
| Velocity (Steady)      | U      | V        | W      |
| Velocity (Purturbence) | u      | v        | w      |
| Rotation               | Roll   | Pitch    | Yaw    |
| Angle                  | $\phi$ | $\theta$ | $\psi$ |
| Angular Veliocity      | p      | q        | r      |

### The Euler Angles
The following diagrams show four reference frames:
1) Earth Axes Frame $F_E$
2) Intermediate Frame $F_C$
3) Intermediate Frame $F_D$
4) Body Axes Frame $F_B$

The first step is to rotate through yaw - through an angle of $\psi$ to go from $F_{E}$ to $F_{C}$:

Then you rotate through pitch - through an angle of $\theta$ to go from $F_C$ to $F_D$:

Then you rotate through roll - through an angle of $\phi$ to go from $F_D$ to $F_{B}$:
>This must be done in the correct order: Yaw -> Pitch -> Roll

### Reference Axes - Wind
We need to be able to define the forces acting on the body, and most of our "external" forces will be of aerodynamic origin.
>Hence, we need a convenient set of orthogonal axes fixed in the vehicle; then we need to know where the wind vector is, relative to these in order to express the aerodynamic forces mathematically.

If the atmosphere is steady and not moving relative to the earth, then the axes are at a tangent to the flight trajectory.
#### Angles $\alpha$ and $\beta$ 
The angle of attack $\alpha$, needs no explanation.
$\beta$ is the side-slip angle which is the angle that you need to translate the wind through to get to the vertical plane of symmetry of the aircraft (if there is a sideways component to the wind then $\beta$ is non zero).
### State Vector
$$V_{T}=\sqrt{U^{2}+V^{2}+W^{2}}$$
$$\dot{V}_{T}=\frac{U\dot{U}+V\dot{V}+W\dot{W}}{V_{T}}$$
$$\dot{\beta}=\frac{\dot{V}V_{T}-V\dot{V}_{T}}{V_{T}^{2}\cos\beta}$$
$$\dot\alpha =\frac{U\dot{W}-W\dot{U}}{U^{2}+W^{2}}$$
Meaning that the new state vector is:
$$X^{T}=[V_{T}~\beta~\alpha~\phi~\theta~\psi...]$$
### Stability Axes
The relative motion of the body axes away from the wind axes is useful when defining a disturbance, or a response to a control deflection.
It is convenient to have the two sets coincident just before the start of any study of the dynamics following a disturbance.
>This is not a particularly relevant set of axes

