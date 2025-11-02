Mesh adaption is where we increase the number of cells where there are large gradients in the solution.
**Motivation**:
- Numerical dissipation present in all numerical schemes means that regions of the flow with large gradients (e.g. shocks) become smeared over multiple computation cells
- To make the solution "sharper", we need to add more mesh points to reduce the mesh spacing.
**Refinement Criteria**: (Normally a set of PDEs are solved such that:)
$$\Delta x_{i,j,k}\propto\left(\frac{\partial S_{i,j,k}}{\partial x}\right)^{-1}~~~~\Delta y_{i,j,k}\propto\left(\frac{\partial S_{i,j,k}}{\partial y}\right)^{-1}~~~~\Delta z_{i,j,k}\propto\left(\frac{\partial S_{i,j,k}}{\partial z}\right)^{-1}$$
Where $S$ is some scalar quanitity. Mach number is often used. The resulting equations are normally very complex, and require more time to solve than the flow equations.
### Structured Mesh Adaption
![[Pasted image 20251023132107.png|centre]]
![[Pasted image 20251023132119.png|centre]]
### Unstructured Mesh Adaption
Unstructured mesh adaption is much simpler. Extra nodes, and hence cells, are simply added where the gradients are large (known as enrichment). Some cells can be removed where gradients are very small, but normally there will be more cells in an adapted unstructured mesh than the original one.
This part is simple, but when new points are added new cells are created, and all the connectivity must be recomputed. This is extremely time consuming.
![[Pasted image 20251023132305.png|centre]]
We can also refine a cartesian type grid as an unstructured grid. This makes recalculation of connectivity slightly simpler.
![[Pasted image 20251023132350.png|centre]]
![[Pasted image 20251023132402.png|centre]]
![[Pasted image 20251023132442.png|centre]]
