>It is possible to describe all fluid flow using the **Navier-Stokes Equations**, be they 2D/3D, viscous/inviscid, steady/unsteady, compressible/incompressible.

However it is impossible to solve these equations analytically, so numerical methods have been researched for over 100 years.
### The 3-D Navier-Stokes Equations in a Fixed Axis System
![[Pasted image 20250923131254.png|centre]]
![[Pasted image 20250923131316.png|centre]]
![[Pasted image 20250923131331.png|centre]]
### Reduction of the Navier-Stokes Equations
>If we ignore the viscous effects we get the Euler equations:
![[Pasted image 20250923131602.png|centre]]

>If we assume steady flow we get the steady Euler equations

>And if we assume that the flow is irrotational we can introduce the velocity potential $\phi$ 
![[Pasted image 20250923131729.png|centre|400]]

>Finally we can assume isentropic flow to derive the full potential equation:
![[Pasted image 20250923132524.png|centre|400]]
>If we assume small perturbations we obtain a linear equation:
![[Pasted image 20250923132632.png|centre|400]]

Which is what programmes like XFoil or XFLR will solve.

