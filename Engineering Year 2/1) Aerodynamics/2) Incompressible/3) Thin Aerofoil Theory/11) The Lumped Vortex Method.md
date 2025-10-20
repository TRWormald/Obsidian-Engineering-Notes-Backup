The thin aerofoil theory problem has a continuous $\gamma(s)$ distribution that requires an analytic solution: 
![[Pasted image 20250302171259.png|centre|300]]
>Is it possible to replace this entire continuous distribution with point or "lumped" vortices, so that viewed from the far field it looks the same. i.e. it predicts the same lift as full thin aerofoil theory?

### Simplifying the Thin Aerofoil Method
The general method we will develop is similar to the 2D generalised methods developed earlier, but with the location of singularities and control points linked to a panel representation of the geometry.

The camber line of the thin aerofoil will be split into a series of $N$ flat panels each with a point vortex on it.
A "no normal flow" condition is then applied on each panel and the set of equations solved for the vortex strengths in a similar way to previous panel method solutions.

The key question is:
**How do we get the correct lift?**
- A Kutta condition will need to be enforced
	- This can be done in a number of ways
		- Katz & Plotkin
		- Kuethe & Chow

When applying the new method we will usually just:
1) Place vortices
2) Apply boundary conditions
3) Solve for vortex strengths
The Kutta condition will not be directly applied - instead we will apply it indirectly or implicitly be enforcing suitable choices for the location of the singularities and control points.
**The appropriate locations are established by looking at the case of a think symmetric aerofoil with $N=1$**

For this aerofoil to have the same lift as thin aerofoil theory the circulation of the point vortex must equal the total circulation of the thin aerofoil vortex sheet.
Then we need to determine its location of the vortex and the control points to get this as a solution of the problem.

Since the lift of the thin symmetric aerofoil acts at the CP the point vortex, of strength $\Gamma$, is placed at the panel quarter chord point:![[Pasted image 20250302174109.png|centre]]
If we are solving this problem for the point vortex circulation there would be just one unknown $\Gamma$ so one boundary condition of no normal flow could be imposed on the panel.
This would fix the circulation. The choice of imposing this at the aerofoil (panel) trailing edge (i.e. where a Kutta condition is usually applied) would seem to be the intuitive choice. In fact this would mean that the method would not predict lift correctly.
We want the circulation to match:
$$\Gamma=\int_{0}^{c}\gamma(x)~dx,~~~~\gamma(\theta)=2\alpha V_\infty\frac{1+\cos\theta}{\sin\theta}$$
So instead of imposing no normal flow at the trailing edge, the same condition is applied at a control point somewhere else on the panel so that the lift is the same as that calculated using full thin aerofoil theory.

Thus, because the lift we want is known, the unknown is the location of the control point.
The situation is then as follows:
![[Pasted image 20250302174537.png|centre|300]]
![[Pasted image 20250302174555.png|centre|300]]
To impose the boundary condition the velocity normal to the chord line is needed. This is a combination of the velocity induced by the vortex and the freestream:
$$V_{\infty}\sin\alpha+w\approx V_{\infty}\alpha +w=0$$
Where $w$ is the vertical velocity at the control point due to the vortex:
$$w=V_{\theta}=-\frac{\Gamma}{2\pi r}=-\frac{\Gamma}{2\pi(kc-c/4)}$$
But now the equation appears to have two unknowns: $k$ and $t$.
But in this case the circulation must be the same as thin aerofoil theory in order to give the same lift therefore:
$$l=\rho_{\infty}V_{\infty}\Gamma=\pi \alpha c \rho_{\infty}V_{\infty}^{2}$$
Hence:
$$\Gamma=\pi \alpha c V_{\infty}$$
The zero normal velocity at $kc$ gives:
$$\frac{-\pi c V_{\infty}\alpha}{2\pi (kc-c/4)}+V_{\infty}\alpha=0~~~~\rightarrow~~~~\boxed{k=0.75}$$
So we have determined that if we had put the vortex at the quarter chord and the control point at the three quarter chord position and calculated the solution, then the circulation and lift would have been correct as they would match thin aerofoil theory.
### Lumped Vortex Approximation
The control point is sometimes called the aft neutral point. 
It effectively accounts for the Kutta Condition and gives surprisingly good results.
It is useful for preliminary calculations when precise details of local flow are not required, and gives reasonable approximations for lift, but detail of flow close to aerofoils is poor.

This extends into use in multiple panel cases i.e. $N>1$
Strictly speaking this is only valid in 2D, but it is widely applied ad hoc in 3D.

### General Lumped Vortex Method
When extending to approximate the flow past thin aerofoils using a set of panels; each panel has a point vortex at its panel quarter chord and a control point at its three-quarter chord.
![[Pasted image 20250302180126.png|centre]]
This is more accurate than using a single point vortex, but remains a cheap, simple method which can give good answers. The 3D extension of this method is called the vortex lattice method.
We can solve problems using the following:
$$\boxed{\mathbf{A\vec{\Gamma}=\vec{R}}}$$
Where:
$$\mathbf{\vec{\Gamma}}=[\Gamma_{1},\Gamma_{2},...,\Gamma_{N}]^{T}$$
$$\mathbf{\vec{R}}=[R_{1},R_{2},...,R_{N}]^{T}$$
From freestream:
$$R_{i}=-\vec{V}_{\infty}\cdot\vec{n}_{i}$$
$A$ is the velocity influence matrix with entries $a_{i,j}$.
![[Pasted image 20250302180522.png|centre]]

