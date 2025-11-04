Finite-differences are restrictive for general problems: they require structured meshes and an involved coordinate transformation. Hence, the majority of CFD codes now are **finite-volume based**.
### The Finite-Volume Method
- Assume a constant variation of the solution across each cell
- Discretise and solve the integral form of our PDEs
- We use Greens Theorem to transform our volume integrals into boundary integrals.

### The Temporal Term
The differential form of a system of equations is:
$$\frac{\partial\mathbf{\underline{U}}}{\partial t}+\frac{\partial\mathbf{\underline{F}}}{\partial x}+\frac{\partial\mathbf{\underline{G}}}{\partial y}=0$$
We wish to transform this to an integral equation.
Integrating the equation throughout the entire volume/area of a computational cell:
$$\int\int_{A}\left(\frac{\partial\mathbf{\underline{U}}}{\partial t}+\frac{\partial\mathbf{\underline{F}}}{\partial x}+\frac{\partial\mathbf{\underline{G}}}{\partial y}\right)dA=0$$
First, just consider the temporal derivative part:
$$\int\int_{A}\left(\frac{\partial\mathbf{\underline{U}}}{\partial t}\right)dA=\frac{\partial}{\partial t}\int\int_{A}\mathbf{\underline{U}}dA$$
Then define the volume averaged value of $\mathbf{\underline{U}}$ as $\mathbf{\bar{\underline{U}}}$ defined by:
$$\mathbf{\bar{\underline{U}}}= \frac{1}{A}\int\int_{A}\mathbf{\underline{U}}~ dA$$
Therefore:
$$\int\int_{A}\left(\frac{\partial\mathbf{\underline{U}}}{\partial t}\right)dA=A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}$$
### The Flux Integral
We can collect the flux functions generally as:
$$\mathbf{F}=[\mathbf{\underline{F}},\mathbf{\underline{G}},\mathbf{\underline{0}}]^{T}$$
So that:
$$\int\int_{A}\left(\frac{\partial\mathbf{\underline{U}}}{\partial t}+\frac{\partial\mathbf{\underline{F}}}{\partial x}+\frac{\partial\mathbf{\underline{G}}}{\partial y}\right)dA=A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}+\int\int_{A}\nabla\cdot\mathbf{F}~dA=0$$
The volume flux integral ($\int\int_{A}$) is awkward, so we change it using Greens theorem which relates a volume integral to a boundary integral.

>**Greens Theorem (2D**
>$$\int\int_{A}\nabla\cdot\mathbf{F}~dA=\int_{c}\mathbf{F}\cdot \underline{\mathbf{n}}~ds$$
>Where $c$ is the domain boundary, i.e. the contour around the edge of the cell, $ds$ is an elemental length of it, and $\mathbf{\underline{n}}$ is the outward unit normal to the boundary.

So the integral form of the equation is:
$$A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}+\int_{c}\mathbf{F}\cdot \underline{\mathbf{n}}~ds=0$$
with $c$ being defined as positive anticlockwise. **This is still an exact form of the equations**.
### Expanding for 2D
![[Pasted image 20251104132058.png|centre|300]]
We have the equation derived above:
$$A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}+\int_{c}\mathbf{F}\cdot \underline{\mathbf{n}}~ds=0$$
But $d\mathbf{\underline{s}}=[dx,dy,0]^{T}$ and so:
$$\mathbf{\underline{n}}=\frac{d\mathbf{\underline{s}}\times\mathbf{\underline{k}}}{|d\mathbf{\underline{s}}|}=\frac{[dy,-dx,0]^{T}}{|d\mathbf{\underline{s}}|}$$
So:
$$\int_{c} \mathbf{F}\cdot\mathbf{\underline{n}}~ds=\int_{c}\mathbf{F}\cdot\frac{[dy,-dx,0]^{T}}{|d\mathbf{\underline{s}}|}ds$$
Hence,
$$A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}+\int_{c}\mathbf{\underline{F}}~dy-\mathbf{\underline{G}}~dx=0$$
Which is **still an exact form of the equations**.

### Discretise in Space
So we now have:
$$A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}+\int_{c}\mathbf{\underline{F}}~dy-\mathbf{\underline{G}}~dx=0$$

>**The Finite-Volume Discretisation**
>We take $\mathbf{\underline{U}}$ to be represented by the actual value of $\mathbf{\underline{U}}_{i,j}$ in the centre of the discrete cell $i,j$. **i.e. we assume the solution is constant across a single cell.**

We can say that as cell size trends to zero:
$$\frac{\partial \mathbf{\underline{U}}}{\partial t}=\frac{d \mathbf{\underline{U}}_{i,j}}{dt}$$
So:
$$\frac{d \mathbf{\underline{U}}_{i,j}}{dt}=- \frac{1}{A}\int_{c}\mathbf{\underline{F}}~dy-\mathbf{\underline{G}}~dx$$
This equation is solved in each cell to give the cell-centred solution in each cell.
### Discretise in Time
We now have:
$$\frac{d \mathbf{\underline{U}}_{i,j}}{dt}=- \frac{1}{A}\int_{c}\mathbf{\underline{F}}~dy-\mathbf{\underline{G}}~dx$$
This is the general form of a Finite-Volume scheme. There are many ways to solve this equation. The method used to compute the flux integral depends on the spatial discretisation scheme chosen. The flux integral is the residual for each cell, known as $\mathbf{\underline{R}}_{i,j}$.
![[Pasted image 20251104133123.png|centre]]
### Evaluation of the Flux