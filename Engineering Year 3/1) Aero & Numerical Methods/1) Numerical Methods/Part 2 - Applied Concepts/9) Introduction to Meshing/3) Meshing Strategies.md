Among the two mesh classes, there are several commonly-used strategies for meshing:
**Structured**
- Simple cartesian, not body fitted (immersed boundary)
- Single-block, body-fitted
- Multi-block, body-fitted
**Unstructured**
- Body-fitted
- Non-body-fitted, volume mesh intersects parameterised surface (immersed boundary)
>The choice of meshing strategy is related to the capabilities of your flow solver - most flow solvers are either structured or unstructured (not both)

### Terminology
>**Body Fitted**
>The vertices and faces of the mesh conform to solid surfaces. i.e. The geometry of interest defines, and is defined by, one or more boundaries of the mesh

Body fitted meshes are the norm since boundary conditions can be implemented as part of the existing spatial discretisation. If a mesh is not body-fitted, then additional numerical methods are needed to apply boundary conditions (immersed boundary method) - *this will not be discussed in this course*.

