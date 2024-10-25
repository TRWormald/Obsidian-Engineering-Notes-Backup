Example 5.4 would have been easier if we had used **cylindrical polar co-ordinates**:
$$x=r\cos\theta,~~y=r\sin\theta$$
In order to do that we need to know what an infinitesimal piece of area $dA$ is in polar coordinates.
![[Pasted image 20241025141443.png|centre|300]]
The above diagram shows us that $dA=r~dr~d\theta$, that is:
$$\int\int f(x,y) ~dx\cdot dy=\int\int f(r\cos\theta,r\sin\theta)~r\cdot dr\cdot d\theta$$
\
More generally, if we change co-ordinates to some other co-ordinate system:
$$x=x(u,v),~~~y=y(u,v)$$
then it can be shown that the infinitesimal piece of area:
$$dA=dx\cdot dy=\left|\frac{\partial(x,y)}{\partial(u,v)}\right|du~dv$$
Where the area scale factor:
$$|J|:=\left|\begin{matrix}\frac{\partial x}{\partial u} &\frac{\partial x}{\partial v}\\\frac{\partial y}{\partial u}&\frac{\partial y}{\partial v}\end{matrix}\right|$$
Is the determinant of the so called Jacobian matrix $J$
![[Pasted image 20241025142254.png|centre]]
#### Example 5.5
![[Pasted image 20241025141758.png|centre]]
