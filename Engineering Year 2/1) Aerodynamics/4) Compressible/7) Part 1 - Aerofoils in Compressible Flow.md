### Recap
For large positive deflection angle $\theta$, flow expands through a series of infinitesimal Mach waves which form an isentropic expansion fan  that increases speed and decreases pressure.
**The deflection angle is related to the Prandtl-Meyer angle or function:**
$$\theta=v(M_{2})-v(M_{1})$$
**Mach waves** (expansion and compression) and oblique shock waves **are reflected** at **flow boundaries**.
### What Now?
We've looked at:
1) The basics of compressible flow
2) Shockwaves in compressible flow
So we will now cover:
3) Wings in compressible flow, looking at:
	1) Linearised 2D aerofoil theory
	2) Transonic 2D aerofoil behaviour
	3) 3D Compressible Flow
### The 2D Full Potential Equation
Consider steady 2D inviscid compressible flow over a body in a uniform stream which is isentropic and irrotational (the density is a variable). Irrotational flow means that the velocity field can be represented in terms of velocity potential $\phi$:
$$u=\frac{\partial \phi}{\partial x},~~~~~~v=\frac{\partial \phi}{\partial y}$$
Then to obtain an equation to solve for $\phi$, use continuity, momentum (1D Euler) and isentropic speed of sound ($dp=a^{2}d\rho$).

