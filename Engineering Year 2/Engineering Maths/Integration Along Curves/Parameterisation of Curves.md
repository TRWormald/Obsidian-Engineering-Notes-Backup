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
In 