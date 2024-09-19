### Recap of Y1 Content
In Y1 we only considered shear forces, but shear strains in beams were neglected.
Shear strains are negligible if the aspect ratio (span/thickness) is large. In reality however cross-sections warp due to shear stresses. i.e. sections deform out of plane in a non linear fashion:
![[Pasted image 20240918203724.png]]
This can be seen in the I-beam above, where the flanges have deformed differently to the web.
**Planar sections don't necessarily remain planar.**
#### Shear Stress Definition
The shear stress $\tau$ is a measure of 'tangential force per unit area'. It arises when we apply a 'sliding force' to the surface:
![[Pasted image 20240918203901.png|centre]]
It is a field property (like direct stress $\sigma$), which means that it can vary continuously within a body and can be considered at a point.
$$\tau=\lim_{\delta A\rightarrow0}\frac{\delta S}{\delta A}$$
We use the same units as with direct stress:
$$1~\text{Pa}=1\frac{\text{N}}{\text{m}^2}=10^{-6}\text{MPa}=10^{-6}\frac{\text{N}}{\text{mm}^2}$$
#### Shear Strain Definition
Shear strain $\gamma$ is the angular rotation in radians (non-dimensional).
There are two primary cases, pure shear and simple shear:
![[Pasted image 20240918204613.png|centre]]
Element 'edges' (or 'shear planes') don't change length - but simply translate or rotate.
However element 'diagonals' do change length:
![[Pasted image 20240918204705.png|centre|300]]
#### Shear Modulus
For linear elastic behaviour shear stress is proportional to shear strain:
$$\tau=G\gamma$$
![[Pasted image 20240918204901.png|centre|300]]
Where the constant of proportionality $G$ is the shear modulus.
This is a material property, just like [[Young's Modulus]] or Poisson's Ratio.
In fact, for isotropic materials these three properties obey a very simple relationship:
$$G=\frac{E}{2(1+v)}$$
#### Complementary Shear Stresses
For equilibrium complementary shear stresses must exist to balance translational and rotational tendencies:
![[Pasted image 20240918205114.png|centre]]
![[Pasted image 20240918205158.png]]
**This means that all four complementary shear stresses are equal in magnitude!!!**
#### Shear Forces in Beams
The most important thing to remember about shear forces in beams is that:
*'The shear force distribution is the derivative of the bending moment distribution'*
![[Pasted image 20240918205929.png|centre|300]]
### Shear Stresses Nomenclature
When talking about shear stresses we will from now on include two subscripts:
- The first indicates the normal to the plane being considered
- The second indicates the direction of the tangential force.
![[Pasted image 20240918205349.png|centre]]
In the example above the uppermost shear stress takes the form:
$$\tau_{yz}$$
This indicates the fact that the stress is normal to the $y$ plane and in the direction of $z$.
If the stress was instead:
$$\tau_{yx}$$
The arrow would be pointing out of the page.
### Shear Stresses in Bending
Take the below image as an example of a slender structure of solid cross section subjected to downward shear force $S$ along a principal axis (i.e. intersecting with a line of symmetry/maximum or minimum SMA).
![[Pasted image 20240918210259.png|centre]]
We want to find the shear stress at a certain point in the beam:
![[Pasted image 20240918211535.png|centre|200]]
We want to find the shear stress at a height $y_{1}$ above the neutral axis.
![[Pasted image 20240918212816.png|centre|300]]
This is a side view of the beam, it is much clearer to see what forces are balancing each other out in this instance.
The beam is in equilibrium so the horizontal forces acting on it must sum to zero, therefore:
$$(\tau+d\tau-\tau)(b\cdot dz)+(\sigma+d\sigma-\sigma)(b\cdot dy)=0$$
In other terms:
$$d\tau(b\cdot dz)=-d\sigma(b\cdot dy)$$
**The total shear force at layer $y_{1}$ is the 'accumulation' of horizontal forces $d\sigma (b\cdot dy)$ above $y_{1}$, hence:**
$$\tau_{1}(b_{1}\cdot dz)=\int_{y_{1}}^{h}(d\sigma\cdot b)~dy$$
*Note that at the free surface ($y=h$ we must have $\tau_{1}=0$*.
By rearranging and substituting we can get:
$$\boxed{\tau_{1}=\frac{S}{Ib_{1}}\int_{y_{1}}^{h}y\cdot dA}$$
**Note that the integral is the same as the first moment of area, hence:**
$$\boxed{\tau_{1}=\frac{S}{Ib_{1}}Q_{x_{1}x_{1}}}$$
#### Shear Stresses in a Rectangular Cross-Section
For a rectangular cross-section we can calculate the first moment of area to be equal to:
$$Q_{x_{1}x_{1}}=\frac{b}{2}(h^{2}-y_{1}^{2})$$
Substituting this into our equation for shear stress we get:
$$\tau_{1}=\frac{S}{2I_{xx}}(h^{2}-y_{1}^{2})$$
Resulting in the following shear stress distribution:
![[Pasted image 20240918214201.png|centre|300]]
Note how the shear stress is greatest at the neutral axis and zero at distance $h$ from it.
This is the opposite to direct stress - where it is maximum/minimum at the extremities and zero at the neutral axis.