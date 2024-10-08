### Bulk Modulus
We use bulk modulus to relate spherical stress (Where $\sigma_{xx}=\sigma_{yy}=\sigma_{zz}=\sigma$) to volumetric strain:
$$\sigma=K\frac{\Delta V}{V_{0}}$$
Volumetric stress describes the change in material volume:
$$\frac{\Delta V}{V_{0}}=\frac{V-V_{0}}{V_{0}}$$
Since we can say that the deformed volume is equal to:
$$V=(1+\varepsilon_{xx})(1+\varepsilon_{yy})(1+\varepsilon_{zz})~dx~dy~dz$$
(For an infinitesimal element)
$$\begin{align*}
\frac{\Delta V}{V_{0}}&= \varepsilon_{xx}+\varepsilon_{yy}+\varepsilon_{zz}\\
&= \frac{(\sigma_{xx}+\sigma_{yy}+\sigma_{zz})(1-2v)}{E}
\end{align*}$$
Allowing us to show that:
$$\boxed{K=\frac{E}{3(1-2v)}}$$
### Applying Shear and Bulk Moduli
With shear modulus $G$ and bulk modulus $K$ being able to be represented as:
$$G=\frac{E}{2(1+v)}~~~~~~~~~K=\frac{E}{3(1-2v)}$$
There are bounds on what Poisson's ratio can be for isotropic materials:
$$v\in(-1,0.5)$$
Since the shear and bulk moduli must be positive and finite.
Note that most engineering materials have a Poisson's ratio of $v \in (0.2,0.5)$.
