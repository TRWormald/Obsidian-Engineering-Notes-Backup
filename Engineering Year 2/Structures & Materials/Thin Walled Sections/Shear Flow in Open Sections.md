We make several assumptions about thin walls:
1) Direct stresses are constant through the thickness:
$$\sigma_{z_{(n)}}=const.$$
![[Pasted image 20240922124219.png|centre|200]]
2) Through-thickness stresses are negligible:
$$\sigma_{n}=0,~~~~~~~~\tau_{zn}=0$$
![[Pasted image 20240922124317.png|centre|200]]
3) In plane shear stresses are constant through the thickness:
$$\tau_{zs_{(n)}}=const.$$
![[Pasted image 20240922124411.png|centre|200]]
Following these assumptions, we define a new vectoral quantity called **shear flow**, i.e. shear force per unit arclength $s$:
$$\boxed{q_{(s)}=t_{(s)}\cdot\tau_{zs}}$$
Its units are usually $\text{[N/mm]}$

### Calculating Shear flow in Open Thin-Walled Sections
We will consider a small element of the thin wall (within the $z - s$ plane)
![[Pasted image 20240922130726.png]]
Two stress components exist: $\sigma_{z}$ and $\tau_{sz}$.
Balancing the forces in the $z$ direction we get:
$$[(\tau+d\tau)-\tau]\cdot (t~dz)~+[(\sigma+d\sigma)-\sigma]\cdot(t~ds)=0$$
$$\tau\cdot(t~dz)+d\sigma\cdot(t~ds)=0$$
Therefore rearranging gives:
$$t\frac{d\sigma}{dz}+t\frac{d\tau}{ds}=0$$
We know that $\tau=\frac{q}{t}$, hence:
$$\boxed{-\frac{dq}{ds}=\frac{d\sigma}{dz}t}$$
Substituting in the $\sigma_{z}$ from [[Direct Bending Stresses#Combined Loading|combined loading]] and going through several stages of rearranging gives:
$$q_{(s)}=q_{0}-\underbrace{\left(\frac{S_{x}I_{xx}-S_{y}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}\right)}_{C_{x}}\int_{0}^{s}x_{(s)}t_{(s)}ds-\underbrace{\left(\frac{S_{y}I_{yy}+S_{x}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}\right)}_{C_{y}}\int_{0}^{s}y_{(s)}t_{(s)}ds$$Or more simply:
$$\boxed{q_{(s)}=q_{0}-C_{x}\int_{0}^{s}x_{(s)}t_{(s)}~ds-C_{y}\int_{0}^{s}y_{(s)}t_{(s)}~ds}$$
