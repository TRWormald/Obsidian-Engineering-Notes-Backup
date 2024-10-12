The key to evaluating these types of integrals is to define a single (intrinsic) coordinate $t$ that parametrises the curve $C$. Then use:
$$d\mathbf{r}=\frac{d\mathbf{r}}{dt}dt$$
Consider first curves in 2D:
For some curves it is obvious how to do this, e.g. using the $x$-coordinate as the parameter:
- Straight line $y=bx+a$, or $x=t$, $y=a+bt$, so:
$$\mathbf{r}(t)=(t,a+bt)=(0,a)+(1,b)t$$
$$\Rightarrow d\mathbf{r}=(1,b)~dt$$
- Parabola $y=bx^{2}+a \Rightarrow$
$$\mathbf{r}(t)=(t,bt^{2}+a)$$
$$\Rightarrow d\mathbf{r}=(1,2bt)~dt$$
For other curves one can use an angular formulation:
- Circle $x^{2}+y^{2}=a^{2} \Rightarrow$
$$\mathbf{r}(t)=(a\cos t,a\sin t),~t\in[0,2\pi]$$
$$\Rightarrow d\mathbf r = (-a\sin t,a\cos t)~dt$$
- Ellipse $\frac{x^{2}}{a^{2}}+ \frac{y^{2}}{b^{2}}=1 \Rightarrow$
$$\mathbf{r}(t)=(a\cos t,b \sin t),~t\in [0,2\pi]$$
$$\Rightarrow d\mathbf r=(-a\sin t,b\cos t)~dt$$
**In 3D the concepts are similar; e.g.**
- Straight line:
$$\mathbf{r}=\mathbf a+\mathbf b t=(a_{1}+b_{1}t, a_{2}+b_{2}t,a_{3}+b_{3}t)$$
$$\Rightarrow d\mathbf r =(b_{1},b_{2},b_{3})=\mathbf b ~dt$$
- Helix:
$x, ~y$ describe a circle, so that the helix lies on the surface of a cylinder, with linearly varying value of $z$. Here $a$ is the radius of the helix and $\frac{b}{a}=\tan\theta$ where $\theta$ is the helix angle.
$$\mathbf r =(x,y,z)=(a\cos t,a\sin t,bt)$$
$$\Rightarrow d\mathbf r=(-a\sin t,a\cos t, t)~dt$$
### Calculating total length/arclength
The length, or total arclength $S$ of a curve $C$ parameterised by $\mathbf r =(x(t),y(t),z(t))$ from $t=a$ to $t=b$ is the sum of little pieces of curve (infinitesimal arcs):
$$\begin{align*}
ds&= |d\mathbf{r}|=\left|\frac{d\mathbf{r}(t)}{dt}dt\right|=\left|\frac{d\mathbf{r}}{dt}\right|dt\\
&= \left|\frac{dx}{dt}\mathbf{i}+\frac{dy}{dt}\mathbf{j}+\frac{dz}{dt}\mathbf{k}\right|dt \\
&= \sqrt{\left(\frac{dx}{dt}\right)^{2}+\left(\frac{dy}{dt}\right)^{2}+\left(\frac{dz}{dt}\right)^{2}}~dt
\end{align*}$$
So that:
$$\begin{align*}
S=\int_{C}ds=\int_{C}|d\mathbf r|\\
=\int_{t=a}^{b}\sqrt{\left(\frac{dx}{dt}\right)^{2}+\left(\frac{dy}{dt}\right)^{2}+\left(\frac{dz}{dt}\right)^{2}}~dt
\end{align*}$$
