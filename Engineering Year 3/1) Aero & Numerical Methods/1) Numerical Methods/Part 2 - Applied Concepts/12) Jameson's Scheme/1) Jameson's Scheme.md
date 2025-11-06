We have seen previously, for the general finite-volume scheme, that we can obtain:
![[Pasted image 20251106130617.png|centre|400]]
And for a general discrete cell we have:
![[Pasted image 20251106130635.png|centre|250]]
Where $i$ is a cell counter. Hence we just need to loop over cell faces to compute the residual.
But how do we obtain the flux values $\mathbf{\underline{F}}_{k}$ and $\mathbf{\underline{G}}_{k}$ at the cell faces?

One method that has been developed uses "Central Discretisation" and was devised by Antony Jameson.
### Jameson's Central Discretisation
Jameson chose the most simple approximation. He evaluated the solution at each cell face using a simple average of the values either side:
![[Pasted image 20251106131124.png|centre|300]]
$$\mathbf{\underline{U}}_{BC}=\frac{1}{2}(\mathbf{\underline{U}}_{ij}+\mathbf{\underline{U}}_{i+1~j})$$
$$\mathbf{\underline{U}}_{DA}=\frac{1}{2}(\mathbf{\underline{U}}_{i-1~j}+\mathbf{\underline{U}}_{ij})$$
However we must be careful. The flux functions $\mathbf{\underline{F}}$ and $\mathbf{\underline{G}}$ are non-linear, and so:
$$\mathbf{\underline{F}}\left(\frac{1}{2}(\mathbf{\underline{U}}_{ij}+\mathbf{\underline{U}}_{i+1~j})\right)\ne \frac{1}{2}\left(\mathbf{\underline{F}}(\mathbf{\underline{U}}_{ij})+\mathbf{\underline{F}}(\mathbf{\underline{U}}_{i+1~j})\right)$$
### Central Discretisation
#### Cartesian Cell Case
Consider a structured cartesian cell, length $\Delta x$, height $\Delta y$, with a scalar equation:
![[Pasted image 20251106132044.png|centre|300]]
Assume: $\mathbf{\underline{U}}=u$, $\mathbf{\underline{F}}(\mathbf{\underline{U}})=cu$ where $c$ is a constant, and $\mathbf{\underline{G}}(\mathbf{\underline{U}})=0$.
For a cartesian cell $A=\Delta x \cdot \Delta y$, so the flux integral then becomes:
![[Pasted image 20251106132233.png|centre|400]]
So:
![[Pasted image 20251106132253.png|centre|450]]
Evaluating the fluxes at the faces:
![[Pasted image 20251106132323.png|centre|500]]

From our flux integration, we have:
![[Pasted image 20251106132345.png|centre|500]]
Then using a first order explicit approximation for the temporal derivative gives:
![[Pasted image 20251106132430.png|centre|350]]
But this is the FTCS finite-difference analogue for:
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=0$$
And this is unconditionally unstable.
### Artificial Dissipation
The basic Jameson method is now a very famous classical finite-volume method. The idea is simple but the basic method is unstable, and so to make it work in practice requires the addition of artificial dissipation (damping). Jameson spent a huge amount of time perfecting the dissipation. He added two types of dissipation:
1) Background 4th order dissipation: used always at all points in the flow
	This is sufficient to stabilise the flow, however large gradients (shocks) cause wiggles in the solution.
$$\epsilon_{4}\Delta x^{4}\frac{\partial ^{4}u}{\partial x^{4}},~~~\epsilon_{4}=\frac{1}{256}$$![[Pasted image 20251106132844.png|centre|200]]
2) A 2nd order term: used only at large gradients
	This has a large 
$$\epsilon_{2}\Delta x^{2}\frac{\partial ^{2}u}{\partial x^{2}}$$
![[Pasted image 20251106132913.png|centre|200]]
