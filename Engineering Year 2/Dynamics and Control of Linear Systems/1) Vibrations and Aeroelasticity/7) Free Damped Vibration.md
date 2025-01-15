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

The ratio $\frac{c}{2(mk)^{\frac{1}{2}}}$ is dimensionless and is called the damping ratio $\zeta$ so we can rewrite the equation above as:
$$s_{1,2}=-\zeta\omega_{0}\pm\omega_{0}(\zeta^{2}-1)^\frac{1}{2}$$
#### Underdamped Motion

#### Overdamped Motion

#### Critically Damped Motion
