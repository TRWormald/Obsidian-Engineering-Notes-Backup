Recall that a vector field $\mathbf{v}$ is only conservative if and only if $curl~\mathbf{v}=0 \Leftrightarrow \mathbf{v}=\boldsymbol{\nabla}\phi$, for some scalar function $\phi$.
We can now add the following result:
*If the vector field $\mathbf{F}$ is **conservative** then the work integral $\int_{A}^{B}\mathbf F \cdot d\mathbf r$ between two points $A$ and $B$ is **independent of the path** $C$ chosen between $A$ and $B$ (provided $\mathbf{F}$ remains finite within a simple domain containing $A$ and $B$)*
\
Moreover, writing $\mathbf{F}=\mathbf{\nabla}\phi$ we have:
$$\int_{C}\mathbf{F}\cdot d\mathbf{r}=\int_{A}^{B}\mathbf{F}\cdot d\mathbf{r}=\int_{A}^{B}\boldsymbol{\nabla}\phi\cdot d\mathbf{r}=\phi(\mathbf{b})-\phi(\mathbf{a})$$
Hence the integral only depends on the value of $\phi$ at $A$ and $B$ and is independent of the path taken between them.
#### Example 4.6
![[Pasted image 20241012143344.png]]
We must use the previous force field:
$$\mathbf{F}=(2xy+z^{3},x^{2},3xz^{2})$$
![[WhatsApp Image 2024-10-12 at 14.41.27_aba98ae9.jpg|centre]]
#### Remarks
- The converse is also true; if  the work integral is independent of the path taken between any two points then there must exist a scalar potential function $\phi$ such that $\mathbf F=\boldsymbol \nabla \phi$
- If $C$ is a closed curve, then we can show that for a conservative vector field:
$$\oint_{C}\mathbf{F}\cdot d\mathbf r=0$$
- Force fields that are not conservative ($\boldsymbol{\nabla}\times\mathbf{F}\ne 0$) are called **non-conservative** or **dissipative**. An example is the force on a mass in a rotating frame due to angular acceleration $\mathbf{a}$:
$$\mathbf{F}=m\mathbf{a}=m\boldsymbol{\omega}\times\mathbf{r}$$
Then $curl F=2m\boldsymbol\omega$ and clearly from the physics the work done moving in such a force field is not independent of path.
### Summary
![[Pasted image 20241012144800.png]]