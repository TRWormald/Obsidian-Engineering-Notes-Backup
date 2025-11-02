### Chimera/Overset Meshes
As an alternative to structured multiblock meshes is the Chimera/Overset approach. This is where:
- Single block grids are generated around each body independently
- The complete mesh is assembled by placing all meshes over each other, with no matching boundaries
These kinds of meshes are usually used for simulations with relative motion of bodies, however a special flow solver is required to interpolate the solution between Chimera/Overset blocks.
![[Pasted image 20251023130516.png|centre|400]]
The overlap region between the meshes might be large - and it is inefficient to solve for the solution in all blocks - therefore an algorithm is used to remove redundant cells in each mesh, and minimise the size of the overlap region.
We also need a complex tagging algorithm to find neighbouring cells between different grid blocks. These cells are tagged as:
- Normal cell - the solution is stored and updated by the solver
- Fringe cell - solution is stored and interpolated from another grid block
- Hole cell - solution is not stored
The interpolation must be accurate to preserve the overall spatial accuracy of the solver.
#### Examples
![[Pasted image 20251023130811.png|centre]]
![[Pasted image 20251023130821.png|centre]]
### Hybrid Meshes
Studies show that unstructured meshes are not suitable for viscous computations. This is because:
- Viscous terms are second differences, and normally require at least five points in each coordinate direction.
- It is very awkward to obtain high accuracy over many cells for unstructured meshes.
- Also there is no obvious cell direction normal to solid surfaces, so large gradients are difficult to maintain near surfaces (required for turbulence models)
To overcome these problems, hybrid meshes have been implemented. This is where a structured grid is used around solid surfaces and unstructured meshes are used far away from solid surfaces. Exact matching at the boundary between the two means no interpolation is necessary.
![[Pasted image 20251023131254.png|centre]]
A high quality structured grid near the surface is very good at accurately resolving flow features, particularly viscous layers, whilst an unstructured grid away from solid surfaces simplifies the mesh generation process, and allows coarser grid densities away from areas of interest.
![[Pasted image 20251023131414.png|centre]]
