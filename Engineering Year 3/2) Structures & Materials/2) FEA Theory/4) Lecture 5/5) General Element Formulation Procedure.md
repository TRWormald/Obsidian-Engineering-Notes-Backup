The procedure for element formulation described so far becomes increasingly complicated for increasingly complicated elements. Elements can be higher order and have more nodes. They can have irregular shapes and curved boundaries. And $\bar{\phi}$ becomes difficult to invert symbolically. And volume and boundary integrals are too complex to compute analytically.

Generally applicable interpolation functions were developed for regularly shaped elements, called master elements.
Mapping from the actual to master element and from master to actual are defined.
And we also need numerical integration.
### Lagrange Shape Functions
The most common interpolation functions for finite element formulation are the Lagrange Shape Functions.
For a 1D element with $n$ nodes, $n$ Lagrange shape functions, $N_{i}(\xi)$, can be defined:
![[Pasted image 20251024152759.png|centre]]
Where the $\xi_{i}$ is the coordinate of the $j^{th}$ node.
Note that $N_{i}(\xi)$ are functions of degree $n-1$ and zero at all nodes except the $i^{th}$.
### Numerical Integration
The exact evaluation of the integrals:
![[Pasted image 20251024152914.png|centre]]
is not always possible. Therefore integrals are evaluated numerically with procedures known as numerical integration, numerical quadrature, or Gaussian quadrature.
These involve approximating the integrand by a polynomial of sufficient degree. In 1D:
![[Pasted image 20251024153049.png|centre|400]]
This should look familiar. It is a finite element interpolation of $F(x)$, where:
- $F(x_i)$ denotes the values of $F(x)$ at the $i^{th}$ evaluation point $x_{i}$
- $\psi_{i}(x)$ are polynomials of degree $N-1$ 
	- Linear interpolation: polynomial order 1
	- Quadratic interpolation: polynomial order 2

In general quadrature formulae have the form:
![[Pasted image 20251024153244.png|centre]]
Evaluation points, $x_{i}$ are called quadrature points or integration points. The coefficients $W_{i}$ are called quadrature weights. They are usually tabulated as they depend on the functions $\psi_{i}$ and on the domain of integration, not on $F(x)$.

Of all options, the Gauss-Legendre quadrature is the most commonly used. It is based on Legendre polynomials.
![[Pasted image 20251024153437.png|centre|400]]
These are complete and orthogonal, but defined in $[-1,1]$. This requires mapping of the domain of integration from the global to a normal or master coordinate system.
![[Pasted image 20251024153534.png|centre]]
