We know from the Euler-Bernoulli Beam Theory (See [[Longitudinal Stresses in Beams]]) that we can calculate the radius of curvature of a beam as follows:
$$\frac{1}{R}=\frac{M}{E\cdot I}=K$$
Where $K$ is the curvature and is equal to $\frac{1}{R}$
\
It can be shown that, for small displacements, the curvature is equal to the second derivative of the deflection $w(x)$.
Therefore:
$$\frac{d^2w}{dx^2}=\frac{M}{E\cdot I}$$
$$\frac{d^2w(x)}{dx^2}=\frac{M(x)}{E\cdot I}$$
So, the deflection can be calculated through:
$$w(x)=\iint\frac{M(x)}{E\cdot I}\cdot dx +C_1\cdot x+C_2$$
This does however mean that we'll need two boundary conditions to determine $C_1$ and $C_2$
Note that the first derivative of the bending moment is the curvature or rotation, which gives us another equation to solve for the constants:
$$w^{'}(x)=\int\frac{M(x)}{E\cdot I}\cdot dx +C_1$$
##### Examples of boundary conditions:

![[Pasted image 20240227182234.png|center]]
\
![[Pasted image 20240227182258.png|center]]

##### Superposition
When multiple loads are applied to a single beam we can solve for the deflections caused by each load separately and then combine them together:
![[Pasted image 20240227182725.png|center|500]]
##### Deflection Formulae
![[Pasted image 20240227182406.png|center]]
![[Pasted image 20240227182428.png|center]]
