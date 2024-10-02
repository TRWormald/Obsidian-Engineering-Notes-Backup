We know from [[Ellipses and Energy#Orbital Energy|earlier]] that:
$$E=-\frac{GMm}{2r}$$
Where $E=K~(Kinetic)+U~(Potential)$ and $G$ is the gravitational constant, $M$ and $m$ are the masses of the two objects, and $r$ is the orbital radius.
We can also calculate **escape velocity** i.e. the minimum velocity required to escape the gravity of a body, when launched from the ground:
$$\begin{align*}
\frac{1}{2}mv^{2}&= \frac{GMm}{r}\\
v_{esc}&=\sqrt{\frac{2GM}{r}} 
\end{align*}$$
### The Two Body Problem
This is the equation of motion for two bodies interacting gravitationally with each other. This is important as we consider things like this all the time - the earth and a satellite, the earth and the moon, the sun and the earth etc.
We need to be able to do this so that we can:
- To point the antenna of a ground station  
- To initiate an engine burn 
- To perform measurements 
- To time tag measurements 
- To rendezvous
#### Derivation
Consider the gravitational force between two bodies:
![[Pasted image 20241002174430.png|centre|300]]
We need to define a coordinate system such that:
$$\vec{r}=\vec{r}_{1}-\vec{r}_{2}=\vec{r}_{21}$$
Where $\vec{r}$ is the relative position vector pointing from $m_{2}$ to $M_{1}$.
Also where $\hat{r}_{21}$ is the unit vector pointing from $m_{2}$ to $M_{1}$
And $r=|\vec{r}|$ is the magnitude of $\vec{r}$.
![[Pasted image 20241002174737.png|centre|400]]
Note how we also have $\vec{r}_{0}$ which is the vector from the origin to the Centre of Mass.
\
We can define the forces between the two objects as:
$$\vec{F}_{12}=M_{1}\vec{\ddot{r}_{1}}=-\frac{GM_{1}m_{2}}{r^{2}}\hat{r}_{12}$$
$$\vec{F}_{21}=m_{2}\vec{\ddot{r}_{2}}=-\frac{GM_{1}m_{2}}{r^{2}}\hat{r}_{21}=\frac{GM_{1}m_{2}}{r^{2}}\hat{r}_{12}$$
Due to the fact that $\hat{r}_{21}=-\hat{r}_{12}\Rightarrow$ $\vec{F}_{12}=-\vec{F}_{21}$.
\
We can now say that:
$$\vec{\ddot{r}}=\vec{\ddot{r}}_{1}-\vec{\ddot{r}}_{2}=\left(-\frac{G\bcancel{M_{1}}m_{2}}{\bcancel{M_{1}}r^{2}}\hat{r}_{12}\right)-\left(\frac{G\bcancel{m_{2}}M_{1}}{\bcancel{m_{2}}r^{2}}\hat{r}_{12}\right)$$
So:
$$\vec{\ddot{r}}=-\frac{Gm_{2}}{r^{2}}\hat{r}_{12}-\frac{GM_{1}}{r^{2}}\hat{r}_{12}=-\frac{G(M_{1}+m_{2})}{r^{2}}\hat{r}_{12}$$
