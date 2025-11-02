### Triangular Finite Element Formulation
![[Pasted image 20251024150631.png|centre]]
Triangular Finite Elements have 6 degrees of freedom (each node - of which there are three - is able to move in the x and y directions).
![[Pasted image 20251024150719.png|centre]]
The constant terms, $a_{1}$ and $a_{4}$ capture in-plane rigid body motion. The linear terms enable states of constant strain to be specified.
Recalling from earlier the constant strain element:
$$\begin{bmatrix}\epsilon_{xx} \\ \epsilon_{yy} \\ \epsilon_{xy}\end{bmatrix}=\begin{bmatrix}\frac{\partial}{\partial x} &0 \\ 0&\frac{\partial}{\partial y} \\ \frac{\partial}{\partial y}&\frac{\partial}{\partial x}\end{bmatrix}\begin{bmatrix}u_{x} \\ u_{y}\end{bmatrix}$$
![[Pasted image 20251024151512.png|centre]]
![[Pasted image 20251024151523.png|centre]]
![[Pasted image 20251024151632.png|centre]]
![[Pasted image 20251024151656.png|centre]]
![[Pasted image 20251024151940.png|centre]]
