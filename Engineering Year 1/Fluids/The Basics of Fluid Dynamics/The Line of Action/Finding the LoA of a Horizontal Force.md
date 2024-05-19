When finding the Line of Action of a horizontal force applied by a fluid we need to consider several factors:
1) If the surface is not flat (unlike in the example below) we must consider its projected area - as we treat the fluid "trapped" between an imaginary vertical plane and the surface as static and hence the forces on that plane must be equal to the forces on the surface.
2) Unlike with the [[Finding the LoA of a Vertical Force|line of action of a vertical force]] we can't use the centroid of the object as this would produce a moment about that point due to the uneven distribution of forces above and below that point - as a result we have to use a point below the centroid.
![[diagram-20240519 2.png|center|500]]
We can define the moment about the centroid as:
$$M_x=F_{h}(h_{cp.}-h_{c})=\iint_{A}zp\cdot dA=-\rho gI_{xx}$$
We can then rearrange this to get:
$$\large\boxed{h_{cp.}=h_{c}+\frac{\rho g I_{xx}}{F_{h}}}$$
Where $h_{cp.}$ is the height below the surface of the fluid of the centre of pressure, $h_{c}$ is the height of the centroid below the surface, $\rho$ is the density of the fluid, $g$ is the acceleration due to gravity, $I_{xx}$ is the second moment of area of the surface, and $F_{h}$ is the horizontal force exerted on the surface.