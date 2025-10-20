>Equations of Motion form a mathematical model, for a rigid-body aircraft. The model provides a complete description of the response to controls or disturbances, subject only to modelling limitations.
 Outputs can be measured in terms of displacement, velocity, and acceleration.
 We can also augment the model to include equations which describe engine gyroscopic effects and control system dynamics.

#### What do we need to know?
- We are **not** required to memorise a full derivation of the equations
- We **do** need to understand their structure and the terms involved
- The general nonlinear equations are given first, and simplified versions are presented later.
- We **do** need to learn the notation (for axes) from previous lectures
### Derivation of the Equations of Motion
We start from Newton's Second law - when applied to a rigid body:
![[Pasted image 20250926102006.png|centre|400]]
(Where all motions are relative to an **inertial** frame)

These are commonly interpreted as:
$$\text{Force = mass }\times\text{ inertial acceleration} ~~~~\boxed{ma_{i}=\sum F_{i}}$$
$$\text{Moment = Moment of Inertia }\times\text{ Angular Acc.} ~~~~\boxed{I_{j}\alpha_{j}=\sum M_{j}}$$
#### Components of Inertial Acceleration
We start by working towards defining the **inertial accelerations** arising from the components of external force acting on the aircraft.
Consider an orthogonal set of body aces with origin fixed at the CG of the rigid body shown in the figure:
![[Pasted image 20250926102343.png|centre]]
$\bar p$ is an arbitrary point within the body axes at position $(x,y,z)$
Local components of *linear* velocity and acceleration at $\bar p$ relative to the body axes are $(u,v,w)$ and $(a_x,a_y,a_z)$.
Components of the *angular* velocity of $\bar p$ relative to the body axes are $(p,q,r)$.
The body axes themselves are in motion relative to an external inertial or earth frame, with linear velocities $(U,V,W)$.

The velocity components at $\bar p$ relative to the origin $O$ are:
$$u=\dot x - ry+qz$$
$$v=\dot y - pz+rx$$
$$w=\dot z - qx+py$$
Where the two final terms are due to circular motion and tangential velocity:
![[Pasted image 20250926102841.png|centre]]
![[Pasted image 20250926102858.png|centre|250]]
Since the body (the aircraft) is assumed to be rigid, $\dot x=\dot y=\dot z=0$ (since the point $\bar p$ should not be moving in relation to the CG)
Therefore the velocity equations reduce to:
$$u=- ry+qz$$
$$v=- pz+rx$$
$$w=- qx+py$$

We now need to re-write these in terms of the inertial frame. Without loss of generality, we can consider the inertial frame to be instantaneously coincident with the body axes. 
We can then obtain the absolute velocity components $(u',v',w')$ of the point $\bar p$ by adding the velocity components $(U,V,W)$ of the origin/CG to the local velocity components $(u,v,w)$.
This gives us:
$$u'=\dot{x}'=U+u=U-ry+qz$$
$$v'=\dot{y}'=V+v=V-pz+rx$$
$$w'=\dot{z}'=W+w=W-qx+py$$
The corresponding accelerations in the inertial frame are therefore:
![[Pasted image 20250926103556.png|centre|400]]
Given that the inertial frame is considered to be instantaneously coincident with the body axes:
$$x'=x,~y'=y,~z'=z,~\dot{x}=\dot{x}',~\dot{y}=\dot{y}',~\text{and }\dot{z}=\dot{z}'$$
Which when substituted gives:
![[Pasted image 20250926103801.png|centre|400]]

#### Generalised Force Equations
Now we can apply Newton's Second Law, we consider an incremental mass $\delta m$ at each point $\bar{p}$ in the rigid body.
Thus the incremental components of force acting on the mass will be given by:
$$(\delta m\cdot a_{x}',\delta m\cdot a_{y}',\delta m\cdot a_{z}')$$
For the body as a whole, we substitute the expressions for components of inertial acceleration and then sum these increments. Giving:
![[Pasted image 20250926104025.png|centre|400]]
Substituting the expressions for inertial accelerations into the force equations:
![[Pasted image 20250926104110.png|centre|400]]
Giving:
$$\huge{\boxed{\begin{align*}
m(\dot{U}-rV+qW)&= X\\
 m(\dot{V}-pW+rU)&= Y\\
m(\dot{W}-qU+pV)&= Z
\end{align*}}}$$
#### Generalised Moment Equations
We can then consider the incremental moments produced by forces acting on the incremental mass at point $\bar{p}$. Summing these over the body yields the moment equations. 
For full derivation refer to [[Flight Dynamics Lecture 3 - Equations of Motion 1.pdf#page=25|the lecture slides]].
We can fully simplify the moment equations to:
$$\huge{\boxed{\begin{align*}
I_{xx}\dot{p}-(I_{yy}-I_{zz})qr-I_{xz}(pq+\dot{r})&= L\\
I_{yy}\dot{q}-(I_{xx}-I_{zz})pr-I_{xz}(p^{2}-r^{2})&= M\\
I_{zz}\dot{r}-(I_{xx}-I_{yy})pq-I_{xz}(qr-\dot{p})&= N
\end{align*}}}$$
#### Kinematic Equations for Rotation
We can find the relationship between body axes rates $(p,q,r)$ and attitude (Euler angle) rates $(\dot\phi,\dot\theta,\dot\psi)$ by carrying out the necessary trigonometric transformations according to the sequence below:
![[Pasted image 20250926110406.png|centre|400]]
This yields:
$$\huge{\boxed{\begin{align*}
\dot\phi&= p+\tan\theta(q\sin\phi+r\cos\phi)\\
\dot\theta&= q\cos\phi -r\sin\phi\\
\dot\psi&= \frac{q\sin\phi+r\cos\phi}{\cos\theta}
\end{align*}}}$$
We can also use the Euler angles to transform between body axes velocities
and inertial axes velocities, these form the so-called navigation equations:
![[Pasted image 20250926110717.png|centre|400]]
### The 12 Equations of Motion for General Atmospheric 6-DoF flight
The following equations are the 12 equations of motion needed to describe 6 Degree of Freedom flight for general atmospheric conditions.
$$\huge{\boxed{\begin{align*}
m(\dot{U}-rV+qW)&= X\\
 m(\dot{V}-pW+rU)&= Y\\
m(\dot{W}-qU+pV)&= Z
\end{align*}}}$$
$$\huge{\boxed{\begin{align*}
I_{xx}\dot{p}-(I_{yy}-I_{zz})qr-I_{xz}(pq+\dot{r})&= L\\
I_{yy}\dot{q}-(I_{xx}-I_{zz})pr-I_{xz}(p^{2}-r^{2})&= M\\
I_{zz}\dot{r}-(I_{xx}-I_{yy})pq-I_{xz}(qr-\dot{p})&= N
\end{align*}}}$$
$$\huge{\boxed{\begin{align*}
\dot\phi&= p+\tan\theta(q\sin\phi+r\cos\phi)\\
\dot\theta&= q\cos\phi -r\sin\phi\\
\dot\psi&= \frac{q\sin\phi+r\cos\phi}{\cos\theta}
\end{align*}}}$$
![[Pasted image 20250926110717.png|centre|400]]
