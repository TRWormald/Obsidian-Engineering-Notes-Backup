Lets consider a steady 2D flow over a flat plate in the $x$ direction:
![[Pasted image 20250924110528.png|centre]]
Lets also consider the **Wall Boundary Conditions**:
At the wall $y=u=v=0$, and hence:
$$\cancel{u\frac{\partial u}{\partial x}}+\cancel{v\frac{\partial u}{\partial y}}=-\frac{1}{\rho}\frac{dp}{dx}+\nu\frac{\partial^2u}{\partial y^2}$$$$\frac{dp}{dx}=\mu\left(\frac{\partial^{2}u}{\partial y^{2}}\right)_\text{wall}$$

Lets also consider the **Edge Boundary Conditions**:
At the boundary layer edge $u=u_{e}$, derivatives w.r.t $y=0$ (by definition of the boundary layer edge) Hence:
$${u\frac{\partial u}{\partial x}}+\cancel{v\frac{\partial u}{\partial y}}=-\frac{1}{\rho}\frac{dp}{dx}+\cancel{\nu\frac{\partial^2u}{\partial y^2}}$$
$$\frac{dp}{dx}=-\rho_{e}u_{e}\frac{du_{e}}{dx}=\boxed{\mu\left(\frac{\partial^{2}u}{\partial y^{2}}\right)_\text{wall}}$$
In a uniform flow over a flat plate there is no pressure gradient, so:
$$\frac{dp}{dx}=0$$
And hence:
$$\left(\frac{\partial^{2}u}{\partial y^{2}}\right)_\text{wall}=0$$
This makes it a special case, reducing the number of boundary conditions to be solved - and allows an accurate solution to be derived.

