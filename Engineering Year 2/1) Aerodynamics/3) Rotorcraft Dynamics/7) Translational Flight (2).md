## A Recap of [[6) Translational Flight (1)|Last Time]]
![[Pasted image 20250302182756.png|centre]]
The forcing function (in forward flight) has a maximum and minimum value at $\psi=90$ degrees and $\psi=270$ degrees respectively. It follows then that the displacement has a maximum and minimum value at $\psi=180$ and $\psi=360$ degrees respectively. This means that in forward flight the rotor disc will pitch upwards (in the positive sense):
![[Pasted image 20250302183006.png|centre]]
## This Time
### Flapping and Feathering Equivalence
An autogyro has a flapping hinge, and no feathering hinge, but by directly tilting the rotor disk the effective pitch of the blades can be varied cyclically around the rotor azimuth - a form of cyclic pitch control:
![[Pasted image 20250302183215.png|centre]]
The powered rotor (helicopter) cannot be manually tilted with such ease. The fully articulated rotor head, controlled across the stationary/rotational interface by a swash plate, can apply collective and cyclic changes of pitch. 
![[Pasted image 20250302183610.png|centre]]
Thus the pitch can be cyclically changed to prevent the blades from flapping (in translational flight) and also address the problem of lift asymmetry.
$$\text{Blade Flap Angle}~~\beta=a_{0}-a_{1}\cos\psi-b_{1}\sin\psi-...$$
$$\text{Blade Pitch Angle}~~\theta=A_{0}-A_{1}\cos\psi-B_{1}\sin\psi-...$$
The longitudinal cyclic pitch angle input will counter the lateral rotor tilt.
### Swash Plate Mechanism
![[Pasted image 20250302184136.png|centre]]
![[Pasted image 20250302184152.png|centre]]
![[Pasted image 20250302184205.png|centre]]
![[Pasted image 20250302184217.png|centre]]
### Flapping ~ Feathering Equivalence
The amount of lateral cyclic pitch input $B_{I}$ applied, by forward stick input for the pilot, that is required to negate any rearward flapping of the rotor is equivalent to the flap angle $a_{1}$. This is referred to as **Flapping ~ Feathering Equivalence**.
![[Pasted image 20250302184355.png|centre]]
![[Pasted image 20250302184411.png|centre]]
![[Pasted image 20250302184424.png|centre]]
![[Pasted image 20250302184448.png|centre]]
For a pure helicopter the no flapping plane (also known as the tip-path-plane) must be inclined in the direction of flight in order to provide the necessary propulsive force. Thus the pilot pushes the stick forward more than just enough to counter the rotor flap back:
![[Pasted image 20250302184601.png|centre]]
![[Pasted image 20250302184613.png|centre]]
### Power and Induced Velocity in Translational Flight
The following is a breakdown of Helicopter Power Losses:
![[Pasted image 20250302185551.png|centre]]
#### Induced Velocity in Translational Flight
It can be seen that as the translational speed increases, the flow through the rotor is predominantly the component of the onset flow and an even more evenly distributed induced velocity results:
![[Pasted image 20250302185720.png|centre]]
Thrust:$$T=(\rho A v)2v$$ For the hovering rotor, resulting in:
$$v=\sqrt{\frac{T}{2\rho A}}$$
Clearly for translational flight the unit mass flow $\rho A v$ has increased as it now includes the translational component of flow through the rotor. So unit mass flow is $\rho A V'$, where:
$$V'=\sqrt{(V\cos\alpha)^{2}+(V\sin\alpha+v)^{2}}$$
![[Pasted image 20250302185946.png|centre]]
Thus $V'$ is the vector sum of the translational and induced velocities so in the original thrust equation:
$$T=(\rho A V')2v$$
So that:
$$v=\frac{T}{2\rho A V'}=\frac{C_{T}\rho A (\Omega R)^{2}}{2\rho A \Omega R\sqrt{\lambda^{2}+\mu^{2}}}$$
Thus, since it has been shown  that: $\lambda=\frac{V\sin\alpha +v}{\Omega R}$, and $\mu=\frac{V\cos\alpha}{\Omega R}$:
$$V'=\Omega R\sqrt{\lambda^{2}+\mu^{2}}$$
And therefore:
$$v=\frac{\frac{1}{2}C_{T}\Omega R}{\sqrt{\lambda^{2}+\mu^{2}}}$$
So, if $V=0$, then $\mu=0$, $\lambda=\frac{v}{\Omega R}$ and $v=\Omega R\sqrt{\frac{C_{T}}{2}}$
Which is the same as $v$ in hover.
