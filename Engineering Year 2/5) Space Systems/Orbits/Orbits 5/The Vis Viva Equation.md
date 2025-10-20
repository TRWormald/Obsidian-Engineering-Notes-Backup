7.In space travel velocity is important, because to change it we need to use fuel. Using some of the properties of an ellipse, and the conservation of energy, we can find an expression for the velocity at any point in an orbit.
\
We have previously found the orbital energy to be:
$$E=\frac{1}{2}mv^{2}- \frac{GMm}{r}$$
And we can divide through by mass to get the specific energy of an orbit:
$$\varepsilon=\frac{1}{2}v^{2}- \frac{GM}{r}=\frac{1}{2}v^{2}- \frac{\mu}{r}=\boxed{(e^{2}-1)\frac{\mu^{2}}{2h}}$$
For an ellipse we also know that:
$$h^{2}=\mu a(1-e^{2})$$
So:
$$\varepsilon=(e^{2}-1)\frac{\mu^{2}}{2[\mu a(1-e^{2})]}$$
$$\varepsilon=\frac{\mu^{2}}{2a\mu}\frac{\cancel{e^{2}-1}}{(-1) \cancel{e^{2}-1}}=- \frac{\mu}{2a}$$
Which means that:
$$\boxed{\varepsilon=\frac{1}{2}v^{2}- \frac{\mu}{r}=- \frac{\mu}{2a}}$$
We can rearrange this for velocity:
$$\boxed{v=\sqrt{\mu\left[\frac{2}{r}- \frac{1}{a}\right]}}$$
### Special Case for Circular Orbits
For circular orbits we can assume that $r\equiv a$, so:
$$v_{c}^{2}=\mu\left[\frac{2}{r}- \frac{1}{r}\right]= \frac{\mu}{r}$$
Therefore the velocity of a circular orbit is inversely proportional to the square root of the altitude.
### Considering Parabolic Orbits
For a parabolic orbit, seen below, the escape velocity can be calculated to be:
![[Pasted image 20241009201649.png|centre|250]]
$$v_{esc}=\sqrt{\frac{2\mu}{r}}$$
Note that if we compare $v_{esc}$ with $v_{c}$, there is only a factor of $\sqrt{2}$ difference:
$$v_{esc}=\sqrt{\frac{2\mu}{r}}~~~~~~~v_{c}=\sqrt{\frac{\mu}{r}}$$
Thus the $\Delta V$ to escape on a parabolic orbit from a circular orbit is $(\sqrt{2}-1)v_{c}$.

