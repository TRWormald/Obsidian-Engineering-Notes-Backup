If we want to calculate the angular acceleration of a rigid body under an applied net moment:
$$\sum M_O = I_O\ddot{\theta}$$
So the sum of the moments is equal to the moment of inertia times by the angular acceleration. Where:
$$I_O =\int r^2 \cdot dm$$
Effectively the moment of inertia is a function of distribution of mass of a body around the point of rotation.
##### The Parallel Axis Theorem
The moment of inertia depends on the axis of rotation $O$. We can calculate the moment of inertia around any point given we know the moment of inertia about the centre of gravity of the object (units $kg~m^2$), the mass of the object, and the distance between that point and the centre of gravity:
$$I_O=I_G+d^2m$$
##### The Moment of Inertia of a Rod/Bar
For a slender bar of length L and mass m (t<<L):
![[Pasted image 20240229155004.png|center|150]]
The moment of inertia around G:
$$I_G=\int y^2 \cdot dm = \int_{-L/2}^{L/2}y^2\frac{m}{L}\cdot dy = \frac{mL^2}{12}$$
The moment of inertia about its end:
$$I_O=\frac{mL^2}{12}+m\left(\frac{L}{2}\right)^2=\frac{mL^2}{3}$$
##### The Moment of Inertia of a Disk/Wheel#
For a **solid wheel** with radius R and mass m:
![[Pasted image 20240229155122.png|center|300]]
An infinitesimal element of mass:
$$dm=m\frac{dA}{A}=m\frac{2\pi r\cdot dr}{\pi R^2}=\frac{2m}{R^2}r\cdot dr$$
Moment of inertia around G:
$$I_G=\int_0^R r^2\cdot dm=\frac{2m}{R^2}\int_0^R r^3\cdot dr =\frac{mR^2}{2}$$
##### The Radius of Gyration
The radius of gyration is the distance from an axis at which the mass of a body may be assumed to be concentrated.
In other words it is the equivalent $I_G$ produced by placing a point mass $m$ at distance $k_G$ from the axis of rotation.
So:
$$I_G=mk_G^2$$
$$k_G=\sqrt{\frac{I_G}{m}}$$
For a solid wheel:       $k_G=R/\sqrt{2} \approx 0.71R$
For a spoked wheel:   $k_G \approx R$
#####
This means that we can now calculate the angular acceleration around the centre of mass from only the linear forces applied to a rigid body.
![[Pasted image 20240229160042.png|center]]
