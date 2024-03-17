The kinematics of a rigid body can be described by a combination of **translation** and **rotation**.
\
Note that a rigid body does not deform under applied forces, which means that relative distances within the body remain constant.

#### Rotation Around a Fixed Axis
##### 2D Bodies
Lets consider a rigid body with a fixed axis of rotation:
![[Pasted image 20240229114826.png|center]]
The above diagram (left) shows the [[Angular Velocity]] as well as the velocity at any given point with radius r from the point of rotation, whilst the diagram (right) shows in addition the [[Angular Acceleration]] the accelerations at that point.
In summary:
$$v_t=\omega~r$$
$$v_n=0$$
$$a_t=\alpha~r$$
$$a_n=\omega^2~r=\frac{v^2}{r}$$
These are very similar to the kinematic equations in polar coordinates:
![[Pasted image 20240229115211.png|center]]
##### 3D Bodies (Vector Form)
For a planar body rotating around a normal vector through point $O$:
![[Pasted image 20240229120049.png|center|400]]
The velocity is given by:
$$\textbf{v}=\boldsymbol{\omega}\times\textbf{r}$$And acceleration is:
$$\textbf{a}=\dot{\textbf{v}}$$
$$=\boldsymbol{\omega}\times\dot{\textbf{r}}+\dot{\boldsymbol{\omega}}\times\textbf{r}$$
$$=\boldsymbol{\omega}\times(\boldsymbol{\omega}\times\textbf{r})+\boldsymbol{\alpha}\times\textbf{r}$$
Noting the fact that the acceleration can be broken down into the normal and tangential components.
Where:
$$\boldsymbol{\omega}=\begin{pmatrix} 0\\0\\\omega\end{pmatrix}=\omega\textbf{k}$$
For planar (2D) problems and rotation about the z-axis.
And the position in the xy-plane is given by:
$$\textbf{r}=\begin{pmatrix}r_x\\r_y\\0\end{pmatrix}=r_x\textbf{i}+r_y\textbf{j}$$
