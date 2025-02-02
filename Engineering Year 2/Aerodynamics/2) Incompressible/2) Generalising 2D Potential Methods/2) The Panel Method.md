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
### 2D Source Panel Methods
Assumptions are made about the form of $\lambda_{s}$ on each panel - most commonly a constant or linear variation is used.
We then obtain a set of equations to solve for the panel source strength by applying a "surface is a streamline" condition at a discrete set of points on each panel, for example at the midpoints.

A simple approach assumes that $\lambda_{s}$ is a constant on each panel, but varies from panel to panel 