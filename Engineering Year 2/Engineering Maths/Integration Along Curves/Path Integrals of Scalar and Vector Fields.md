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

