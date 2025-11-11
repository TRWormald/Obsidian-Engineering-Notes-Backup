So far we have assumed that the solution values have been stored at the cell centres. This is a natural choice, since the finite volume method produces a residual update based on the cell boundary integers.
However, there are some challenges when using the cell centred approach:
- Boundary Conditions
	How do we apply our stencil at the boundaries where one or more stencil points will be missing
- Obtaining Surface Values
	Surface values are important for determining body forces, however the cell-centred approach does not store values on the surface but half a cell away from the surface.
### Cell-Centred Boundary Conditions
>**Halo Cells**
>These are additional fictitious cells added outside the mesh boundary to complete the stencil. The solution is not updated here but explicitly specified in order to enforce boundary conditions. 

![[Pasted image 20251111130821.png|centre|300]]
Let's consider an inviscid boundary where the flow must be tangential. Since the solution at each cell face is an average of that either side, we reflect the normal component of the velocity vector, and keep the same tangential part, and so half of the values either side give us tangential flow since the normal components cancel.

For scalar components, e.g. density, we simply use the same value as the first inner cell.

We could use the local gradient to get a more accurate value, but then we need to do something more clever with the velocity, since changing the pressure and density without changing the velocity vector changes the total pressure, which cannot happen ([[Bernoulli's Equation]]).
### Cell-Centred Surface Values
We use surface pressures in order to integrate forces for lift and drag etc.
![[Pasted image 20251111131134.png|centre|300]]
A first order approximation involves assuming that the value at the surface is equal to the first cell.

A second order approximation assumes linear variation and extrapolates the value down to the surface.
$$\mathbf{\underline{U}}_{surface}=\mathbf{\underline{U}_{A}}+\frac{\mathbf{\underline{U}}_{A}-\mathbf{\underline{U}}_{B}}{\Delta s_{1}}\Delta s_{2}$$
$$\int\Delta\phi dV=\int\Delta \mathbf{n} dS$$
#### Cell-Centred - The Impact of Mesh Quality
We encounter a further problem with the cell-centred approach being affected by mesh quality. Consider highly skewed cells:
![[Pasted image 20251111131538.png|centre|300]]
![[Pasted image 20251111131620.png|centre|300]]
The values at "C" are unlikely to be accurately given by $\frac{1}{2}(A+B)$.
### Cell-Vertex
The problem encountered with the cell-centred approach can be avoided by storing the solution at the cell nodes/mesh vert