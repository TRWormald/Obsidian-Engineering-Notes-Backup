Consider a scalar equation in 2D for simplicity:
$$\frac{\partial u}{\partial t}+a \frac{\partial u}{\partial x}+b\frac{\partial u}{\partial y}=0$$
For simplicity, assume we solve the equation on a cartesian mesh of constant spacing ($\Delta x$ and $\Delta y$ are constant) using a finite-difference implementation (finite-volume schemes follow similarly). The backward time, centred space implicit method gives:
![[Pasted image 20251113130507.png|centre|400]]
We can write our BTCS scheme in terms of differences:
![[Pasted image 20251113130554.png|centre]]
Recall that the right hand side is the residual, and that the implicit BTCS scheme applied to the 2D scalar equation results in a matrix equation where each row has five non-zero elemetns.
For non-scalar equations the matrix elements become blocks. For example, a 2D system of four equations would result in a block pentadiagonal matrix where each of the five blocks is a 4x4 matrix.
### Computational Cost
To exactly solve a $n\times n$ matrix with bandwidth $b$ then the number of operations required is given by:
$$N_{op}=\frac{1}{12} (b^{2}-1)(3n-b)$$
Hence going from a tri- to pentadiagonal matrix for a realistic mesh dimension means approximately three times the number of operations.
Similarly, going to three dimensions results in a septadiagional matrix and approximately six times the work.
Direct solutions of the matrix equation is not often used even for scalar equations. For systems of equations, almost never.
![[Pasted image 20251113131040.png|centre]]However, this analysis is too optimistic because bandwidth does not equal the number of non-zero elements in each row.

>**Bandwidth of a Matrix**
>The largest number of columns separating the first and last non-zero elements in any row.

![[Pasted image 20251113131202.png|centre]]
![[Pasted image 20251113131220.png|centre]]
For a general 2D mesh, $NI\times NJ$ the bandwidth is actually $2NI+1$

The dimension of the implicit system $n$ is the number of grid cells times the number of equations:
$$NI\times NJ \times NK \times N_{eqn}$$
The cost of solving the matrix system is proportional to the matrix dimension $n$ times the square of the matrix bandwidth $b$.
But the matrix bandwidth $b$ is also a function of the grid dimensions, since we must store grid points in a 1D vector.

Hence, exactly solving the implicit system very quickly becomes too computationally expensive to consider.
*But do we need to solve the matrix exactly?*
