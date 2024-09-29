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
Stress is defined in a convenient but arbitrary coordinate system $XY$. But what are the stresses in the coordinate system $X'Y'$, at angle $\theta$ to the original $XY$ coordinate system?
![[Pasted image 20240929113128.png|centre|300]]
To find the stresses at the new coordinate system, consider the equilibrium of an infinitesimal element (with unit depth) cut at an angle $\theta$ (measured CCW from the Y-axis) on which a normal stress $\sigma_{x'x'}$ and shear stress $\tau_{x'y'}$ act:
![[Pasted image 20240929113250.png|centre|400]]
Resolving forces perpendicular and parallel to the cut plane:
$$\sigma_{x'x'}=(\sigma_{xx}\cos\theta+\tau_{xy}\sin\theta)\cos\theta+(\sigma_{yy}\sin\theta+\tau_{xy}\cos\theta)\sin\theta$$
$$\tau_{x'y'}=-(\sigma_{xx}\cos\theta+\tau_{xy}\sin\theta)\sin\theta+(\sigma_{yy}\sin\theta+\tau_{xy}\cos\theta)\cos\theta$$
We can reshuffle and combine into a transformation matrix $\textbf{T}$:
$$\begin{bmatrix}\sigma_{x'x'}\\\sigma_{y'y}\\\tau_{x'y'}\end{bmatrix}=\begin{bmatrix}\cos^{2}\theta&\sin^{2}\theta&2\sin\theta\cos\theta\\\sin^{2}\theta&\cos^{2}\theta&-2\sin\theta\cos\theta\\-\sin\theta\cos\theta&\sin\theta\cos\theta&\cos^{2}\theta-\sin^{2}\theta\end{bmatrix}\begin{bmatrix}\sigma_{xx}\\\sigma_{yy}\\\tau_{xy}\end{bmatrix}$$
Where $\sigma_{y'y'}$ is found using $\theta_{y'}=\theta_{x'}+ \frac{\pi}{2}$ 
\
Theses stress transformation equations will enable us to calculate the stresses in any given direction, and form the core of 2D stress analysis.
### Properties of Plane Stresses
The stress transformation equations enable us to calculate the stresses in any direction. As we rotate through different angles the direct stresses vary periodically:
![[Pasted image 20240929114152.png|centre]]