The resulting equation to solve is given by:
![[Pasted image 20250405122920.png|centre]]
This is a closed form in $\phi$ as $a$ is given by:
![[Pasted image 20250405122953.png|centre]]
Where $a_{0}$ is a known property of the flow.
We can then compare the full potential equation with the Laplace equation:
$$\frac{\partial^{2}\phi}{\partial x^2}+\frac{\partial^2 \phi}{\partial y^2}=0$$
From which we see that Laplace is linear whilst the full potential equation is nonlinear, so we can only solve it numerically and there is no superposition of solutions.
**As an alternative to numerical solutions look for algebraic solutions by considering small perturbations to free stream velocity and linearising.**
#### Linearising the 2D Full Potential Equation
Let's now assume that $u$ and $v$ are small perturbations to the free stream $V_{\infty}$. And consider the following diagram of the system:
![[Pasted image 20250405132048.png|centre|300]]
$$u=\frac{\partial \phi}{\partial x}=V_{\infty}+\hat{u}=V_\infty+\frac{\partial \hat{\phi}}{\partial x}$$
So:
$$\phi=V_{\infty}x+\hat\phi$$ $$v=\frac{\partial \phi}{\partial y}=\hat{v}=\frac{\partial\hat\phi}{\partial y}$$
**This is a very good approximation for thin bodies at a low AoA ($\alpha$)**
We can substitute perturbation velocity potential, $\hat\phi$ into the "Velocity Potential Equation" to give the "Perturbation Velocity Potential Equation":
![[Pasted image 20250405133138.png|centre]]
For a freestream Mach Number $M_{\infty}<0.8$ or $1.2<M_{\infty}<5$ (i.e. outside the transonic region) nonlinear terms are negligible, giving:
$$\boxed{\boxed{(1-M_{\infty}^{2})\frac{\partial^{2}\hat{\phi}}{\partial x^{2}}+\frac{\partial^{2}\hat\phi}{\partial y^{2}}\approx 0\Rightarrow(M_{\infty}^{2}-1)\frac{\partial^{2}\hat{\phi}}{\partial x^{2}}-\frac{\partial^{2}\hat\phi}{\partial y^{2}}\approx 0}}$$
This is the **Linearised Velocity Potential Equation**, for subsonic flow this equation can be transformed into an incompressible Laplace equation in a new space, for which analytic solutions are possible (Prandtl-Glauert), whilst for supersonic flow this can be shown to be a wave equation which can be solved analytically (Ackeret).
#### Linearised Compressible Pressure Coefficient
From the definition of the pressure coefficient we can make approximations for compressible flow similar to those used to derive the Linear Velocity Potential equation.
![[Pasted image 20250405133758.png|centre]]
The linearised incompressible pressure coefficient has the same final form starting from the incompressible flow pressure coefficient equation:
$$\boxed{C_{p}\approx -\frac{2\bar{u}}{V_{\infty}}}$$
#### Subsonic Prandtl-Glauert Correction 1
$$\boxed{\boxed{(1-M_{\infty}^{2})\frac{\partial^{2}\hat{\phi}}{\partial x^{2}}+\frac{\partial^{2}\hat\phi}{\partial y^{2}}\approx 0}}$$
Consider the linearised velocity potential equation. If we apply coordinate transformations in terms of the Glauert Factor $\beta=\sqrt{1-<M_{\infty}^{2}}$:
![[Pasted image 20250405134153.png|centre]]
In which case we can show that:
$$\boxed{\frac{\partial^{2}\hat\phi}{\partial\xi^{2}}+\frac{\partial^{2}\hat\phi}{\partial\eta^{2}}=0}$$
Which is the linear Laplace equation and identical to that solved for incompressible flow. We can solve this equation on the transformed geometry, noting that the angle of attack which was originally $\alpha$ is now $\hat\alpha=\beta\alpha$ in the transformed plane (small angles of attack have been assumed).
Then a compressible flow over an aerofoil of thickness ratio $t/c$ has the same pressure distribution but scaled by a constant as incompressible flow over an aerofoil with thickness ratio $(t/c)_{0}$ where $(t/c)_{0}=\beta(t/c)$ since:
![[Pasted image 20250405134613.png|centre]]
Usually, however, a new scaled potential is introduced such that:
$$\bar{\phi}=D\bar\phi\Rightarrow\boxed{\boxed{\frac{\partial^{2}\hat\phi}{\partial\xi^{2}}+\frac{\partial^{2}\bar\phi}{\partial\eta^{2}}=0}}$$
But why have we done this?
##### Why Did We Scale The Potential?
If we consider the angle of any streamline in the flow, and assume small perturbation velocities and angles, the flow velocity is tangent to the streamline. This means that for small angles and thin aerofoils the angle of the streamline is approximately the same. So to a linear approximation the streamlines including surface streamlines are the same shape, so can solve the incompressible flow over the same aerofoil. 
#### Subsonic Prandtl-Glauert Correction 2
Remembering the compressible pressure coefficient and expanding it gives us:
![[Pasted image 20250405142015.png|centre]]
Soi finally, if $\bar{u}=\frac{\partial\bar\phi}{\partial\xi}$ is the solution of Laplace's equation i.e. the incompressible solution on the same aerofoil:
$$C_{p}\approx -\frac{2\hat{u}}{V_\infty}=\frac{1}{\beta}\left(-\frac{2\bar{u}}{V_{\infty}}\right)$$
With the section inside the brackets being the "linearised incompressible $C_{p}$", which we can call $C_{p0}$ so that:
$$\boxed{\boxed{C_{p}\approx \frac{1}{\beta}C_{p0}}}$$
So we can relate pressure (and hence lift and pitching moment) to incompressible values for the same aerofoil geometry. This indicates that incompressible data for an aerofoil can be  corrected and used to give a good first guess in design.
**Note that:**
- This approach can extend to 3D, reduction to a Laplace equation on a scaled geometry is similar but the simplifications possible in 2D to use the same geometry don’t apply. 
- Since scaled incompressible Cp and only drag contribution as subsonic is from integral of pressure, hence D’Alembert’s paradox still applies.
So:
Due to the link between incompressible analysis and the Prandtl-Glauert correction, they have common features:
- Predicted drag = 0
- Aerodynamic centre is at 0.25c
The PG is not the only correction factor, there is also the Karmen-Tsien - which is better for unsteady aerodynamics.
#### Supersonic Linearised Ackeret Theory 1
Consider again the linearised velocity potential equation, but now for $M_{\infty}>1$ with no upstream interference. Remember that the thickness and $\alpha$ must be small:
![[Pasted image 20250405142729.png|centre]]
In this case the pressure coefficient can be related directly to the local surface inclination $\theta$ in radians (positive = into the flow) by:
$$\frac{dp}{d\theta}=\frac{\gamma M_{\infty}^{2}}{\sqrt{M_{\infty}^{2}-1}}p~~~~\Rightarrow~~~~\boxed{C_{p}=\frac{2\theta}{\sqrt{M_{\infty}^{2}-1}}}$$
##### Example Calculation
![[Pasted image 20250405142954.png|centre]]
#### Supersonic Linearised Ackeret Theory 2
Applying this to a flat plate 2D aerofoil at angle of attack $\alpha$ we get a constant pressure distribution.
![[Pasted image 20250405170641.png|centre]]
The lift and induced drag are:
![[Pasted image 20250405170701.png|centre]]
Note that supersonic flow Drag (wave drag) does not equal zero - D'Alembert's paradox doesn't apply.
We get the centre of pressure at 0.5c (vs 0.25 for incompressible)
The general approximate result for wave drag is:
$$\boxed{\boxed{C_{d}=\frac{\sqrt{M_{\infty}^{2}-1}}{4}C_{l}}}$$
Which we can use for most aerofoils at low $\alpha$.
##### Applications to Wedge Aerofoils
For a thin "double wedge" high speed section, linearised Ackeret theory gives:
![[Pasted image 20250405174617.png|centre]]
Note that there are now two components to the wave drag, one due to incidence and one due to thickness.
##### Why use Ackeret?
Ackeret provides convenient simplification for curved surfaces, especially where the angle may be a function of other variables.
In this case an integral is needed for Cl or Cd (taking appropriate force components for each one)
![[Pasted image 20250405174747.png|centre]]
#### Wave Drag
Energy is lost to the wave system shed by the aerofoil, hence the generation of Wave Drag - note that it occurs even in isentropic flow.
The previous two examples of the application of Ackeret theory show components due to incidence (which is lift dependent) and thickness.
In general, wave drag has three components due to:
- Lift
- Thickness
- Camber
And we build up the drag value by summing these components:
![[Pasted image 20250405175031.png|centre]]
#### Linearised 2D Aerofoil Characteristics
![[Pasted image 20250405175103.png|centre]]
What we can see is that the Ackeret (the black lines) come close to representing the actual (typical) values, especially where speeds are below M0.8 or above M1.2.
#### Real Supersonic Aerofoil Flows
![[Pasted image 20250405175339.png]]
Modelling shock waves is not possible using linearised small perturbation theory...
But using the analysis for flows with shocks shows rather small errors at low values of $\alpha$. Wave drag is mostly due to energy lost in expansion and compression of waves (as opposed to total pressure loss through oblique shocks).
## Revision
![[Pasted image 20250405175513.png|centre]]
