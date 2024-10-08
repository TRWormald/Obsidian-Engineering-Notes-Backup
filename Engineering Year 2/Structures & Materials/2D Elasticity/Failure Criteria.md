When does a material fail under combined loading conditions?
How do we extrapolate from uniaxial tests to compound stress states?
How do we account for different failure mechanisms: ductile and brittle.
\
We assume that a material is elastic after which it fails suddenly or yields plastically.
The goal is to define a yield envelope that separates elastic from plastic deformation; any stress state within its boundaries is elastic. We will define this in terms of principal stresses.
\
### Failure @ Maximum Principal Stress
This is failure when maximum principal stress reaches a critical value.
![[Pasted image 20241008223745.png|centre|400]]
This applies quite well to failure of brittle materials such as ceramics and cast iron.
### Failure @ Maximum Principal Strain
This is failure when maximum principal strain reaches a critical value.
![[Pasted image 20241008223952.png|centre|400]]
### Failure @ Maximum Shear Stress
This is failure that occurs when maximum shear stress reaches a critical value.
This is also sometimes known as the Tresca yield criterion.
Experiments on annealed metals showed that spherical stress doesn't cause yield.
Therefore it is the difference in principal stresses that drives failure (i.e. the diameter of Mohr's circle).
\
![[Pasted image 20241008224316.png|centre|400]]
We can obtain the critical values as follows:
From uniaxial tensile tests $\sigma_{2}=\sigma_{3}=0$, so:
$$\tau_{critical}=\frac{|\sigma_{1}-\sigma_{2}|}{2}=\frac{\sigma_{Y}}{2}$$
### Maximum Distortion Energy
According to the Von Mises yield criterion:
Failure occurs when deviatoric strain energy reaches critical value.
![[Pasted image 20241008224733.png|centre]]
$$\sigma_{1},\sigma_{2},\sigma_{3}=\text{mean stress }\sigma_{m}+\text{deviatoric components }\sigma_{i}'$$
$$\text{mean/hydrostatic stress}: \sigma_{m}=\frac{1}{3}(\sigma_{1}+\sigma_{2}+\sigma_{3})$$
The total strain energy per unit volume due to principal stresses is given by:
$$\hat{U}_{total}=\sum\limits_{i=1}^{3} \frac{1}{2}\sigma_{i}\varepsilon_{i}$$
