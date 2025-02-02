### 2D Source Sheet
![[Pasted image 20250202165253.png|centre]]
As we've previously seen in [[1) Simple 2D Generalised Methods]] an arbitrary (non-lifting) body can be modelled by covering the surface with a source sheet.
The sheet strength $\lambda(s)$ is chosen so that the combined action $\lambda_{s}$ and the freestream velocity $U_{\infty}$ makes the surface a streamline i.e. no flow across it.

An analytic solution for $\lambda(s)$ for an arbitrary geometry is not possible, instead the surface is divided into a finite number of panels. In most implementations the panels are flat.
Note that for panel $j$:
$$length=\Delta s_{j}$$
The distribution of panels and hence the length of the panels $\Delta s_{j}$ must be specified. For an aerofoil constant length panels are not suitable. **More panels are needed at the leading and trailing edges.**
![[Pasted image 20250202165641.png|centre]]
### The Full Cosine Method
A frequently used method of spacing panels for an aerofoil is the full cosine method:
![[Pasted image 20250202165828.png]]
$$x=\frac{c}{2}(1-\cos\beta)$$
Angle $\beta$ takes values between 0 and $\pi$ and is incremented by a fixed amount of $\Delta\beta$ to get the panel locations.
*Note how with this method if you have a significant gradient you get more panels while if you have a relatively straight line you get more equal spacing.*
## 2D Source Panel Methods
### Constant Source Method
Assumptions are made about the form of $\lambda_{s}$ on each panel - most commonly a constant or linear variation is used.
We then obtain a set of equations to solve for the panel source strength by applying a "surface is a streamline" condition at a discrete set of points on each panel, for example at the midpoints.
#### A Simplistic Approach
A simple approach assumes that $\lambda_{s}$ is a constant on each panel, but varies from panel to panel. This is one of the first successful methods. 
![[Pasted image 20250202170501.png|centre]]
To create a set of equations to solve for the constant panel strengths $\lambda_{j}$, a "surface is a streamline" condition is applied at the control points. In the version shown here this is achieved by implementing a Neumann condition i.e. by setting the velocity normal to each panel to zero at the control points.
After obtaining the influence coefficients and applying boundary conditions (in a similar way to the point source method described in the last lecture), the linear set of equations to be solved is of the form:
$$\mathbf{A\vec{\lambda}}=\mathbf{\vec{R}}$$
Where:
$$\mathbf{\vec{\lambda}}=[\lambda_{1}+...+\lambda_N]^T$$
$$\mathbf{\vec{R}}=[R_{1}+...+R_N]^T$$
And $\mathbf{A}$ is a matrix with entries $a_i,j$ the influence coefficients.
#### Solution Costs of the Linear Equation
- All entries of the influence matrix (size $N^2$) are non-zero and its generally not symmetric.
- It is a computationally demanding problem as the number of panels increases
- Gaussian elimination to invert the matrix is not practical for large problems.
- Instead of this we use iterative techniques

#### Comparison of Constant Source Panel vs Point Sources
![[Pasted image 20250202171135.png]]
(The above is for a cylinder)
For aerofoils:
![[Pasted image 20250202171201.png|centre]]
### Linear Source Methods
Another common approach is to assume that $\lambda(s)$ varies linearly along a panel. The only difference in method is the calculation of the influence coefficients (which is beyond the scope of this course).
If we assume that value of $\lambda$ at the ends of each panel are equal to $\lambda_{j}$ and $\lambda_{j+1}$. Then the variation on the panel is:
$$\lambda(s)=\lambda_{j}+\frac{s-s_{j}}{\Delta s_{j}}(\lambda_{j+1}-\lambda_{j})$$
#### Constant vs Linear Panels
![[Pasted image 20250202174212.png|centre]]
Here we can see that there is a much more gradual change between the panels rather than the "stepped" approach.
## 2D Vortex Sheet
The vortex sheet is a line of "infinitesimal" vortices of strength $d\Gamma=\gamma~ds$
![[Pasted image 20250202174339.png|centre]]
Where $\gamma=\gamma(s)$ is the vortex strength per unit length along the sheet (this is sometimes referred to as the vorticity distribution).

The velocity potential, stream function, and tangential velocity at point $P$ due to an element of the sheet is:
$$d\phi=-\frac{\g}{}$$