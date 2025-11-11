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
The problem encountered with the cell-centred approach can be avoided by storing the solution at the cell nodes/mesh vertices.
The flux across each face is simply obtained from an average of the fluxes at the vertices:
![[Pasted image 20251111131731.png|centre|400]]
Note that the updating scheme for each cell is the same regardless of the storage approach used:
![[Pasted image 20251111131806.png|centre|275]]
The flux integral gives the change in the solution for the volume surrounded by the vertices, i.e. it is not associated with a specific solution point. The difference between the cell-centred and cell-vertex schemes is in the evaluation of the face fluxes.

So, if the solution is stored at the mesh points:
- What does this mean for the stencil?
- How much information is required outside the stencil?
- What do we need to do at the boundaries?
- How would we apply an upwind scheme?

#### Cell-Vertex Update - Redistribution
The flux integral gives the change in the solution for the volume surrounded by the vertices, i.e. it is not associated with a specific solution point.
Hence this change has to be redistributed to the cell vertices by a simple averaging process:
$$\Delta \mathbf{\underline{U}}_{C}=\frac{1}{4}(\Delta\mathbf{\underline{U}}_{1}+\Delta\mathbf{\underline{U}}_{2}+\Delta\mathbf{\underline{U}}_{3}+\Delta\mathbf{\underline{U}}_{4})$$
But this is diffusive. The redistribution procedure needs modifying at boundaries and upwind implementation is difficult.
#### Cell-Vertex - Stability
Similar to the cell-centred central discretisation, the cell-vertex scheme is fundamentally unstable and requires artificial dissipation to stabilise.
However, there is an additional cause of instability for cell vertex schemes.
The fluxes computed at each face may satisfy the equations, but there is an unbounded error, $\Delta\mathbf{\underline{F}}$ which can cause an odd-even instability, called the Chequerboard instability.
The values of the cell face fluxes are unaffected by this error, so the scheme cannot correct it.

### Vertex-Centred Scheme
A third approach is a combination of cell-centred, and cell-vertex; solution data is stored at cell vertices, but the mesh cells are not used as the control volumes.

>**Vertex centred scheme**
>Control volumes are created around each mesh vertex (usually called nodes) by joining each mesh cell centre with each mesh face centre; this is called a dual mesh, and is normally constructed during a pre-processing stage, prior to running a simulation.

![[Pasted image 20251111132928.png|centre|200]]

| Advantages                                                                                                                                                        | Disadvantages                                                                                                                                                                    |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Have points on boundary: no need for special boundary treatment                                                                                                   | This approach means the control volumes are expensive to store and the flux integral expensive to compute, as the control volume is constructed from many smaller edges or faces |
| For an unstructured mesh, each control volume has more edges so more mesh points influence the solution; much more accurate as it covers spatial variation better |                                                                                                                                                                                  |
| For both structured and unstructured meshes it allows higher order flux integration. One value of f                                                               |                                                                                                                                                                                  |
