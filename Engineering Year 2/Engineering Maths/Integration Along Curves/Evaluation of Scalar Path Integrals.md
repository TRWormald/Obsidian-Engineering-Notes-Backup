To evaluate the scalar path integrals of the form:
$$\int_{C}f(\mathbf{r})~ds=\int_{C}f(\mathbf{r})|d\mathbf{r}|$$
from points $A$ to $B$ along the curve $C$:
1) Parameterise the curve $C$ as $\mathbf r(t)=(x(t),y(t),z(t))$
2) Work out the limits $a$ and $b$ on $t$
3) Calculate
$$\begin{align*}
ds&= |d\mathbf{r}|=\left|\frac{d\mathbf{r}(t)}{dt}dt\right|=\left|\frac{d\mathbf{r}}{dt}\right|dt\\
&= \left|\frac{dx}{dt}\mathbf{i}+\frac{dy}{dt}\mathbf{j}+\frac{dz}{dt}\mathbf{k}\right|dt \\
&= \sqrt{\left(\frac{dx}{dt}\right)^{2}+\left(\frac{dy}{dt}\right)^{2}+\left(\frac{dz}{dt}\right)^{2}}~dt
\end{align*}$$
4) Evaluate the scalar field $f$ along $\mathbf r(t)=(x(t),y(t),z(t))$ and integrate with respect to $t$.
$$\int_{C}f(\mathbf{r})~ds=\int_{t=a}^{b}f(x(t),y(t),z(t))\sqrt{\left(\frac{dx}{dt}\right)^{2}+\left(\frac{dy}{dt}\right)^{2}+\left(\frac{dz}{dt}\right)^{2}}~dt$$
We have already seen examples of this:
- Total arclength $S$ is just the scalar path integral $S=\int_{C}1~ds$ of the field $f(\mathbf{r})=1$.
#### Example 4.3
![[Pasted image 20241012131736.png|centre]]
![[WhatsApp Image 2024-10-12 at 13.34.17_5737ef5d.jpg|centre]]
![[WhatsApp Image 2024-10-12 at 13.34.17_da3627bf.jpg|centre]]
