Lets now consider a 1 DOF damped system, with the following equation of motion and initial conditions:
![[Pasted image 20250115213654.png|centre]]
The EOM is a linear homogeneous differential equation with constant coefficients. This equation has the following exponential solution:
$$x(t)=Ae^{st}=Ae^{(s_{R}+iS_{I})t}=Ae^{S_{R}t} e^{iS_{I}t}$$
Where $s$ is a complex number, and $A$ is an unknown constant.
Therefore differentiating the above gives:
$$x=Ae^{st}\Rightarrow\dot{x}=sAe^{st}\Rightarrow\ddot{x}=s^{2}Ae^{st}$$
Which when substituted into the EOM gives:
$$(ms^{2}+cs+k)Ae^{st}=0$$
Which we can then solve as a quadratic in $s$ to get:
$$s_{1,2}=\frac{-c\pm\sqrt{c^{2}-4mk}}{2m}$$
In which we can get one of three results:
- two real solutions
- two complex solutions
- one (double) real solution

If we have **two distinct roots** then the total solution is:
$$x(t)=A_{1}e^{s_{1}t}+A_{2}e^{s_{2}t}$$
### Determining the Level of Damping
We can take the solution to the quadratic equation in $s$ and rearrange it to get:
$$s_{1,2}=-\frac{c}{2m}\pm\sqrt{\frac{k}{m}}\left(\frac{c^{2}}{4mk}-1\right)^{\frac{1}{2}}$$
The type of damping is determined by the part of the equation inside the brackets, if:
- $c^{2}/(4mk)>1$ then the system is overdamped
- $c^{2}/(4mk)<1$ then the system is underdamped
- $c^{2}/(4mk)=1$ then the system is critically damped

The ratio $\frac{c}{2(mk)^{\frac{1}{2}}}$ is dimensionless and is called the damping ratio $\zeta$:
$$\boxed{\zeta=\frac{c}{2\sqrt{mk}}}$$
So we can rewrite the equation above as:
$$s_{1,2}=-\zeta\omega_{0}\pm\omega_{0}(\zeta^{2}-1)^\frac{1}{2}$$
#### Underdamped Motion
In underdamped motion:
$$0<\zeta<1 \Rightarrow s_{1,2}=-\zeta\omega_{0}\pm \omega_{0}(\zeta ^{2}-1)^{\frac{1}{2}}$$
Which can be further simplified to be:
$$s_{1,2}=-\zeta \omega_{0}\pm i\omega_{0}\sqrt{1-\zeta ^{2}}$$
From which we can say that:
$$\boxed{\omega_{D}=\omega_{0}\sqrt{1-\zeta^{2}}}$$
Where $\omega_D$ is the damped natural frequency.
Hence solving the differential equation using the is we get:
$$x(t)=Ae^{-\zeta\omega_{0}t}\cos(\omega_{D}t-\phi)$$
Where the exponential is the decaying function, the first term inside the cosine is the harmonic motion with the natural damped frequency, and the final term is the phase lag due to damping.
#### Overdamped Motion
In overdamped motion:
$$\zeta>1 \Rightarrow s_{1,2}=-\zeta\omega_{0}\pm \omega_{0}\sqrt{\zeta^{2}-1}$$
Therefore solving the differential equation gives:
$$x(t)=e^{-\zeta\omega_{0}t}(A_{1}e^{\omega_{0}\sqrt{\zeta^{2}-1}t}+A_{2}e^{-\omega_{0}\sqrt{\zeta^{2}-1}t})$$
Where the oscillation is exponentially decaying aperiodic motion. Note that the terms inside the brackets represents a real non-oscillatory function.
#### Critically Damped Motion
In critically damped motion:
$$\zeta=1\Rightarrow s_{1,2}=-\omega_{0}$$
So there is a special solution due to having a double real root:
$$x(t)=(A_{1}+A_{2}t)e^{-\omega_{0}t}$$
### Experimental Identification of Damping
We can identify damping from the *free response* using the **Logarithmic Decrement**. Consider the free response of a 1DOF damped system in $t_{1}$ and $t_{1}+T_{D}$, where $T_{D}=2\pi/$