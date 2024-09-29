### Stress Definition
*The total stress on an infinitesimal element of a plane taken within a deformed elastic body is defined as the resultant of all the actions of the molecules situated on one side of the plane upon the molecules on the other side.*
**Saint-Venant (1797-1886)**
\
An infinitesimal element of material with dimensions $dx×dy ×dz$ is subjected to direct stresses $σ_{xx}$ and shear stresses $τ_{xy}$ . Direct stresses act normal to a face, whereas shear stresses act parallel.
![[Pasted image 20240929111311.png|centre|300]]
The first index in these defines the face on which the force acts, whilst the second tells you the direction of the stress.
### Complementary Shear
As the elements we will be considering are in equilibrium the shear stresses are not independent:
![[Pasted image 20240929111555.png|centre|300]]
If we consider moment equilibrium about the centre of this infinitesimal element:
$$\tau_{xy}=\tau_{yx}$$
As a result of this we can express our 3D stress state in 6 components:
$$\bar{\sigma}=\begin{bmatrix}\sigma_{xx}&\tau_{xy}&\tau_{xz}\\\tau_{xy}&\sigma_{yy}&\tau_{yz}\\\tau_{xz}&\tau_{yz}&\sigma_{zz}\end{bmatrix}$$
This formulation is known as the Cauchy stress tensor.
### Plane Stress
A common simplification is plane stress, with no out of plane stresses:
$$\sigma_{zz}=\tau_{xz}=\tau_{yz}=0$$
So the 3D stress state is reduced to three independent variables: $\sigma_{xx}$, $\sigma_{yy}$, and $\tau_{xy}$.
![[Pasted image 20240929112423.png|centre]]
### Stress Transformations
