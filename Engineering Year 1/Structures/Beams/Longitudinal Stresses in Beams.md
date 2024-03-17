We know that bending moments come from tensile and compressive forces in the beam, however we didn't explain how to model these. The diagram below shows this:
![[Pasted image 20240227115734.png#center|400]]
It is possible to determine the actual stress by considering an infinitesimal section of the beam and solving using the facts of stress equilibrium, strain compatibility, and elasticity - however this is horrendously complicated and results in partial differential equations. And as a result we use a simpler method.
##### Basic Derivation
The more simple way that we use to approximate stress is the __Euler-Bernoulli Beam Theory__.
Its base assumption is that:
![[Pasted image 20240227120138.png]]
In the case of an **Elastic Beam**, with **H<<L** , considering **Small Deflections** and with **Zero Shear Force**: *Planar sections remain planar and perpendicular to the beam's axis*
This results in a very small error:
![[Pasted image 20240227120328.png]]
\
The entirety of the theory is based around the concept of the 'neutral axis' which is the line along which there is no tension or compression.
The neutral axis passes through the [[Centroid]] of the beam and is perpendicular to the applied load:
![[Pasted image 20240227120828.png]]
Where the dashed line is the neutral axis, and the image on the right is the cross section of the beam.
\
Deriving the equation from the fact that $\sigma (y)=\frac{E\cdot y}{R}$ gives the stress at any given point from the neutral axis and that the total force must be zero, and hence $F=\int dF=\frac{E}{R}\int y \cdot dA=0$. So the moment about the neutral axis is $dM=y\cdot dF$ and the total moment is $M=\frac{E}{R}\int y^2\cdot dA=\frac{E\cdot I}{R}$. This also leads to the fact that the radius of curvature is equal to $R=\frac{E\cdot I}{M}$.
And putting all of these together we get:
##### The Euler-Bernoulli Beam Theory:
\
$$\frac{M}{I}=\frac{\sigma}{y}=\frac{E}{R}$$
Where:
$M$ is the bending moment ($Nm$)
$I$ is the [[Second Moment of Area]] of the cross section ($m^4$)
$\sigma$ is the longitudinal stress ($Pa$)
$y$ is the distance from the neutral surface/axis ($m$)
$E$ is the [[Young's Modulus]] of the material ($Pa$)
$R$ is the radius of curvature ($m$)
\
With the diagram below being a good example of how this is likely to look:
![[Pasted image 20240227121750.png#center|400]]
\
It is now possible to calculate:
\
1) The maximum stress:
$$\sigma_{max}=\frac{M_{max}\cdot y_{max}}{I}$$
2) The radius of curvature:
$$R=\frac{E\cdot I}{M}$$


