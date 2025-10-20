>Time marching is used to predict the evolution of the flow, but at a *discrete set of points*, and over *discrete time periods*. This means that we can abandon the need to seek continuous functions as a solution to fluid flow problems!

To do this we introduce a labelling notation:
![[Pasted image 20251002132530.png|centre]]
![[Pasted image 20251002132540.png|centre]]
The continuous function $u(x,t)$ is modelled by a finite number of point values:
$$\huge{u(i\Delta x, n\Delta t)=u_{i}^{n}}$$
Where:
$i$ is the spatial mesh point counter
$n$ is the time level counter

Clearly our time-marching problem is how do we relate $u_{i}^{n+1}$ to $u_{i}^{n}$ for each mesh point $i$.
![[Pasted image 20251002132743.png|centre]]
Can we define an equivalent equation involving the solution values at our discrete mesh points? This is known as discretising the equation.
The trick is to use Taylor Series expansions. We have the solution $u$ stored at the points on a computational grid.

Consider expressing $u_{i+1}^{n}$ in terms of quantities at time level $n$:
![[Pasted image 20251002132934.png|centre]]
![[Pasted image 20251002132953.png|centre]]
![[Pasted image 20251002133013.png|centre]]
![[Pasted image 20251002133024.png|centre]]
![[Pasted image 20251002133033.png|centre]]
![[Pasted image 20251002133150.png|centre]]
### Arbitrary Stencils
[[Numerical Methods Lecture 4.pdf#page=20|Numerical Methods Lecture 4, p.20]]
>Stencils of arbitrary order can be constructed for any derivative through construction of an appropriate linear system.