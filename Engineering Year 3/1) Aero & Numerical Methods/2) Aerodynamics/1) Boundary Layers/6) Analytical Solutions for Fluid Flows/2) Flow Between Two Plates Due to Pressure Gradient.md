### Flow due to Pressure Gradient Between Two Fixed Plates
#### Assumptions
The assumptions we make are:
- 2D, incompressible, plane, viscous, axial flow
- Zero gravity effects, flow driven by pressure gradient
- Fully developed flow (sufficiently far from entrance.
![[Pasted image 20251029213655.png|centre|400]]
Again from continuity we can obtain that $u=u(y)$. And again reduce the momentum equations to:
$$\mu \frac{\partial^{2}u}{\partial y^{2}}=\frac{\partial p}{\partial x},~~~~~~\frac{\partial p}{\partial y}=\frac{\partial y}{\partial z}=0$$

Hence:
$$\mu\frac{\partial^{2}u}{\partial y^{2}}=\frac{\partial p}{\partial x}=constant<0$$
Integrating twice with respect to $y$ gives us:
$$u=\frac{1}{\mu}\frac{dp}{dx} \frac{y^{2}}{2}+C_{1}y+C_{2}$$
To solve this equation we apply the boundary conditions:
$$\begin{align*}
y&= +h \Rightarrow u=0\\\\
y&= -h \Rightarrow u=0
\end{align*}$$
And obtain:
$$u=\frac{1}{\mu}\frac{dp}{dx}\frac{h^{2}}{2}+C_{1}h+C_{2}$$
$$u=\frac{1}{\mu}\frac{dp}{dx} \frac{h^{2}}{2}-C_{1}h+C_{2}$$
This means that:
$$C_{1}=0,~~~~~~~~C_{2}=- \frac{1}{\mu}\frac{dp}{dx}\frac{h^{2}}{2}$$
Therefore the solution is:
$$u=-\frac{dp}{dx}\frac{h^{2}}{2\mu}\left(1-\frac{y^{2}}{h^{2}}\right)$$
