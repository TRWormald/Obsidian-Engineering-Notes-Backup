Consider the work done by a force in moving a load from $x=a$ to $x=b$:
$$Work=Force\times Distance$$
But force is a vector so:
$$W=\mathbf{F\cdot d}=\mathbf{F}\cdot ((b-a)\mathbf{i})$$
Now, what if $\mathbf{F}$ were not constant, $\mathbf{F}=\mathbf{F}(x)$? Then:
$$\begin{align*}
W&= \lim_{N\rightarrow\infty}\sum\limits_{j=1}^{N}(\textbf{F}(x_{j})\cdot\mathbf{i})(\Delta x)\\
&= \int_{a}^{b}(\mathbf{F\cdot i})~dx\\
W&= \int_{t=0}^{t=(b-a)}\textbf{F}\cdot d\mathbf{r}
\end{align*}$$
We can parameterise the path by:
$$\mathbf{r}(t)=(a,0,0)+(t,0,0)$$
Where $\textbf{r}(t)$ is the position of the load, so that in this case $d\mathbf{r}=dt~\mathbf{i}$. More generally, if $\mathbf{F}=\mathbf{F}(\mathbf{r})$ is a vector field which varies with spatial position $\mathbf{r}=(x,y,z)$ and distance moved is in direction $\mathbf{c}$, then motion occurs along the line:
$$\mathbf{r}(t)=\mathbf{a}+\mathbf{c}t,~~~~~~~~ \text{for which }~~d\mathbf{r}(t)=\mathbf{c}~dt$$
So that:
$$W=\int_{t=0}^{t=(b-a)}\textbf{F}(\mathbf{r}(t))\cdot \mathbf{c}~dt$$
#### Example 4.1
![[Pasted image 20241011152044.png]]

![[WhatsApp Image 2024-10-12 at 12.13.37_4f9b665b.jpg|centre]]
![[WhatsApp Image 2024-10-12 at 12.14.24_405e70ed.jpg|centre]]


#### The Work Integral
The **work integral** is an example of a path integral of a vector field:
$$\int_{C}\mathbf{v}(\mathbf{r})\cdot d\mathbf{r}$$
We can interpret this in 2D as summing the components of the vectors in the direction of the tangent to the curve $C$ at each point along $C$ whose position vector is $\mathbf{r}$.
![[Pasted image 20241012122818.png|centre]]
In order to evaluate such path integrals we need to have a parametrisation of the curve $C(t)$ just like we did in [[Path Integrals of Scalar and Vector Fields#Example 4.1|Example 4.1]]. So:
$$\mathbf{r}(t)=x(t)\mathbf{i}+y(t)\mathbf{j}+z(t)\mathbf{k}=(x(t),y(t),z(t))$$
Then:
$$d\mathbf{r}=\frac{d\mathbf{r}(t)}{dt}dt=\left(\frac{dx(t)}{dt}\mathbf{i}+\frac{dy(t)}{dt}\mathbf{j}+\frac{dz(t)}{dt}\mathbf{k}\right)dt$$
#### Path (line) integral of a scalar field $f(\mathbf{r})$ 
$$\int_{C}f(\mathbf{r})~ds=\int_{C}f(\mathbf{r})|d\mathbf{r}|$$
Where $ds$ is the infinitesimal arclength along $C$.
We can interpret this in 2D as taking a path $C$ across the contours $f=const.$ summing up the height.
![[Pasted image 20241012123424.png|centre]]
Clearly in general, if two different curves $C_1$ and $C_2$ connect the same end points a and b then the integrals along $C_1$ and $C_2$ will be different.
