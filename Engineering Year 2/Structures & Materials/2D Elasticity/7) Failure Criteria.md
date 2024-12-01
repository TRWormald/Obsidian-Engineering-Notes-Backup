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
Using Hooke's Law: $\varepsilon_{1}=\frac{1}{E}[\sigma_{1}-v(\sigma_{2}+\sigma_{3})]$, etc.
$$\hat{U}_{total}=\frac{1}{2E}[\sigma_{1}^{2}+\sigma_{2}^{2}+\sigma_{3}^{2}-2v(\sigma_{1}\sigma_{2}+\sigma_{1}\sigma_{3}+\sigma_{2}\sigma_{3})]$$
If we sub in the hydrostatic/mean stress:
$$\begin{align*}
\hat{U}_{hydrostatic} &=  \frac{3(1-v)}{2E}\sigma_{m}^{2}\\
&= \frac{1-2v}{6E}(\sigma_{1}+\sigma_{2}+\sigma_{3})^{2}
\end{align*}$$
And if we subtract the volumetric from the total energy:
$$\hat{U}_{deviatoric}=\frac{1}{12G}\left[(\sigma_{1}-\sigma_{2})^{2}+(\sigma_{2}-\sigma_{3})^{2}+(\sigma_{1}-\sigma_{3})^{2}\right] $$
To get the critical deviatoric strain energy, we use tensile test data:
$$\hat{U}_{critical}=\frac{\sigma_{Y}^{2}}{6G}$$
resulting in the Von Mises failure criterion:
$$(\sigma_{1}-\sigma_{2})^{2}+(\sigma_{2}-\sigma_{3})^{2}+(\sigma_{1}-\sigma_{3})^{2}=2\sigma_{Y}^{2}$$
Which for plane stress $\sigma_{3}=0$ reduces to:
$$\sigma_{1}^{2}-\sigma_{1}\sigma_{2}+\sigma_{2}^{2}=\sigma_{Y}^{2}$$
![[Pasted image 20241008225750.png|centre|400]]
The yield locus is an ellipse, which is at $\pi/4$ to the principal axes.
\
Note how the Von Mises and Tresca agree closely; with their maximum difference being about 15%.
![[Pasted image 20241008225918.png|centre|400]]
