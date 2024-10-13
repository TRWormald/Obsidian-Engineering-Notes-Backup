In multi-cell sections we analyse each cell $j$ separately, considering individual cell areas $\bar{A}_{j}$ and solving for shear flow constants $\bar{q}_{j}$.
We follow the right hand rule when integrating along each cell.
Cells interact in two different ways:
![[Pasted image 20241013121607.png]]
### Simultaneous Equations
Cells are indexed by the subscript $j=1...n$, where $n$ is the total number of cells.
We introduce a 'notional cut' in each cell, and we get $n$ unknown values of $\bar{q}_{J}$.
The externally applied load or global deformation usually provides an additional unknown:
- Pure torsion: $T$ or $\frac{d\theta}{dz}$
- Shear loading $e_{x}$, $e_{y}$, or $\frac{d\theta}{dz}$
We need $(n+1)$ equations to solve for these unknowns.
\
Writing the twist rate equation for cell $j$ gives:
$$\frac{d\theta}{dz}=\frac{1}{2\bar{A}_{j}G}\oint_{j}q_{(s)}^{closed} \frac{ds}{t}$$
So we can rearrange this to be:
$$\oint_{j}q_{(s)}^{closed} \frac{ds}{t}=(2\)$$