There are two different types of pendula that we are going to look at:
1) Mathematical Pendula
2) Physical/Compound Pendula
##### Mathematical Pendula
These consist of a mass $m$ attached to a massless string of length $L$:
![[Pasted image 20240229165639.png|center|150]]
If we consider the dynamics of the particle, where the free-body diagram is as follows:
![[Pasted image 20240229165741.png|center|200]]
![[Pasted image 20240229165759.png|center|250]]
So using small angle approximations:
$$\ddot{\theta}+\frac{g}{L}\theta=0$$
Resulting in:
![[Pasted image 20240229165947.png|center]]
The tension in the string can be found via:
![[Pasted image 20240229170304.png|center|600]]
Note that if we consider the extreme conditions:
1) Tension is minimum at $\theta=\pm\theta_0$, and $\dot{\theta}=0$
$$T_{min}=mg~cos~\theta_0 \approx mg\left(1-\frac{\theta_0^2}{2}\right)$$
2) Tension is maximum at $\theta=0$ and $\dot{\theta}=\dot{\theta}_{max}$
$$T_{max}=mg+mL\dot{\theta}_{max}^2=mg+mL\theta^2_0\frac{g}{L}$$
$$=mg(1+\theta_0^2)$$

##### Compound Pendula
A compound pendulum is a rigid body hinged around a point $O$, at distance $d$ from the centre of mass $G$. It is more realistic for a physical pendulum.
![[Pasted image 20240229171055.png|center|300]]
If we consider the dynamics of the rigid body:
![[Pasted image 20240229171139.png|center|350]]
This is very similar to the equations for a mathematical pendulum, as a result we can create a variable $L_{eq}$ (the equivalent length):
$$\ddot{\theta}+\frac{g}{L_{eq}}\theta=0$$
$$L_{eq}=\frac{I_O}{md}$$
Resulting in the oscillation frequency being:
$$f=\frac{1}{2\pi}\sqrt{\frac{g}{L_{eq}}}=\frac{1}{2\pi}\sqrt{\frac{mgd}{I_O}}$$