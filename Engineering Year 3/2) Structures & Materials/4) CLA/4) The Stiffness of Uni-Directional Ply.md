The objective is to describe the stiffness and strength of uni-directional composite ply.
In macromechanics we derive constitutive equations by modelling the ply as a homogeneous material.
### Stress
![[Pasted image 20251114152156.png|centre]]
### Strain
![[Pasted image 20251114152212.png|centre]]
![[Pasted image 20251114152224.png|centre]]
### Composite Stress-Strain Relationship
As mentioned earlier we consider lamina as a homogeneous material, and that it is anisotropic - which means that the mechanical properties differ along the direction of fibres and perpendicular to the fibres.
![[Pasted image 20251114152336.png|centre]]
The sign convention is that 123 refers to the material axes, and xyz refers to the structural axes.

For a general anisotropic, linear-elastic material:
![[Pasted image 20251114152426.png|centre]]
![[Pasted image 20251114152454.png|centre]]
![[Pasted image 20251114152510.png|centre]]
![[Pasted image 20251114152521.png|centre]]
![[Pasted image 20251114152534.png|centre]]
![[Pasted image 20251114152546.png|centre]]
![[Pasted image 20251114152558.png|centre]]
### Composite Lamina: Specially Orthotropic
We can formulate constitutive equations in natural/material axes (123) and assume each lamina to be loaded under plane stress.

The constitutive equations reduce for a specially orthotropic material:
![[Pasted image 20251114152739.png|centre]]
$Q_{ij}$ components are known as reduced stiffness:
$$Q_{ij}=C_{ij}-\frac{C_{i3}C_{j3}}{C_{33}},~~~i,j=1,2,6$$
found from $C_{ij}$ imposing the plane stress condition:
![[Pasted image 20251114152854.png|centre]]
We can find $\mathbf{Q}$ by inverting the plane stress compliance matrix $\mathbf{S}$:
![[Pasted image 20251114153028.png]]
To give:
![[Pasted image 20251114153039.png|centre]]
And the compliance matrix is constructed by considering three load cases:
1) Uni-axial stress $\sigma_{11}$ 
![[Pasted image 20251114153123.png|centre]]
2) Uni-axial stress $\sigma_{22}$
![[Pasted image 20251114153145.png|centre]]
3) Pure shear $\tau_{12}$
![[Pasted image 20251114153206.png|centre]]
Each load case provides a column of $\mathbf{S}$:
![[Pasted image 20251114153252.png|centre]]
The symmetry of the compliance matrix gives:
$$\frac{\nu_{21}}{E_{22}}= \frac{\nu_{12}}{E_{11}}$$
### Summary
![[Pasted image 20251114153358.png|centre]]
![[Pasted image 20251114153406.png|centre]]
