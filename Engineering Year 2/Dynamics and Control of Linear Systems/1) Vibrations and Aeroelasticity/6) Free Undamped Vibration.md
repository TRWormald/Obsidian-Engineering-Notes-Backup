>Vibrating systems are dynamic systems. To be able to solve their EOMs, we have to know their initial state or initial conditions (IC)

From a mathematical perspective a 1DOF EOM is a second order linear ODE and to be able to solve it we have to know two initial conditions:
- Initial position $x(0)=x_{0}$
- Initial velocity $\dot{x}(0)=\dot{x}_{0}=v_{0}$

For a freely vibrating undamped system:
![[Pasted image 20250115212324.png]]
Which we assume is vibrating harmonically, resulting in the position being determined by the following equation:
$$x=A\sin(\omega t+\varphi) \Rightarrow \ddot{x}=-\omega^{2}A\sin(\omega t+\varphi)$$
If we substitute this back into the equation of motion:
$$(-\omega^{2}m+k)A\sin(\omega t+\varphi)=0$$
$$-\omega^{2}m+k=0 \Rightarrow \omega ^{2}=\frac{k}{m}$$
Therefore a free undamped 1 DOF system **vibrates harmonically with angular frequency proportional to the square root of k over m.** *Note that this is the natural frequency $\omega_{0}$*

For non-zero ICs we can apply them to $x$ and $\frac{dx}{dt}$ to solve for $A$ and $\varphi$, resulting in:
$$\boxed{A=\sqrt{x_{0}^{2}+\frac{v_{0}^{2}}{\omega^{2}_{0}}}}$$
$$\boxed{\varphi=\tan^{-1}\left(\frac{x_{0}\omega_{0}}{v_{0}}\right)}$$
It is now possible to rewrite the EOM:
$$\boxed{\ddot{x}+\omega_{0}^{2}x=0}$$
We have divided by $m$ and then substituted in $\omega_{0}=\sqrt{\frac{k}{m}}$.
### Rotational vs. Rectilinear Motion in 2D
![[Pasted image 20250115213530.png|centre]]


