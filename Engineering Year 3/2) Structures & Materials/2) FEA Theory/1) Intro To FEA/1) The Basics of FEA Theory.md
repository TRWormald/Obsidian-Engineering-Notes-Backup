[[FEA Theory - Lecture 1.pdf|Lecture Slides]] can be found here.

>PDEs describe nature, and the Finite Element Method is used for numerically solving PDEs in engineering and mathematical modelling.

FEM solves initial boundary value problems - it subdivides large systems into smaller, simpler parts called finite elements. This is done via discretising continuum domains with a mesh of elements connected at nodes. This formulation leads to a system of algebraic equations, cast in matrix form, approximating the unknown function over the domain.
A solution is approximated by minimising an error function through the calculus of variations.

### Elements of Solid Mechanics for the Finite Element Method
Solid mechanics is governed by 15 PDEs in 15 unknowns (functions)
	There are three basic arguments **Equilibrium, Compatibility, and Constitutive**
	Deformable continua have infinite degrees of freedom
The determination of deformations, stress and strain states in any body subjected to loads, and constraints passes through solving this set of PDEs.

#### Compatibility Equations
These are the conditions that must be met by the displacement and strain components to ensure continuity (no material gaps or overlaps) and that the boundary conditions are respected.
Any displacement field satisfying the compatibility equations defines a compatible structural configuration.
![[Pasted image 20251003150827.png|centre]]

![[Pasted image 20251003150857.png|centre]]
![[Pasted image 20251003150915.png|centre]]
#### Equilibrium Equations
These are the conditions that stresses must meet for the body to be in equilibrium under the action of active and boundary forces.
Any generalised stress field satisfying the equilibrium equations defines a set of internal forces in equilibrium with external forces.
![[Pasted image 20251003151053.png|centre]]
#### Constitutive Equation
These are stress-strain relationships that describe the material's resistance to deformation under applied loads. For isotropic materials Hooke's law relates stresses and strains in terms of Young's modulus, and Poisson's Ratio.
![[Pasted image 20251003151226.png|centre|400]]
##### Navier's Equations
Substituting the strain-displacement equations into the constitutive equations, and the resultant equations into the equilibrium equation, we obtain Navier's equations.
Strains and Stresses are eliminated from the formulation, leaving the displacements as the only unknowns to be solved for.

**Displacement Methods -> Basis for FEM formulation**
![[Pasted image 20251003151417.png|centre]]
