An **eigenvector** of a $n\times n$ matrix $A$ is a nonzero vector $\vec{x}$ such that:
$$A\vec{v}=\lambda\vec{v}$$
For some scalar $\lambda$, where $\lambda$ is called an **eigenvalue** of $A$.
Hence, an eigenvector is a vector transformation, which when applied to a matrix, creates a scaled version of itself.
### Finding Eigenvalues
To find the eigenvalues of a square matrix you must solve the equation:
$$\det(A-\lambda I)=0$$
Where as above, $\lambda$ is an eigenvalue, $A$ is some square matrix, and $I$ is the identity matrix.
This will give a polynomial which can be solved to give all of the eigenvalues of the matrix.
### Finding Eigenvectors
Eigenvectors can be found by plugging in the known eigenvalues of a matrix into the equation:
$$(A-\lambda I)\vec{v}=0$$
And solving for $\vec{v}$.
