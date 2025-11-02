Take the following NACA0012 aerofoil which has been meshed in an unstructured grid with triangular elements:
![[Pasted image 20251021131456.png|centre|400]]
How is the mesh stored?
We have a list of node co-ordinates, as well as a list of cells/faces joining the nodes.
![[Pasted image 20251021131559.png|centre]]
### Cutcell Mesh
Below is an example of the same aerofoil, but using an unstructured grid with cutcell mesh:
![[Pasted image 20251021131724.png|centre|400]]
Cutcell meshing is automated, and can mesh complex geometries and topologies.
Cutcell is:
1) **Unstructured** - note that some cells have more than four faces
2) **Efficient** - there is refinement near the surface where it is needed and the mesh gets coarser out to the farfield
3) **Mesh Adaption** - It is extremely quick and east to automate refinement and coarsening
#### How do you make a cutcell mesh?
1) Import a surface (probably an STL triangulation)
2) Make a background grid and detect where intersection occurs
3) Refine cells with intersections until you are happy with the resolution
4) Split mesh edges and re-insert in mesh - detecting any new edges created
5) Split surface edges and insert in mesh - detecting any new edges created
6) Add all edges to loops around faces
7) Detect any split faces
8) Detect any split cells
##### How do you know if a cell is split or not?
1) Pick a vertex. Colour the edges that meet at that vertex
2) Colour any vertices that are part of a coloured edge
3) Repeat this process until no more vertices or edges are coloured on a particular step
4) Are there any vertices or edges left uncoloured? If no, you are finished and the cell is unsplit. If yes you have traced out one loop, and the next loop must be another (new) cell that has been split off from it.
>In 3D, exactly the same process can tell you if a cell has been split too, but it requires detecting all the split faces first, which requires knowing all the split edges.

This ‘bootstrap’ integer logic works fine, but only if you make zero errors. A single error will fail the entire process. Consider how many types of edge, face and cell splits can exist in general. There is almost no limit to their complexity. Your code must handle them all - this is no small challenge! Often people avoid these issues; relatively few cartesian methods resolve all splits. Cart3D (NASA) and the one we gave you do, though.
Cartesian meshes are suitable for inviscid or low-Re cases. To handle high-Re, you need to insert boundary layer cells that are appropriately stretched. The SOLAR system from BAe is a nice example of this