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
$$d\phi=-\frac{\gamma~ds}{2\pi}\theta$$
$$d\psi=\frac{\gamma~ds}{2\pi}\ln r$$
$$dV_\theta=-\frac{\gamma~ds}{2\pi r}$$
Then the velocity potential and steam function at point $P$ due to the whole sheet is:
$$\phi=-\int_{a}^{b}\frac{\gamma}{2\pi}\theta ~ds$$
$$\psi=\int_{b}^{a}\frac{\gamma}{2\pi}\ln r~ds$$
### Vortex Sheet Strength
The total circulation around a finite length of the sheet is:
$$\Gamma=\int_{a}^{b}\gamma~ds$$
The discontinuity in velocity across the sheet, which is the local jump in tangential velocity, is equal to the local sheet strength:
$$\gamma=v_{t1}-v_{t2}$$
![[Pasted image 20250202174836.png|centre]]
### 2D Vortex Sheet
![[Pasted image 20250202174903.png|centre]]
### Doublet Sheets
We can replace a vortex element by a doublet sheet element with an appropriate strength distribution.
e.g. A 2D flat panel with a constant vortex strength distribution could be replaced by a linear doublet strength distribution on the same panel (note the gradient of the doublet strength depends on the direction defined as the positive direction for the doublet).
### 2D Vortex Panel Methods
- An arbitrary body can be modelled by covering the surface with a vortex sheet
- The sheet strength $\gamma(s)$  is chosen so that the combined action of $\gamma(s)$ and the freestream velocity makes the surface a streamline. Also need to enforce a Kutta condition in order to ensure correct physical solution.
- This cannot be solved analytically for arbitrary bodies and is usually solved numerically using a panel method.
#### Constant Vortex Panel Methods
If there are N panels then to create a set of equations to solve for the constant panel strengths $\gamma_{j}$  , a “surface is a streamline” condition is applied at the control points. Gives $N$ equations.

We also need an equation to enforce the Kutta condition. In 2D one way this can be done is by setting:
$$\gamma_{1}+\gamma_{N}=0$$
We have $N$ unknowns but $N+1$ equations. Solve by deleting one of the control point equations or using a least squares approach.
#### Linear Vortex Panel Methods
There are $N$ panels with the strength of the panels specified at each end so $N+1$ unknowns. For panel $j$, panel strengths at ends are $\gamma_{j}$  and $\gamma_{j+1}$ there is then a linear variation in between, as shown for a source panel. A “surface is a streamline” condition is applied at control points on each panel giving N equations.

Again we need to enforce the Kutta condition using:
$$\gamma_{1}+\gamma_{N}=0$$
Now we have $N+1$ unknowns and $N+1$ equations.
### Lifting Flow Vortex Panel Solutions
![[Pasted image 20250202181154.png|centre]]
Note how the linear vortex panels are much more accurate at the peak of the negative pressure distribution curve, more accurately modelling the lift generated.
## From 2D to 3D
3D panel methods are very similar to 2D methods, after selecting a singularity type the same four steps are needed:
1) Geometry Discretisation
2) Calculation of Influence Coefficients and Influence Matrix equations
3) Solution of the linear set of equations
4) Secondary calculations: pressures, forces, off-body velocities etc.
### Point and Distributed Elements in 3D
![[Pasted image 20250202181414.png|centre]]
3D distributed element expressions are found by considering small element of a surface, using the 3D point singularity formula for the small element and then integrating over the surface.
### Surface Panelling
Paneling of 3D geometries is more complex, especially for complex geometries. Most commonly used approaches use quadrilateral or triangular panels, created from a mesh of points on the body surface.
![[Pasted image 20250202181453.png|centre]]
It is always possible to join 3 points on geometry with a fat panel, but 4 arbitrary points don't necessarily lie on a plane.
This means that curved panels are sometimes required, however:
- This makes the expressions for velocities induced by the panel and after the panel more complicated to evaluate
- There can be gaps between panels if the curved edges don't match exactly.

Sometimes the geometry is approximated so that flat panels can be used. This means there is some compromise on the accuracy of the representation so that the mash points are not necessarily lying on the true geometry and gaps can arise between panels. These cause "leakage" which causes errors in solutions.
### Wake Modelling
- A wing sheds vorticity into the wake. 
- It is crucial to shed the wake in the most physically realistic way to get the correct lift. 
- In steady 2D flow the Kutta condition is sufficient to get the correct lift. It implies conditions on pressure and velocity at TE, but we normally focus on the velocity when implementing it. 
- In 3D again want to shed the wake smoothly, but the Kutta condition is implemented via a pressure condition to allow for spanwise flow. Modelling of the wake behind the wing is also important. A 2D Kutta condition will work adequately if the wing is not highly swept. 
 - Will see more on wake modelling in a later lecture.
## Notes
Panel methods can be used for arbitrary shapes and extended easily to 3D
However:
- Only for low speeds
- No viscous effects
- No shocks
We can however extend their use using:
- Compressibility corrections
- Coupling to boundary layer solvers, aeroelastic representations, thermal effects, etc.