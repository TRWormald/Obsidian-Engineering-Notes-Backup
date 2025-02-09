A vortex sheet is placed on the chord line and as this is also the camber line it must be made a streamline of the flow:
![[Pasted image 20250209224304.png|centre]]
And with a symmetric aerofoil:
$$\frac{dz}{dx}=0$$
To make the chord line a streamline there must be no flow normal to it. So we need to find:
1) The component of the freestream velocity normal to the chordline:
![[Pasted image 20250209224405.png]]
2) The vortex induced velocity normal to the chordline $w(x)$
At a point $x$ on the chordline the vortex-induced velocity normal to the line is $w(x)$.
This is found by considering the velocity induced by a small element of the vortex sheet with strength $\gamma(\xi)d\xi$ located at distance $\xi$ from the origin on the chordline:
![[Pasted image 20250209224600.png]]
So using $v_{\theta}=-\frac{\Gamma}{2\pi r}$:
$$dw(x)=-\frac{\gamma(\xi)~d\xi}{2\pi(x-\xi)}$$
Then integrating to find total velocity induced by the whole sheet is:
$$\boxed{w(x)=- \frac{1}{2\pi}\int_{0}^{c}\frac{\gamma(\xi)}{x-\xi}~d\xi}$$
The no normal flow condition is then:
$$\boxed{V_{\infty}\sin(\alpha)+w(x)=0}$$
And for small angles:
$$V_\infty\alpha+w(x)=0$$
So substituting this becomes:
$$\boxed{\boxed{\frac{1}{2\pi}\int_{0}^{c}\frac{\gamma(\xi)~d\xi}{(x-\xi)}=V_{\infty}\alpha}}$$
This is the special form of the FUNDAMENTAL THIN AEROFOIL EQUATION for a symmetric aerofoil.
This **must be solved subject to the [[3) The Kutta Condition|Kutta Condition]]**
### The Fundamental Thin Aerofoil Equation
To solve this equation we use the following transformation:
$$\xi=\frac{c}{2}(1-\cos\theta)$$
$$x=\frac{c}{2}(1-\cos\theta_{0})$$
![[Pasted image 20250209225451.png|centre]]
Once substituting the Fundamental Thin Aerofoil Equation becomes:
$$\boxed{\boxed{\frac{1}{2\pi}\int_{0}^{\pi}\frac{\gamma(\theta)~\sin\theta}{(\cos\theta-\cos\theta_{0})}d\theta=V_{\infty}\alpha}}$$
This is solved using *integral equation theory*. We don't need to solve this. Given a function you need to be able to substitute in and confirm it is the solution of the equation (just don't forget the Kutta Condition)
### Exemplar
For a symmetric aerofoil the given function would be:
$$\boxed{\gamma(\theta)=2\alpha V_{\infty}\frac{1+\cos\theta}{\sin\theta}}$$
To prove it is the solution you need to show that:
1) It satisfies the equation
2) $\gamma(\pi)=0$ i.e. the Kutta condition at the TE is satisfied