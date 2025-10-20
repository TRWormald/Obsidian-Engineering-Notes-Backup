### Rigid body mechanics
The velocity of a rigid body $B$ rotating about a fixed axis can be described by angular velocity vector $\vec\omega$, where $\omega=|\omega|$ is the angular rotation speed (rad/s) and the direction $\hat\omega$ is the axis of (anti-clockwise) rotation. The velocity field at position $\vec{r}$ from the axis is given by:
$$\vec{v}(\vec{r})=\vec{\omega}\times\vec{r}$$
Then we can show that:
$$\text{div }\vec{v}=0,~~~~\text{curl }\vec{v}=2\vec\omega$$
that is, the curl of the velocity field has the direction of the axis of rotation and magnitude that is twice the angular speed of rotation
### Fluid mechanics
Let $\vec{v}$ be the velocity vector field of a fluid flow. Consider the following situations:
#### Example A
The below diagram shows linear simple shear flow between two plates in relative motion:
![[Pasted image 20241001153144.png|centre|400]]
$$\vec{v}=\left(\frac{Vy}{d},0,0\right)$$
$$\Rightarrow\text{ curl }\vec{v}=\left(0,0,-\frac{V}{d}\right)$$
$$\Rightarrow\text{ div }\vec{v}=0$$
This is a rotational ($\text{curl }\vec{v}\ne 0$), incompressible ($\text{div }\vec{v}=0$) flow. The rotation is perpendicular to the ($x,y$)-plane.
### Example B
Consider vortex flow:
![[Pasted image 20241001153545.png|centre|300]]
$$\vec{v}=\left(-\frac{y}{x^{2}+y^{2}},\frac{x}{x^{2}+y^{2}},0\right)=\frac{\hat{\vec\theta}}{r}$$
$$\Rightarrow\text{ curl }\vec{v}=\vec{0}$$
$$\Rightarrow\text{ div }\vec{v}=0$$
This is an irrotational, incompressible flow.
### Definitions
A vector field is said to be **incompressible** if:
$$\text{div } \vec{v}=0$$
A flow whose velocity field $\vec{v}$ is **curl free**, is called **irrotational**:
$$\text{curl } \vec{v}=\vec{0}$$
A force field $\vec{F}$ that satisfies $\text{curl }\vec{F}=\vec{0}$ is said to be **conservative.**

More generally it can be shown that $\text{curl } \vec{v}=\vec{0}$ if and only if:
$$\vec{v}=\text{grad }\phi, \text{ for some scalar field }\phi$$


