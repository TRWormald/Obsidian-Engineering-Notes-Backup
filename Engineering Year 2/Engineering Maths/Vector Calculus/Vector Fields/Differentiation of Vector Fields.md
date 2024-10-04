There are two key types of differentials of a vector field:
1) Divergence (div)
2) Curl (curl)
**Divergence** represents the extent to which the nearby particles being carried by the vector field are being pulled apart.
![[Pasted image 20241001150235.png|centre|300]]
**Curl** represents the amount to which nearby particles being carried by the vector field are being rotated around each other.
![[Pasted image 20241001150250.png|centre|300]]
### Calculating $\text{div} ~\vec{v}$
We can calculate divergence using the equation:
$$\begin{align*}
\text{div }\vec{v}&= \vec{\nabla}\cdot\vec{v}=\left(\frac{\partial}{\partial x},\frac{\partial}{\partial y},\frac{\partial}{\partial z}\right)\cdot(v_{1},v_{2},v_{3})\\
&= \frac{\partial}{\partial x}v_{1}+\frac{\partial}{\partial y}v_{2}+\frac{\partial}{\partial z}v_{3}
\end{align*}$$
*Note how this is a scalar value!*
### Calculating $\text{curl }\vec{v}$
We can calculate curl using the equation:
$$\begin{align*}
\text{curl }\vec{v}&= \vec\nabla\times\vec{v}=\left|\begin{matrix}\vec{i}&\vec{j}&\vec{k}\\ \frac{\partial}{\partial x}&\frac{\partial}{\partial y}&\frac{\partial}{\partial z}\\v_{1}&v_{2}&v_{3}\end{matrix}\right| \\
&= \left(\frac{\partial v_{3}}{\partial y}-\frac{\partial v_{2}}{\partial z}\right)\vec{i}+\left(\frac{\partial v_{1}}{\partial z}-\frac{\partial v_{3}}{\partial x}\right)\vec{j}+\left(\frac{\partial v_{2}}{\partial x}-\frac{\partial v_{1}}{\partial y}\right)\vec{k}\end{align*}
$$
*Note how this is a vector value!*
