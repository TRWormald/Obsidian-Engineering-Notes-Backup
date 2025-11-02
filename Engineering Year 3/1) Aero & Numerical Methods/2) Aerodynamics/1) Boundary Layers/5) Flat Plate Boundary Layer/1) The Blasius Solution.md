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
$$u=(u_{e}x\nu)^{\frac{1}{2}}\frac{F'}{2}\left(\frac{u_{e}}{\nu x}\right)^{\frac{1}{2}}=\frac{u_{e}F'}{2}\Rightarrow\boxed{\frac{u}{u_{e}}=\frac{F'}{2}}$$
Similarly we can then differentiate the function of $\varphi$ again, but this time make it negative so we obtain $v$:
$$\Rightarrow-\frac{\partial\varphi}{\partial x}=-(u_{e}x\nu)^{\frac{1}{2}}\cdot F'(\eta)\frac{\partial\eta}{\partial x}-\frac{1}{2}\left(\frac{u_{e}\nu}{x}\right)^{\frac{1}{2}}\cdot F(\eta)$$
With the first auxiliary variable:
$$\eta=\frac{y}{2}\left(\frac{u_{e}}{\nu x}\right)^{\frac{1}{2}}\Rightarrow\frac{\partial\eta}{\partial x}=- \frac{1}{2x} \frac{y}{2}\left(\frac{u_{e}}{\nu x}\right)^{\frac{1}{2}}=-\frac{\eta}{2x}$$
Hence:
$$v=-\frac{\partial \varphi}{\partial x}=(u_{e} x \nu)^{\frac{1}{2}} \frac{\eta}{2x}F'- \frac{1}{2}(\frac{u_{e}\nu}{x})\cdot F$$
Or:
$$\boxed{v= \frac{1}{2}\left(\frac{u_{e}\nu}{x}\right)^{\frac{1}{2}}(F'\eta-F)}$$
### Lets Review
We want to solve the boundary layer equations for a 2D, steady, incompressible flow along a flat plate.
We then introduced two auxiliary variables $\eta$ and $\varphi$, and then solved for $u$ and $v$ using the stream functions.
### X-Momentum
We still need to solve for the derivatives of $u$ and $v$:
![[Pasted image 20251029153511.png|centre]]
Lets then observe the first term of this equation:
![[Pasted image 20251029153742.png|centre]]
And the second term:
![[Pasted image 20251029153801.png|centre]]
And the RHS:
![[Pasted image 20251029153822.png|centre]]
Therefore:
$$-\eta F' F''+\eta F'F''-FF''=F'''$$
i.e.
$$\huge{FF''+F'''=0}$$
Therefore we want a function that when multiplied by its second derivative with respect to $\eta$ is the negative of its third derivative. The form of this ODE can change depending on your initial choice of the definition of $\eta$. This ODE can be solved numerically and is quite simple to complete on computers - it can even be solved by hand.
The first to solve it was Blasius and hence it is named after him. It may be considered exact for incompressible, steady, 2D flow over a flat plate.
### Solving the Blasius ODE
$$\huge{FF''+F'''=0}$$
We know $F(\eta)$ and $\eta(x,y)=\frac{y}{2\delta}$, the boundary conditions are the key to solving the ODE. At the wall, $u=v=0$ due to the no slip, no-flux conditions.
$$F'(\eta=0)=0$$
$$F(\eta=0)=0$$
At the edge of the boundary layer $u=u_{e}$, and:
$$F'(\eta\rightarrow\infty)=2$$
This is still very difficult to solve analytically, so lets solve it numerically:
#### The Shooting Method
First we cast the third order ODE as three coupled first order ODEs:
$$F'(\eta)=G(\eta)$$
$$G'(\eta)=F''(\eta)=H(\eta)$$
$$H'(\eta)=F'''(\eta)=-F(\eta)F''(\eta)=-F(\eta)H(\eta)$$
The boundary condition gives us $F(0)=F'(0)=G(0)=0$, but we are still stuck because we don't have a value for $H(\eta=0)$. However we can employ an iterative approach known as the shooting method. 
This is where we find solutions to the initial value problem by changing the initial conditions until we find the solution that also satisfies the boundary conditions of the original boundary value problem.
1) Guess $F''(0)=H(0)$ and see if the trajectory allows us to find the correct $F'(\eta\rightarrow\infty)=2$ at the edge
2) Check the value of $F'$ at the edge and adjust $F''$
3) Repeat the process with the new value of $F''$
4) This is the equivalent to iterating on the wall shear stress.
![[Pasted image 20251029163407.png|centre]]
![[Pasted image 20251029163418.png|centre]]
This profile can be numerically integrated using definitions of momentum and displacement thickness to give:
$$\frac{\delta^{*}}{x}=\frac{1.721}{Re^{\frac{1}{2}}_{x}}~~~~~~\frac{\theta}{x}=\frac{0.664}{Re^{\frac{1}{2}}_{x}}$$
And the friction coefficient can be computed as:
$$c_{f}=\frac{\tau_{w}}{\frac{1}{2}\rho_{e}u_{e}^{2}}=\frac{0.664}{Re^{\frac{1}{2}}_{x}}=\frac{\theta}{x}$$
Where:
$$\tau=\mu\frac{\partial U}{\partial y}$$
Resulting in the drag coefficient on a one sided plate of length x being:
$$c_{d}=2c_{f}=\frac{1.328}{Re_{x}^{\frac{1}{2}}}$$
