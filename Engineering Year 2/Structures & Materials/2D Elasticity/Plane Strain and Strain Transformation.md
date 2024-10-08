When we have *plane strain* deformations are strictly limited to the *XY* plane.
**Don't** confuse plane strain and plane stress:
$$\text{plane strain : }\varepsilon_{zz}=\gamma_{xz}=\gamma_{yz}=0,\text{but }\sigma_{zz}\ne 0$$
$$\text{plane stress : }\sigma_{zz}=\tau_{xz}=\tau_{yz}=0,\text{but }\varepsilon_{zz}\ne 0$$
In plane stress, although $\sigma_{zz}=0$, thickness $t$ may vary due to $v$ (Poisson's Ratio):
![[Pasted image 20241008110640.png|centre|400]]
*The only times that plane stress and plane strain are the same is when*:
- There are no loads
- $\sigma_{xx}=-\sigma_{yy}$
- The plane is in true shear
- etc.
\
### Strain Transformations
Like with the stress transformation, we can transform strains using the exact same rotation matrix:
$$\begin{bmatrix}\varepsilon_{x'x'}\\\varepsilon_{y'y'}\\\gamma_{x'y'}/2\end{bmatrix}=\begin{bmatrix}\cos^{2}\theta&\sin^{2}\theta&2\sin\theta\cos\theta\\\sin^{2}\theta&\cos^{2}\theta&-2\sin\theta\cos\theta\\-\sin\theta\cos\theta&\sin\theta\cos\theta&\cos^{2}\theta-\sin^{2}\theta\end{bmatrix}\begin{bmatrix}\varepsilon_{xx}\\\varepsilon_{yy}\\\gamma_{xy}/2\end{bmatrix}$$
Where we have used the tensorial shear strain $\varepsilon_{xy}=\gamma_{xy}/2$ rather than the engineering strain $\gamma_{xy}$.
\
We can also use Mohr's circle for transforming the strain:
![[Pasted image 20241008111337.png|centre|400]]
Note that a CCW rotation of the coordinate system is represented by a CW rotation on Mohr's circle.