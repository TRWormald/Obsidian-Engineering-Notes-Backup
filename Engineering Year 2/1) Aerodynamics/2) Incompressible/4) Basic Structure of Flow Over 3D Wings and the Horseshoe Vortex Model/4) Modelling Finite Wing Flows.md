We know that the Navier-Stokes equations describe the 3D flow over a finite wing. It is not possible to solve these analytically so we need to simplify them.

Methods for modelling 2D flows over lifting aerofoils have already been covered, and they can be extended into 3 dimensions.

Before trying to construct a 3D flow model we need to consider the 3D equivalent of the point vortex and the vortex sheet:
### Vortex Filaments and Sheets
Point vortex flow becomes a vortex filament in 3D flow:
![[Pasted image 20250310173813.png|centre]]
While a 2D vortex sheet becomes a 3D vortex sheet:
![[Pasted image 20250310173842.png|centre]]
### Helmholtz Theorems for Vortex Filaments
The Helmholtz Vortex Theorems are:
1) The strength of a vortex filament is constant along its length
2) A vortex filament cannot start or end in a fluid
	Therefore it must form a closed path or extend to the fluid boundaries including infinity.
	![[Pasted image 20250310180018.png|centre|200]]
	![[Pasted image 20250310180037.png|centre|300]]
### Biot-Savart Law for Vortex Induced Velocities
The velocity induced by a vortex filament element $\mathbf{dl}$ is given by:
$$\mathbf{dV}=\frac{\Gamma}{4\pi}\frac{\mathbf{dl \times r}}{|\mathbf{r}|^{3}}$$
![[Pasted image 20250310180254.png|centre|300]]
*Note that this law is a general result for potential theory.*
### Biot-Savart Law for Straight Filaments
There are also some simplified laws for straight filaments:
![[Pasted image 20250310181647.png|centre|200]]
**For a Finite Vortex Element**
$$V=\frac{\Gamma}{4\pi h}(\cos\alpha+\cos\beta)$$
**For an Infinite Vortex Element, $\alpha=\beta=0$**
$$V=\frac{\Gamma}{2\pi h}$$
**For a Semi-Infinite Vortex Element, $\beta=0$**
$$V=\frac{\Gamma}{4\pi h}(1+\cos\alpha)$$
**For a Semi-Infinite Vortex Element, P, level with the end of the vortex, $\alpha=90,~\beta=0$**
$$V=\frac{\Gamma}{4\pi h}$$
