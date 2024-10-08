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
### Hooke's Law
Robert Hooke discovered that there is a linear relationship between the applied stresses and the shear strains.
Therefore linear material behaviour can be described using the matrix:
$$\begin{bmatrix}\varepsilon_{xx}\\\varepsilon_{yy}\\\varepsilon_{zz}\\\gamma_{yz}\\\gamma_{xz}\\\gamma_{xy}\end{bmatrix}=\begin{bmatrix}S_{11}&S_{12}&S_{13}&S_{14}&S_{15}&S_{16}\\S_{21}&S_{22}&S_{23}&S_{24}&S_{25}&S_{26}\\S_{31}&S_{32}&S_{33}&S_{34}&S_{35}&S_{36}\\S_{41}&S_{42}&S_{43}&S_{44}&S_{45}&S_{46}\\S_{51}&S_{52}&S_{53}&S_{54}&S_{55}&S_{56}\\S_{61}&S_{62}&S_{63}&S_{64}&S_{65}&S_{66}\end{bmatrix}        \begin{bmatrix}\sigma_{xx}\\\sigma_{yy}\\\sigma_{zz}\\\tau_{yz}\\\tau_{xz}\\\tau_{xy}\end{bmatrix}$$
Where $S_{ij}$ represent 36 material constants, noting that $S_{ij}=S_{ji}$, due to Maxwell-Betti's reciprocal theorem.
#### Considering Bi-Axial Stress States
If we consider a bi-axial stress state, the final deformation can be considered to be the sum or superposition of the deformations caused by the individual stresses:![[Pasted image 20241008214306.png]]
If we use Poisson's ratio and the [[Young's Modulus]] of the material we can generate the matrix linking the stress and the strains:
$$\begin{bmatrix}\varepsilon_{xx}\\\varepsilon_{yy}\\\gamma_{xy}\end{bmatrix}=\begin{bmatrix}1/E&-v/E&0\\-v/E&1/E&0\\0&0&1/G\end{bmatrix}\begin{bmatrix}\sigma_{xx}\\\sigma_{yy}\\\tau_{xy}\end{bmatrix}$$
In isotropic materials direct and shear strains are decoupled, i.e. they don't affect each other, and consequentially the principal directions for stress and strain coincide.
However for anisotropic materials, like composites, the compliance matrix is fully populated with coupling described by $\bar{S}_{16}$ and $\bar{S}_{26}$ terms where the zeros are in the isotropic compliance matrix.
### The Shear Modulus
For isotropic materials [[Shear Modulus]] G is not independent:
$$\gamma_{xy}=\frac{\tau_{xy}}{G}$$
Which is the shear strain due to pure shear.
If we transform this to $X'Y'$ (+45 degrees):
$$\varepsilon_{x'x'}=\sin\theta\cos\theta\gamma_{xy}=\frac{\tau_{xy}}{2G}$$
When we consider the bi-axial loading case again the direct strain equals:
$$\varepsilon_{x'x'}=\frac{1}{E}(\sigma_{x'x'}-v\sigma_{y'y'})=\frac{\tau_{xy}}{E}(1+v)$$
And equating both gives:
$$G=\frac{E}{2(1+v)}$$
Meaning that we can describe the **isotropic, linear-elastic material under plane stress** using the compliance matrix:
$$\boxed{\begin{bmatrix}\varepsilon_{xx}\\\varepsilon_{yy}\\\gamma_{xy}\end{bmatrix}=\frac{1}{E}\begin{bmatrix}1&-v&0\\-v&1&0\\0&0&(1-v)/2\end{bmatrix}\begin{bmatrix}\sigma_{xx}\\\sigma_{yy}\\\tau_{xy}\end{bmatrix}}$$
Or using the stiffness matrix:
$$\boxed{\begin{bmatrix}\sigma_{xx}\\\sigma_{yy}\\\tau_{xy}\end{bmatrix}=\frac{E}{1-v^{2}}\begin{bmatrix}1&v&0\\v&1&0\\0&0&(1-v)/2\end{bmatrix}\begin{bmatrix}\varepsilon_{xx}\\\varepsilon_{yy}\\\gamma_{xy}\end{bmatrix}}$$
With only **two** material parameters: $E$ and $v$.
