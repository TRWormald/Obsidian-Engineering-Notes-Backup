For 2D, steady, incompressible flow along a flat plate, with no pressure gradients in the external flow, the boundary layer equations are reduced to:
![[Pasted image 20251001110425.png|centre|500]]
The goal of Blasius is to reduce the PDE to an ODE to make it easier to solve.
With the assumption of no external pressure gradients the flow in the boundary layer is *similar*:
![[Pasted image 20251001110609.png|centre]]
This means that the velocity profiles are identical everywhere in the boundary layer - scaled by the thickness of the boundary layer.
This is because there are no gradients in the $x$ direction - and so there is no way for changes to occur, asides from the BL thickness.
#### The Auxiliary Variable $(\mathbf{\eta})$
If we introduce a new **auxiliary variable** $\eta$ which scales with boundary layer height, then $u$ for constant $\eta$ is constant.
So what is the equation for $\eta$?![[Pasted image 20251001110935.png|centre]]
$$\huge{\boxed{\eta=\frac{1}{2}y\left(\frac{u_{e}}{x\nu}\right)^\frac{1}{2}}}$$
#### Introducing The Stream Function
As we have incompressible flow, we know that the stream function exists (from continuity), i.e.
$$u=\frac{\partial\varphi}{\partial y}~~~~~~~~v=\frac{\partial\varphi}{\partial x}$$
With the continuity equation becoming:
$$\frac{\partial u}{\partial x}+\frac{\partial v}{\partial y}=\frac{\partial^{2}\varphi}{\partial x\partial y}-\frac{\partial^{2}\varphi}{\partial y\partial x}\equiv0$$
Which means we only need to find one variable, not two.
#### The Second Auxiliary Variable
With $\eta$ and $\varphi$ we can define a second auxiliary variable:
$$\varphi=(u_{e}x\nu)^{\frac{1}{2}} F(\eta)$$
Where $F$ is some function, then:
$$\Rightarrow \frac{\partial\varphi}{\partial y}=(u_{e}x\nu)^{\frac{1}{2}} F'(\eta)\frac{\partial \eta}{\partial y}+0\cdot F(\eta)$$
And with the first auxiliary variable equalling:
$$\eta=\frac{y}{2}\left(\frac{u_{e}}{\nu x}\right)^{\frac{1}{2}}\Rightarrow\frac{\partial \eta}{\partial y}=\frac{1}{2}\left(\frac{u_{e}}{\nu x}\right)^{\frac{1}{2}}$$
Hence: