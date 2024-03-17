We've previously calculated the longitudinal (axial) stress in beams (See [[Longitudinal Stresses in Beams]]) and we can now calculate the shear stress distribution on the beam's cross section, based on:
- Longitudinal Stress Distribution
- Force Equilibrium
\
##### The Shear Stress along a Cut
![[Pasted image 20240227145327.png]]
Given the above diagram, the shear force $\tau$ is equal to:
$$\tau = \frac{F}{I\cdot B}\cdot \bar{y}\cdot A$$
Where:
$F$ is the shear force ($N$)
$I$ is the second moment of area **of the whole section** ($m^4$)
$b$ is the width **at the position of the cut** ($m$)
$\bar{y}$ is the position of the centroid of **the area below the cut**
$A$ is the **area below the cut**

##### The Shear Stress on the Cross Section
The above equation alone doesn't help us find the shear stress on the cross section, however if we consider the fact that the beam is in equilibrium we can use the concept of force equilibrium:
![[Pasted image 20240227150015.png|center|300]]
As the element is in equilibrium:
$$\tau_{AC}=\tau_{BD}=\tau_{AB}=\tau_{CD}=\tau_{}$$
And hence the same shear stress that develops in the cut also develops on the beam's cross section.
![[Pasted image 20240227150147.png|center|400]]
As a result with a slight redefinition of the variables for the original equation we can say that, given the following diagram:
![[Pasted image 20240227150301.png|center|400]]
$$\tau=\frac{F}{I \cdot b}\cdot \bar{y}\cdot A$$
Where:
$F$ is the shear force ($N$)
$I$ is the second moment of area of **the whole section**
$b$ is the width **at the position where we want to calculate $\tau$**
$\bar{y}$ is the position of the centroid of the **area below this position**
$A$ is the **area below this position**

##### Thin-Walled Sections
In thin-walled sections, the width is much larger than the thickness $b>>t_f$ and therefore the shear stresses perpendicular to the flange are very small and can be ignored $\tau_h>>\tau_v$, this can be seen below:
![[Pasted image 20240227174904.png|center]]
With objects consisting of two or more elementary sections we can consider each in turn:
![[Pasted image 20240227175128.png|center|400]]
With the shear stress in the flange being equal to:
$$\tau(s_f)=\frac{F}{I\cdot t_f}\cdot\bar{y_1}\cdot s_f \cdot t_f=\frac{F}{I}\cdot\bar{y_1}\cdot s_f$$
i.e. a linear distribution varying with $s_f$ as $\bar{y_1}$ is constant.
\
Whilst in the web:
$$\tau(s_w)=\frac{F}{I\cdot t_w}\cdot\bar{y_2}\cdot s_w \cdot t_w=\frac{F}{I}\cdot\bar{y_2}\cdot s_w$$
i.e. a parabolic distribution with $s_w$ as $\bar{y_2}$ is a linear function of $s_w$.
/
![[Pasted image 20240227180143.png|center]]
##### Examples of Shear Stress Distributions
![[Pasted image 20240227180228.png]]
![[Pasted image 20240227180239.png]]
\
![[Pasted image 20240227180248.png|center|400]]
