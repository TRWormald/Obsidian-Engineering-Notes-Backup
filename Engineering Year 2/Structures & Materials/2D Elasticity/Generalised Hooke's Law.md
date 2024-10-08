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
$$\bar\sigma=\begin{bmatrix}\sigma_{xx}&\tau_{xy}&\tau_{xz}\\\tau_{xy}&\sigma_{yy}&\tau_{yz}\\\tau_{xz}&\tau_{yz}& \sigma_{zz}\end{bmatrix}~~~~~~~~\bar\varepsilon=\begin{bmatrix}\varepsilon_{xx}&\tau_{xy}&\tau_{xz}\\\tau_{xy}&\varepsilon_{yy}&\tau_{yz}\\\tau_{xz}&\tau_{yz}& \sigma_{zz}\end{bmatrix}$$