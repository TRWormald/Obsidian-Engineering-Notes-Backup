2D surfaces in our 3D world can be locally represented by a single scalar equation:
$$z=f(x,y)~~~~~~~~or~~~~~~~~g(x,y,z)=0$$
![[Pasted image 20241103160441.png]]
But in order to perform vector calculus on surfaces, it is much easier to have a parametric representation. Surfaces are 2D objects, therefore they need two parameters to describe them.
$$\mathbf{r}(u,v)=x(u,v)\mathbf{i}+y(u,v)\mathbf{j}+z(u,v)\mathbf{k}$$

Sometimes the choice of parameters is obvious:
- If the surface can be written as $z=f(x,y)$ then we can choose $(u,v)=(x,y)$ so that $z=f(u,v)$.
$$\mathbf{r}(u,v)=u\mathbf{i}+v\mathbf{j}+f(u,v)\mathbf{k}$$
- If one co-ordinate does not appear in $g(x,y,z)=0$
$$g(x,y)=0 \Rightarrow z=v ~~ and~ x=x(u),y=y(u)$$
For other surfaces, we can use an angular formulation:
- A cylinder of radius $a$. Parametrise the circular base as $x=a\cos u$, $y=a\sin u$, and the height $z$ as $v$. So that:
$$\mathbf{r}(u,v)=(a\cos u ,a\sin u,v)$$
- A cone $x^{2}+y^{2}=z^{2}$, which is similar, except the radius $a$ depends on $z$.
$$\mathbf{r}(u,v)=(v\cos u, v\sin u)$$