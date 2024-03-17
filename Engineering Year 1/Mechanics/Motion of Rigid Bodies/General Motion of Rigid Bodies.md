As we know the kinematics of a rigid body can be described by a combination of **translation** and **rotation**.
We can formulate kinematics in either **absolute** or **relative** terms.
\
#### Absolute Motion
Solving a problem with **Absolute Motion**, with respect to a fixed coordinate system can be done in the following steps:
1) Express configuration of rigid bodies as geometric relations
2) Differentiate to find velocities and accelerations
##### Examples
###### Rolling Wheel
For a wheel with radius R, which is purely rolling (i.e. no slip)
![[Pasted image 20240229135653.png|center]]
![[Pasted image 20240229135705.png|center]]
\
We can then differentiate again to get the accelerations:
![[Pasted image 20240229135721.png|center]]


#### Relative Motion
Solving a problem with **Relative Motion**, where the motion of a point on a rigid body in general motion can also be expressed relative to another moving point.
For example, lets consider the motion of  two points:
![[Pasted image 20240229135842.png|center|300]]
Relative to point B, A describes an arc:
![[Pasted image 20240229135913.png|center|300]]
And has relative velocity:
$$\textbf{v}_{A/B}=\boldsymbol\omega\times \textbf{r}_{A/B}$$
With the total velocity at A being:
$$\textbf{v}_A=\textbf{v}_B+\textbf{v}_{A/B}$$
![[Pasted image 20240229140204.png|center]]
\
The same formula can be used for relative accelerations:
$$\textbf{a}_A=\textbf{a}_B+\textbf{a}_{A?B}$$
$$=\textbf{a}_B+\boldsymbol{\omega}\times(\boldsymbol{\omega}\times\textbf{r}_{A/B})+\boldsymbol{\alpha}\times\textbf{r}_{A/B}$$
##### A Special Case (Point of Zero Velocity)
This is a special case of relative velocity where:
$$\textbf{v}_A=\textbf{v}_P+\boldsymbol{\omega}\times\textbf{r}_{A/P}$$
$$=0+\boldsymbol{\omega}\times\textbf{r}_{A/P}$$
Consider the following diagram:
![[Pasted image 20240229153258.png|center|300]]
So the rigid body instantaneously rotates around the point P, and the velocity of points A and B are tangent to circular motion around P.
The point P (The instantaneous centre of rotation) is located at the intersection of the normals to the velocity vectors.
The angular velocity at P is given by:
$$\omega=\frac{v_A}{r_A}=\frac{v_i}{r_i}$$
So for any point $i$ on the body:
$$v_i=\omega~r_i$$
Note the following special cases for determining the centre of rotation:
![[Pasted image 20240229153630.png|center]]
##### Examples
###### Rolling Wheel
Given a purely rolling wheel of radius R:
![[Pasted image 20240229144000.png]]
$$\textbf{v}_A=\textbf{v}_O+\textbf{v}_{A/O}$$
$$=\textbf{v}_O+\boldsymbol{\omega}\times\textbf{r}_{A/O}$$
The velocity of the wheel axle:
$$\textbf{v}_O=\omega R\textbf{i}$$
Relative position of A and O:
$$\textbf{r}_{A/O}=-R~sin(\theta)\textbf{i}-R~cos(\theta)\textbf{j}$$
If $\boldsymbol{\omega}=-\omega\textbf{k}$ then:
$$\textbf{v}_{A/O}=\boldsymbol{\omega}\times\textbf{r}_{A/O}=(-\omega\textbf{k})\times(-R~sin(\theta)\textbf{i}-R~cos(\theta)\textbf{j})$$
$$=-R\omega~cos(\theta)\textbf{i}+R\omega~sin(\theta)\textbf{j}$$
So the total velocity $\textbf{v}_A$ is given as:
$$\textbf{v}_A=\omega R(1-cos(\theta))\textbf{i}+\omega R~sin(\theta)\textbf{j}$$
(Which is identical to the expression found using absolute motion)
Note how this means that for theta equals zero the velocity is zero:
![[Pasted image 20240229145022.png|center]]

