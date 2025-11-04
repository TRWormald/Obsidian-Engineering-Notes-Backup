For generated body-fitted meshes, the mesh lines are not aligned to the global $x$, $y$, or $z$ directions - so how can we apply finite differences? We need to transform our coordinates.

> **Coordinate transform**
> Transformation of coordinates from the physical domain to a computational domain, where in the computational domain all mesh lines are equally spaced.

The coordinate transformation is applied to the PDEs; the transformed equations are solved in the equally-spaced computational domain.
![[Pasted image 20251104130622.png|centre]]
The coordinate transform requires **much more work** to implement - and mistakes are easily made.