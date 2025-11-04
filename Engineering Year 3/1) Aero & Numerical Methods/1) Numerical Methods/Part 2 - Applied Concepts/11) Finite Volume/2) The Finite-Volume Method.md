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
$$\int\int_{A}\left(\frac{\partial\mathbf{\underline{U}}}{\partial t}+\frac{\partial\mathbf{\underline{F}}}{\partial x}+\frac{\partial\mathbf{\underline{G}}}{\partial y}\right)dA=A\frac{\partial \mathbf{\bar{\underline{U}}}}{\partial t}+\int\int_{A}\nabla$$