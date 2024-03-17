When a load is not applied through the [[Centroid]] of the section we instead replace this load with a load through the [[Centroid]] and a moment due to eccentricity:
\
![[Pasted image 20240221195054.png]]
\
$$M=P \cdot e$$
\
Where:
$M$ is the moment created due to the eccentricity ($Nm$)
$P$ is the applied load ($N$)
$e$ is the eccentricity ($m$)
\
Stress at any location results from the stress due to the direct load and the stress due to the moment:
\
![[Pasted image 20240221195116.png]]
\
![[Diagram 1.png]]\
This results in:
\
$$ \sigma = -\frac{P}{A}-\frac{M}{I}z$$
\
Where:
$\sigma$ is the stress at a given value of $z$ (from the neutral axis) on the element's cross section ($Pa$)
$P$ is the load applied ($N$)
$A$ is the cross sectional area ($m^2$)
$M$ is the moment due to the eccentricity of the load ($Nm$)
$I$ is the [[Second Moment of Area]] ($m^4$)
\
However this formula only works if the load is placed along one of the axes, if it is placed eccentrically with respect to both axes:
\
![[Pasted image 20240221195447.png]]
\
Resulting in:
\
$$ \sigma = -\frac{P}{A}-\frac{M_z}{I_{zz}}y-\frac{M_y}{I_{yy}}z$$
\
Note: We can calculate $\sigma_{min}$ and $\sigma_{max}$ using $y_{min}$ , $y_{max}$ , $z_{min}$ , and $z_{max}$
\
\
Sometimes it is required that $\sigma < 0$ all over the section (i.e. it is in compression) - this is mainly true for concrete structures as they have very poor tensile strength.
\
So, for this to be the case:
\
$$ \frac{e_z}{b/6} + \frac{e_y}{d/6} < 1 $$
Given that the cross section of the column is as follows:
\
![[Pasted image 20240220111743.png|500]]
\
This means that the load $P$ should be applied within the following region:
\
![[Pasted image 20240221195515.png]]
\
This is called the 'Middle Third Rule'
