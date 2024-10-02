*In classical mechanics, the Kepler problem is to find the position and speed of two bodies over time given their masses, initial positions and velocities. The solution allowed scientists to show that planetary motion could be explained by classical mechanics and Universal Law of gravitation.*
\
#### Setup and Conservation of Momentum
The Kepler problem consists of to determining the radial and angular coordinates, of an object in a Keplerian orbit around the Sun as a function of time.
$\vec{v}_{r}$ is the radial velocity and $\vec{v}_{\theta}$ is the angular velocity. They are perpendicular:
![[Pasted image 20241002194012.png|centre|400]]
We use conservation of angular momentum to show that the motion is planar:
For large $r$ and small $m$, we can write:
$$\vec{L}=\vec{r}\times\vec{p}=\vec{r}\times m\vec{v}$$
or:
$$\vec{L}=\vec{r}\times m\vec{\dot{r}}$$
Where $\vec{L}$ is angular momentum, $\vec{r}$ is the position vector from the origin to the orbiting body, and $\vec{v}$ is the velocity vector of the orbiting body.
#### Looking at the rate of change of Angular Momentum
When we consider the rate of change of angular momentum we see:
$$\vec{\dot{L}}=\frac{d}{dt}(\vec{r}\times m\vec{\dot{r}})=(\vec{\dot{r}}\times m \vec{\dot{r}})+(\vec{r}\times m\vec{\ddot{r}})$$
The cross product of velocity $\vec{\dot{r}}$ and momentum $m\vec{\dot{r}}$ is zero, due to the fact that these vectors are parallel, so:
$$\vec{\dot{L}}=\vec{r}\times m \vec{\ddot{r}}=\vec{r}\times\vec{F}$$
However as $\vec{r}$ and $\vec{F}$ are also parallel, so:
$$\vec{\dot{L}}=0$$
Therefore the motion of $m$ is planar.
#### Specific Angular Momentum
We can obtain specific angular momentum by dividing $L$ by $m$, to obtain:
$$\vec{h}=\vec{r}\times\vec{v}$$
![[Pasted image 20241002200044.png|centre|400]]
The magnitude of $\vec{h}$ can be calculated to be:
$$h=|\vec{r}||\vec{v}|\sin\alpha$$
Where $\alpha$ is the angle between $r$ and $v$:
![[Pasted image 20241002200211.png|centre|300]]
We can also calculate it based on $\gamma$:
![[Screenshot 2024-10-02 201532.png|centre|300]]
Which is the "flight path angle" i.e. how much the velocity vector deviates from the tangent to the orbit:
$$h=|\vec{r}||\vec{v}|\cos\gamma$$
**Conservation of Momentum** means that for any point on an orbit:
$$r_{1}v_{1}\cos\gamma_{1}=r_{2}v_{2}\cos\gamma_{2}$$
Note that $\gamma=0$ at the periapsis and apoapsis.
\
##### Considering Circular Motion
When we consider circular motion:
$$v_{\theta}=r\omega=r \frac{d\theta}{dt}=r\dot{\theta}$$
As:
$$v_{\theta}=v\cos\gamma$$
Then:
$$h=rv\cos\gamma=rv_{\theta}=r\left(r\frac{d\theta}{dt}\right)=r^{2}\dot{\theta}$$
### Equation of Motion for 2 body system:
If we take the cross product of: