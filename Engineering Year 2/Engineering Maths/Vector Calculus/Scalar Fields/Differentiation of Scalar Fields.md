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
