We can rewrite the following equations in matrix form:
$$\sigma_{x'x'}=(\sigma_{xx}\cos\theta+\tau_{xy}\sin\theta)\cos\theta+(\sigma_{yy}\sin\theta+\tau_{xy}\cos\theta)\sin\theta$$
$$\tau_{x'y'}=-(\sigma_{xx}\cos\theta+\tau_{xy}\sin\theta)\sin\theta+(\sigma_{yy}\sin\theta+\tau_{xy}\cos\theta)\cos\theta$$To get:
$$\begin{bmatrix}\sigma_{x'x}\\\tau_{x'y'}\end{bmatrix}=\begin{bmatrix}(\sigma_{xx}+\sigma_{yy})/2\\0\end{bmatrix}+\underbrace{\begin{bmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{bmatrix}}_{\text{2D Rotation Matrix}}\begin{bmatrix}(\sigma_{xx}-\sigma_{yy})/2\\\tau_{xy}\end{bmatrix}$$
If we plot the transformed stresses for $\theta \in[0,\pi]$ on a set of axes with $\theta_{x'x'}$ on the abscissa and $\tau_{xy}$ on the ordinate, we get the Mohr's circle for stress:
![[Pasted image 20240929135734.png|centre]]
![[Pasted image 20240929135756.png|centre]]
