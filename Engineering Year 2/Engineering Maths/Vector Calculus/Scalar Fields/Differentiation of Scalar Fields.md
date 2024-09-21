Lets consider the level curves of a scalar field in 2D, for example a heightmap, the gradient (or slope) is going to be different depending on the path taken over the contours.
We can calculate the gradient or rate of change of slope along any path. So clearly the differential of a scalar field (which is $\phi(x,y,z)$) must itself be a vector.
**Gradient Vector:**
$$\text{grad }\phi=\frac{\partial\phi}{\partial x}\vec{i}+\frac{\partial\phi}{\partial y}\vec{j}+\frac{\partial\phi}{\partial z}\vec{k}$$
Note that:
- The quantity $\text{grad }\phi(x,y,z)$ is a vector field
- Its magnitude $|\text{grad }\phi|$ is the maximum rate of change of $\phi$ 
- It points in the direction of the maximal rate of change of $\phi$; i.e. along the normal vector to the level surface $\phi = const.$
\
To help us understand grad $\phi$, let us consider a directional derivative $D_{a}$ if a scalar field $\phi(x,y,z)$ at a point $\vec{p}$ in a direction $\vec{a}$:
$$D_{a}\phi(\vec{p})=\frac{d\phi(\vec{r}(t))}{dt},~~~~~~~~\vec{r}(t)=\vec{p}+t\vec{\hat{a}}$$

Doing some algebra gives us:
$$D_{a}\phi=\vec{\hat{a}}\cdot \text{grad }\phi$$
Or in other words the gradient in the direction of $\vec{a}$ is equal to the dot product of the unit vector in that direction and $\text{grad }\phi$. 
**This leads us to:**
$$\vec{\nabla}=\frac{\partial}{\partial x}\vec{i}+\frac{\partial}{\partial y}\vec{j}+\frac{\partial}{\partial z}\vec{k}$$
Where $\vec{\nabla}$ 'del' is the **vector differential operator**, and $\text{grad }\phi =\vec{\nabla} \phi$.

### Applications of Gradient
#### Equation for the tangent plane to a surface.
Consider a scalar field $f(x,y,z)$, $\vec{\nabla} f$ is perpendicular to the level surfaces of that field so therefore if we can write a surface as $f(x,y,z)=c$ then the normal is:
$$\vec{n}=\vec{\nabla}f$$
So that the equation for the tangent plane at a point $P$ with position vector $\vec{r}=\vec{r}_{0}$ is:
$$(\vec{r}-\vec{r}_{0})\cdot \vec{n}=0 \Rightarrow (\vec{r}-\vec{r}_{0})\cdot\vec{\nabla}f|_{\vec{r}=\vec{r}_{0}}=0$$
#### Temperature and Pressure
If $\phi$ is a temperature field, then heat flows in the direction $-\vec{\nabla}\phi$. Similarly, if $\phi$ is a pressure field, the wind blows in the direction $-\vec{\nabla}\phi$ in which pressure decreases the most.
#### Force and Potential Energy
We know from 1D that '$F=\frac{dV}{dx}$' where $V$ is a potential (the work associated with moving against a potential energy $-V$). How does this apply in more dimensions?
$$\vec{F}=\text{grad }V$$
i.e. force is in the direction of maximum increase in potential.
This applies quite generally, e.g.
- In elasticity and stress analysis where $V$ is the strain energy and $\vec{F}$ the corresponding stress
- To electrostatic force $\vec{E}$ between two particles of charge $Q_{1}$ and $Q_{2}$ being the gradient of the electrostatic potential $f$ (measured in volts)
- To gravitational force $\vec{F}$ where $V \propto 1/r$ is the gravitational potential.