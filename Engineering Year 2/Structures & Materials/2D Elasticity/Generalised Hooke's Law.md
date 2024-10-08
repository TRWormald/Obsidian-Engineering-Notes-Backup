In solving elasticity problems, there are three governing equations:
1) Equilibrium equations: stress transformation
2) Compatibility equations: strain transformation
3) Constitutive equations: **material model**
\
*The material model relates stress and strain.*
\
The majority of engineering materials are:
- Homogeneous - properties the same in all locations
- Isotropic - properties the same in all directions
- Linear - linear relationship between stress and strain
- Elastic - no energy is lost in deformation
\
We can represent the stress and strain in the material as **tensors**, the following are the Cauchy stress and strain tensors:
$$\bar\sigma=\begin{bmatrix}\sigma_{xx}&\tau_{xy}&\tau_{xz}\\\tau_{xy}&\sigma_{yy}&\tau_{yz}\\\tau_{xz}&\tau_{yz}& \sigma_{zz}\end{bmatrix}~~~~~~~~\bar\varepsilon=\begin{bmatrix}\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{xy}&\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{xz}&\varepsilon_{yz}& \varepsilon_{zz}\end{bmatrix}$$
Where $\varepsilon$ is the mathematical or tensorial shear strain, rather than the engineering shear strain $\gamma$, noting that $\varepsilon_{xy}=\frac{\gamma_{xy}}{2}$.
\
### Hooke's Law
Robert Hooke discovered that there is a linear relationship between the applied stresses and the shear strains.
Therefore linear material behaviour can be described using the matrix:
$$\begin{bmatrix}\varepsilon_{xx}\\\varepsilon_{yy}\\\varepsilon_{zz}\\\gamma_{yz}\\\gamma_{xz}\\\gamma_{xy}\end{bmatrix}=\begin{bmatrix}S_{11}&S_{12}&S_{13}&S_{14}&S_{15}&S_{16}\\S_{21}&S_{22}&S_{23}&S_{24}&S_{25}&S_{26}\\S_{31}&S_{32}&S_{33}&S_{34}&S_{35}&S_{36}\\S_{41}&S_{42}&S_{43}&S_{44}&S_{45}&S_{46}\\S_{51}&S_{52}&S_{53}&S_{54}&S_{55}&S_{56}\\S_{61}&S_{62}&S_{63}&S_{64}&S_{65}&S_{66}\end{bmatrix}        \begin{bmatrix}\sigma_{xx}\\\sigma_{yy}\\\sigma_{zz}\\\tau_{yz}\\\tau_{xz}\\\tau_{xy}\end{bmatrix}$$
Where $S_{ij}$ represent 36 material constants, noting that $S_{ij}=S_{ji}$, due to Maxwell-Betti's reciprocal theorem.
