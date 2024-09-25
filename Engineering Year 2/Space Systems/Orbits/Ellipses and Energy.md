### Some Orbital Terminology
Orbits have some specific terminology to describe certain parts of them. The furthest point from the orbited body is called the **Apoapsis** whilst the closest point is called the **Periapsis**.
These terms are the general - non specific - descriptors, however there are some for specific bodies:
- Apogee/Perigee - Earth
- Apolune/Perilune - Moon
- Apohelion/Perihelion - Sun
### Definition of an Orbit
An orbit is a closed or recurring path that a spacecraft or other body follows around another body.
All orbits have an eccentricity (which is also a property of ellipses) which describes it:
- For e<1 the orbit is closed with a recurring path (elliptical)
- For e>1 it is not an orbit - merely a passing trajectory (hyperbolic)
- For e=0 the orbit is circular
- For e=1 it is parabolic (parabolas are special cases of hyperbolas)

### Ellipse Expressions
$$\text{Periapsis Distance}~~~~~~~~r_{p}=a(1-e)$$
$$\text{Apoapsis Distance}~~~~~~~~r_{a}=a(1+e)$$
$$\text{Semi-major Axis}~~~~~~~~a=(r_{a}+r_{p})/2$$
$$\text{Semi-Minor Axis}~~~~~~~~b=a\sqrt{1-e^{2}}$$
$$\text{Eccentricity}~~~~~~~~e=\frac{r_{a}-r_{p}}{r_{a}+r_{p}}$$
$$\text{Area of Ellipse}~~~~~~~~A=\pi ab$$
$$\text{Equation of Ellispse}~~~~~~~~ \frac{x^{2}}{a^{2}}+ \frac{y^{2}}{b^{2}}=1$$
### The Sidereal vs Solar/Synodic Day
One solar day is the time taken for the Sun to come back to the same place - 24hrs
However due to orbital precession there is also another type of day that we can use - the sidereal day. This is the amount of time it takes for the stars to come back to the same position in the sky - 23hrs 56min. This is also the amount of time it takes for the earth to rotate.
![[Pasted image 20240917181424.png|centre|300]]
This fact is demonstrated in the diagram above.
*Note that satellites orbits are aligned to the Sidereal day - not the solar day*
### Newton's Universal Law of Gravitation
Newton's Law of Gravitation describes the force experienced between two objects due to their masses:
$$F_{12}=-\frac{Gm_{1}m_{2}}{r^{2}}\hat{\vec{r}}_{12}$$
Effectively the force between object 1 and 2 is proportional to the product of their masses - but inversely proportional to the square of the distance between them.
### Orbital Energy
We know that the total Energy 'E' of a system doesn't change therefore:
$$E=KE+PE$$
For space this is often written as:
$$E=K+U$$
Note that $U$ is defined as 0 at infinity so gravitational energy is always negative.
This means that gravitational potential energy increases as distance from earth's centre increases - whilst kinetic energy decreases.
By combining the equations for centripetal force and newton's second law we can derive:
$$K=\frac{1}{2} \frac{GMm}{r}$$
And so:
$$E=K+U$$
$$E=\frac{1}{2}mv^{2}- \frac{GMm}{r}$$
$$E=-\frac{GMm}{2r}$$
Which is the energy required for a circular orbit of radius $r$. As we can see larger orbits (higher $r$ values) require more energy due to the fact that it is negative.