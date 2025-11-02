Let's now consider whether manoeuvring the aircraft makes it more or less stable. In the longitudinal sense this means inducing a non-zero pitch rate, which entails increasing the load factor from 1. This can be achieved in either a banked horizontal turn, or pulling out of a dive.
The latter is easier to treat as it is in the vertical plane.
### Flight in a Vertical Circle
The figure below shows the conditions associated with flight at the bottom of a vertical circular motion:
![[Pasted image 20251028231727.png|centre|500]]
The forward speed is $U=qR$ where $q$ is the pitch rate (or angular velocity) and $R$ is the radius of the pull-up manoeuvre. The centripetal acceleration is given by:
$$a_{c}=(n-1)g=\frac{U^{2}}{R}=q^{2}R=qU$$
So the $g$ being pulled can be related to the associated pitch rate by:
$$q=\frac{n-1}{U}g$$
Therefore for $n=1$ we have $q=0$ as expected.
The continuous pitch rate in the manoeuvre adds an increment in the incidence to the tailplane of:
$$\delta\alpha_{T}=\frac{ql_{H}}{U}$$
Where $l_{H}$ is the moment arm from the tailplane aerodynamic centre to the aeroplane c.g.
Referring to earlier notes the full tail incidence is then:
$$\alpha_{T}=i_{T}+\alpha(1-k)+\frac{ql_{H}}{U}$$
where $i_{T}$ is the tail setting angle relative to the zero-lift line of the wing, Substituting our equation for $q$ into this gives:
$$\alpha_{T}=i_{T}+\alpha(1-k)+\frac{n-1}{U^{2}}gl_{H}$$
We've therefore observed that there is an additional contribution to the tailplane incidence, but not to the wing incidence due to the pitch rate. This is because there is a negligible moment arm between the c.g. and the centre of lift, compared to the distance between the tailplane and the c.g.
However there is additional wing lift, which is required to produce the centripetal acceleration. The change in balance of lift forces between the wing and the tailplane to produce the pitching steady state condition is the reason why the new aerodynamic centre of the aircraft (the neutral point) is different from that in straight and level flight.
#### Stability and Manoeuvre Point/Margin
We can now consider the same criterion for testing stability as we did in [[10) Static Stability|the previous set of notes]]. Namely the restoring of aerodynamic stiffness, by looking at:
$$\frac{1}{a_{1}}\frac{\partial C_{M}}{\partial \alpha}=\frac{\partial C_{M}}{\partial C_{L}}$$
and requiring this to be negative as before. Thus we need to consider the pitching moment equation while allowing for the new incidence at the tail, and the greater overall lift on the aeroplane. The new lift requirement is:
$$Lift= nW=\frac{1}{2}\rho U^{2}S (C_{L_{W}}+\frac{S_{T}}{S}C_{L_{T}})$$
From this we can write:
$$\frac{n}{U^{2}}=\frac{\rho}{2w}(C_{L_{W}}+\frac{S_{T}}{S}C_{L_{T}})$$
where $w$ is the wing loading.
We now deploy the pitching moment equation, as derived in the static margin notes:
$$C_{M}=C_{M_{0}}+x\left(C_{L_{W}}+\frac{S_{T}}{S}C_{L_{T}}\right)-\bar{V}C_{L_{T}}$$
Which can be rewritten as:
$$C_{M}=C_{M_{0}}+xC_{L_{W}}-\left(\bar{V}-x\frac{S_{T}}{S}\right)C_{L_{T}}$$
And $C_{L_{T}}$ can be rewritten as a sum of the incidences and their lift curve slopes. The derivation for the following equation can be found [[Flight Dynamics Lecture 12 - Manoeuvre Stability.pdf#page=14|here]]. We can obtain:
![[Pasted image 20251028235535.png|centre|]]
Which we can partially differentiate to obtain:
![[Pasted image 20251028235605.png|centre|500]]
If we compare the static and manoeuvre static margin equations:
![[Pasted image 20251028235650.png|centre]]
Lets now define a few new terms:
$H_{M}$ is the **manoeuvre margin**
$h_{m}$ is the **manoeuvre point**
All of the extra terms in the manoeuvre margin compared with the static margin are positive so there is a larger margin of stability than in the static case.
![[Pasted image 20251028235854.png|centre]]
The result of this is that the more stable the aircraft the more tailplane deflection is needed to produce a nose-up vertical turn. This is the reason why fighter aircraft are designed to be unstable, as it increases their manoeuvrability.
#### Elevator Angle Per $g$
Another way to approach this problem is to consider the changes from steady level flight to instantaneous level flight at the bottom of the vertical circular motion.
We obtain the moment balance of:
$$C_{M}=C_{M_{0}}+xC_{L_{W}}-\left(\bar{V}-x\frac{S_{T}}{S}\right)C_{L_{T}}$$
This is still valid as $q$ is constant, i.e. there is no pitching acceleration.
Therefore the change in pitching moment from the manoeuvring terms in the equations must be zero.
![[Pasted image 20251029000317.png|centre]]
Under static conditions, the load factor $n=1$ so the third term in the $\alpha_{T}$ expression is zero. Therefore the pitching moment under static conditions can be written as:
![[Pasted image 20251029000412.png|centre|500]]
Rewriting this for the manoeuvring condition, we add a subscript n to designate factors in the equation that change between level flight and a pull up:
![[Pasted image 20251029000457.png|centre]]
Subtracting these two equations from each other gives us the change in $C_{M}$ due to the circular manoeuvre:
![[Pasted image 20251029000538.png|centre]]
![[Pasted image 20251029000553.png|centre]]
![[Pasted image 20251029000606.png|centre]]
#### Stick Force and Determination of Manoeuvre Point from Flight Tests
The stick force (which is proportional to the hinge moment) is closely related to the elevator deflection. To the pilot the stick force is a better indicator than elevator angle. Therefore the stick force per g has been a feature of flight testing to define performance/handling qualities in terms that a pilot can easily imagine.
A positive stick force $P$ is required to increase load factor $n$ for a stable aircraft and zero stick force per g would correspond to the c.g. being at the manoeuvre point.
![[Pasted image 20251029000842.png|centre]]
A flight test can be set up in which the stick force is measured for different load factors and repeated for several different CG positions, with the results plotted as in Fig. 3.
The slope of each of these $P$ vs $n$ lines can be determined.
![[Pasted image 20251029001001.png|centre]]
