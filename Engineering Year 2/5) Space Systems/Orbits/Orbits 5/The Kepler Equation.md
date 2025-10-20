We have previously derived the [[The Kepler Problem#Equation of Motion for 2 body system|Orbit Equation]]:
$$r(\theta)=\frac{h^{2}/\mu}{1+e\cos(\theta-\omega)}=\frac{a(1-e^{2})}{1+e\cos\theta}$$
However it would be nice to find an expression for $r(t)$ and the easiest way to do this is by solving geometrically by introducing the concept of Eccentric anomaly $E$ and mean motion $n$.
![[Pasted image 20241009204005.png|centre|300]]
We can then obtain the Kepler Equation:
$$\boxed{M=n(t-t_{0})=E-e\sin E}$$
Where:
- $M$ is the mean anomaly (rad)
- $n$ is the mean motion (rad/s)
- $t-t_{0}$ is the time since periapsis (s)
- $E$ is the eccentric anomaly (rad)
- $e$ is the eccentricity
\
The mean anomaly $M$ is defined as the angle from periapsis of a body in a circular orbit with the same period.
If the spacecraft were travelling on the circle, its angular velocity would be equal to the mean motion:
$$\boxed{n=\sqrt{\frac{\mu}{a^{3}}}}$$
And true anomaly $\theta$ is related to eccentric anomaly through:
$$\boxed{\tan \frac{\theta}{2}=\sqrt{\frac{1+e}{1-e}}\tan \frac{E}{2}}$$

