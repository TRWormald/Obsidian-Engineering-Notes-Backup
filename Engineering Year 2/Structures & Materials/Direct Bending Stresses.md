### Beam Bending
In Year 1 we considered beam bending in only 2 dimensions meaning that we could use the equation:
$$\frac{M}{I}=\frac{\sigma}{y}=\frac{E}{R}$$
For a simple cantilever beam bending:
![[Screenshot 2024-09-16 222821.png|centre|200]]
However now we are in Year 2 we will be considering bending in more than one direction and hence the same equation (in exactly the same scenario) now becomes:
$$\frac{M_{x}}{I_{xx}}=\frac{\sigma_{z}}{y}=\frac{E}{R_{x}}$$
The linear stress distribution also becomes:
$$\sigma_{z(y)}=\frac{M_{x}}{I_{xx}}y$$
These relationships are much clearer when considered in 3D:
![[Pasted image 20240916223856.png|centre]]
### Combined Loading
Say we apply a combination of CCW moments about the $x, y$ axes, what would the result of this be?
It will be the superposition of the two orthogonal components:
![[Pasted image 20240917123317.png|centre]]
After derivation we get that the planar stress is equal to:
$$\sigma_{z}=-\frac{M_{y}I_{xx}+M_{x}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}x+\frac{M_{x}I_{yy}+M_{y}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}y$$
By setting the planar stress to zero we can find the neutral axis:
$$\sigma_{z}=0=-\frac{M_{y}I_{xx}+M_{x}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}x_{NA}+\frac{M_{x}I_{yy}+M_{y}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}y_{NA}$$
Therefore:
$$\tan\alpha=\frac{M_{y}I_{xx}+M_{x}I_{xy}}{M_{x}I_{yy}+M_{y}I_{xy}}$$
