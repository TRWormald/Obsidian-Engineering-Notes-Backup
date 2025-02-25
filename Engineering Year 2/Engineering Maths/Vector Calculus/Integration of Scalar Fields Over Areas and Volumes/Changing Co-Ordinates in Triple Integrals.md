A general co-ordinate change $(x,y,z)~\rightarrow~(u,v,w)$ can be written in the form:
$$x=x(u,v,w),~y=y(u,v,w),~z=z(u,v,w)$$
\
The infinitesimal piece of volume $dV$ is the volume of the parallelepiped spanned by the vectors:
$$\frac{\partial \mathbf{r}}{\partial u}du,~\frac{\partial \mathbf{r}}{\partial v}dv,~\frac{\partial \mathbf{r}}{\partial w}dw$$
This volume is given by the triple scalar product:
$$\begin{align*}
dV&= \left(\frac{\partial \mathbf{r}}{\partial u}du\right)\cdot\left[\left(\frac{\partial \mathbf{r}}{\partial v}dv\right)\times\left(\frac{\partial \mathbf{r}}{\partial w}dw\right)\right]\\
&= \frac{\partial \mathbf{r}}{\partial u}\cdot\left(\frac{\partial \mathbf{r}}{\partial v}\right)\times \left(\frac{\partial \mathbf{r}}{\partial w}\right)
du~dv~dw\end{align*}$$
But the triple scalar product is equal to the determinant of all three vectors:
![[Pasted image 20241025143323.png|centre|400]]
Where $J$ is the Jacobian matrix of the transformation, sometimes written as:
![[Pasted image 20241025143353.png|centre|300]]
