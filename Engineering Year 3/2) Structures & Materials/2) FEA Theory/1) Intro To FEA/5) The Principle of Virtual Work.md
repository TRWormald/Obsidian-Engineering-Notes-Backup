In Solid Mechanics special weak forms exist:
- The Principle of Virtual Displacements
- The Minimum Total Potential Energy

Before we consider the principle of virtual work, let's refresh our memory on what is meant by work.

### Work
Work is done when a force moves its point of application.
For a particle:
$$W=\mathbf{f}\cdot \mathbf d=\mathbf{f}^{T}\mathbf{d}$$
![[Pasted image 20251003153112.png|centre|400]]
### The Principle of Virtual Displacements
A particle is in equilibrium under the action of a system of forces if the total work done by the forces is zero for any virtual displacement of the particle:
$$\delta W=\mathbf{f}^{T}\delta \mathbf{d}=0$$
![[Pasted image 20251003153304.png|centre|300]]
A rigid body is in equilibrium under the action of a system of forces if the total work done by the forces is zero for any virtual displacement of the body:
$$\delta W_{t}=\delta W_{e}+\cancel{\delta W_{i}}=\delta W_{e}=0$$
The sum of the virtual work done on $A_1$ and $A_2$ is zero:
![[Pasted image 20251003153502.png|centre|400]]
For elastic bodies, the strain field over the deformable continuum makes $\delta W_{i}\ne 0$. Hence:
$$\delta W_{t}=\delta W_{e}+\delta W_{i}=0$$
![[Pasted image 20251003153755.png|centre]]
![[Pasted image 20251003153805.png|centre]]
![[Pasted image 20251003153814.png|centre]]
### The Principle of Minimum Total Potential Energy
![[Pasted image 20251003153840.png|centre]]
![[Pasted image 20251003153853.png|centre]]
![[Pasted image 20251003153904.png|centre]]
**Which is the weak form we were looking for!**
$$\int_{S}\mathbf{p}^{T}\delta\mathbf{u}~dS+\int_{V}\mathbf{b}^{T}\delta\mathbf{u}~dV=\int_{V}\mathbf{\sigma}^{T\delta\varepsilon}~dV$$
