Aircraft structures follow the ‘semi-monocoque’ design philosophy:
- Axial members forming ‘truss’ or ‘frame’ constructions
- Stressed-skin members where structural loads are resisted by outer skin
\
As we move to more realistic thin-walled structures, it becomes necessary to simplify our analyses by assuming that:
1. Skins are good at resisting in-plane shear stresses $𝜏_{𝑧𝑠}$ but are poor at resisting direct stresses $𝜎_𝑧$ as they tend to buckle in compression 
2. Booms carry all direct stresses $𝜎_𝑧$ , e.g. spar caps, stringers, longerons etc. 
3. As a consequence, the shear flow is constant between booms
![[Pasted image 20241011120450.png|centre]]
**Booms** - are axial members that sustain/transmit *direct stresses*
- The 'effective boom area' includes the cross-sectional area of local axial members such as stringers, stiffeners, spar caps, or longerons
- However, it also includes the contribution of neighbouring skins, and their cross-sectional areas are assumed to be concentrated or lumped at points.
**Skins** - are thin webs that sustain/transmit *shear stresses*
- Skins are usually thin and buckle easily, not carrying direct stresses
- However, they are very good at resisting shear stresses, both under shear loading and/or torsion
- Usually they comprise the outer skin and spar webs.
### Structure Idealisation
Skins act as diagonal members in pin-jointed truss structures:
![[Pasted image 20241011121319.png|centre]]
### Effective Boom Areas
The 'lumping' or 'concentration' of skin areas is based on equilibrium of bending stresses and bending moments.
\
Balancing moments $M_{n}$ at boom 2 gives:
![[Pasted image 20241011132157.png|centre]]
Bending stresses are proportional to the distance from the neutral axis, so for bending about $x$ we use the centroid-based coordinates $y$:
![[Screenshot 2024-10-11 132410.png|centre]]
Hence we can calculate the effective boom area expressions:
For shear loading along $y$:
$$B_{k}=J_{k}+\sum\limits_{\text{all connected booms}}\left[\frac{b_{kl}t_{kl}}{6}\left(2+\frac{y_{l}}{y_{k}}\right)\right]$$
For shear loading long $x$:
$$B_{k}=J_{k}+\sum\limits_{\text{all connected booms}}\left[\frac{b_{kl}t_{kl}}{6}\left(2+\frac{x_{l}}{x_{k}}\right)\right]$$
Where:
- $J_{k}$ is the cross-sectional area of local joint or reinforcement
- $b_{kl}$ is the wall length between booms $k$ and $l$
- $t_{kl}$ is the wall thickness between booms $k$ and $l$
- $y_{l}/x_{l}$ is the centroid based coordinate of the connected boom $l$
- 