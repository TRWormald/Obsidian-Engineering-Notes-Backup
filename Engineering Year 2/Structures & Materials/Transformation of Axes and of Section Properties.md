We need to be able to transform section properties by rotating them about structural axes.
\
**2D orthogonal coordinates ($x,y$) can be rotated (transformed) by any angle $\beta$ through:**
$$\begin{bmatrix}x'\\y'\end{bmatrix}=\begin{bmatrix}m&n\\-n&m\end{bmatrix}\begin{bmatrix}x\\y\end{bmatrix}$$
Where:
$$m=\cos\beta$$
$$n=\sin\beta $$
Therefore the transformed coordinates are:
$$x'=mx+ny$$
$$y'=-nx+my$$
![[Pasted image 20240916195820.png|centre|300]]
*So what happens to 2nd moments of area upon axis transformation?*
### Transformation of SMAs
We now have transformed second moments of area:
$$I_{x'x'}=\int y'^{2}dA$$
$$I_{x'x'}=\int(-nx+my)^{2}dA$$
$$I_{x'x'}=m^{2}\int y^{2}~dA+n^{2}\int x^{2}~dA -2mn\int xy~dA$$
Hence:
$$I_{x'x'}=m^{2}(I_{xx})+n^{2}(I_{yy})-2mn(I_{xy})$$
And similarly:
$$I_{y'y'}=m^{2}(I_{yy})+n^{2}(I_{xx})-2mn(I_{xy})$$
$$I_{x'y'}=mn(I_{xx}-I_{yy})+(m^{2}-n^{2})(I_{xy})$$
**These can be written in matrix form as:**
$$\begin{bmatrix}I_{x'x'}\\I_{y'y'}\\I_{x'y'}\end{bmatrix}=\begin{bmatrix}m^{2}&n^{2}&-2mn\\n^{2}&m^{2}&2mn\\mn&-mn&m^{2}-n^{2}\end{bmatrix}\begin{bmatrix}I_{xx}\\I_{yy}\\I_{xy}\end{bmatrix}$$
Where:
$$m=\cos\theta$$
$$n=\sin\theta$$
**Or can be expanded as:**
![[Pasted image 20240916201920.png|centre]]
## The Principal Axes
Rotation angle $\theta$ gives the principal axes when:
- The product second moment of area is zero, or
- The second moments of area are maximal or minimal, so their derivative w.r.t $\theta$ is zero:
$$\frac{\partial}{\partial\theta}(I_{x'x'})=0$$ $$\frac{\partial}{\partial\theta}\left[\left(\frac{I_{xx}+I_{yy}}{2}\right)+\left(\frac{I_{xx}-I_{yy}}{2}\right)\cos2\theta-(I_{xy})\sin2\theta\right]=0$$
$$\begin{align*}
\tan2\theta_{P}&= \frac{2I_{xy}}{I_{yy}-I_{xx}}\\
\theta_{P}&=\frac{1}{2}\arctan\left(\frac{2I_{xy}}{I_{yy}-I_{xx}}\right) 
\end{align*}$$
Hence the angle $\theta_{P}$ rotates ($x,y$) into (1,2), while the angle $\beta_p$ rotates (1,2) into  

