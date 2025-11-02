### Tail Configurations 
There are three types of tail configurations that can be used to achieve trimmed conditions across the flight envelope:
##### 1) Fixed Tail + Elevator
In this case trim is achieved by adjusting the elevator to a datum position, probably different from $\eta=0$, with only the remaining elevator deflection being available for manoeuvring.
We will discuss later how to find the right fixed position for the horizontal tail - the tail setting angle.
##### 2) Trimming Tail + Elevator
The whole horizontal tail can be rotated in pitch to achieve trim with $\eta=0$; the elevator is then used only for additional (more rapidly changing) control (manoeuvring).
##### 3) All-Flying Tail & No Elevator
The datum position is selected for trim; control is then effected by additional movements of the whole tail away from this datum value.

### The Equation for the Elevator Angle to Trim
#### Local Airspeed
The velocity over the tail will not normally be the same as the free stream (note that some tail designs may not be affected), this is because of several factors:
- There will be a reduction in airspeed due to wing and fuselage frag
- There will be an increase in airspeed from the engine/propeller slipstream
We can account for these effects using an efficiency factor $\eta_{T}$. This can be modelled as:
$$U_{T}^{2}=\eta_{T}U^{2}$$
But $\eta_{T}$ is often simply taken to be 1. (assume to be 1 in the coursework unless told otherwise)
#### Downwash and Wake Effects at the Tail
Downwash created by vortices shed downstream from the main wing can alter the flow over the horizontal tail.
Consider the flow field at the horizontal tailplane, where the wing wake is well developed - we would expect that downwash would be significant.
![[Pasted image 20251023161251.png|centre]]
The angles of attack seen by the two lifting surfaces are not going to be equal and the distribution of $\alpha$ across the two surfaces from tip to tip is not going to be equal. 
Generally, the forward surface (while it is developing lift) will have a downward influence on the flow downstream so that the rearward surfaces sees a lesser AoA.
The lifting wing induces a downwash field in its wake.
Downwash also changes quite noticeably with wing angle of attack.
The change of angle is referred to as the downwash angle $\varepsilon$.
#### The Downwash Field
A wing will normally affect the whole of a tailplane with the wider wake causing downwash over the full span of the tail.
The effect of a canard surface will vary depending on whether the point considered is within or without the span of the canard.
A canard will produce additional downwash within the span of the canard, but upwash (leading to additional $\alpha$) outboard of its span.
*We will consider the conventional configuration.*
#### Simple Downwash Models for the Tail
Downwash at the tail is directly proportional to the lift being developed at the wing. In order to express the effective tail angle of attack at $\alpha_{T}$ we need to express $\varepsilon$ (the loss of incidence) at the tail in terms of $\alpha_{wing}$.
An approach is to employ a term $\alpha(1-k)$, where:
$$k=\frac{\partial\varepsilon}{\partial \alpha}$$
Therefore:
$$\alpha_{T}=\alpha-\frac{\partial \varepsilon}{\partial \alpha}\alpha$$
Where $\alpha$ is actually $\alpha_{wing}$, from the zero-lift attitude. Both of these terms become zero when there is no wing lift.
We need an expression for:
$$\varepsilon=\frac{\partial\varepsilon}{\partial \alpha}\alpha$$
One model which represents the downwash at the tailplane is:
$$\varepsilon=\left(\frac{1+\sec\delta}{2+A}\right)\alpha$$
Where $\alpha$ is the wing incidence from the zero lift attitude, and $A$ is the aspect ratio.
![[Pasted image 20251024002609.png|centre|200]]
An alternative expression, developed by Glauert and based on thin aerofoil theory is:
$$\varepsilon=\left(\frac{4}{\pi}\right)^{2}\left(\frac{1+\sec\delta}{2+A}\right)\alpha$$
An alternative empirical expression is:
$$\varepsilon=20C_{L}\frac{\lambda^{0.3}}{A^{0.725}}\left(\frac{3c}{l}\right)^{0.25}$$
Where $\varepsilon$ is in degrees, $c$ is the mean wing chord, $\lambda$ is the taper ratio, and $l$ is the distance aft of the wing quarter chord.
![[Pasted image 20251024002935.png|centre|300]]
Different approximations can be made for different tail positions and wing shapes. A linear approximation can be used for $\varepsilon$ dependency on $\alpha$, so we have:
$$k=\frac{\partial\varepsilon}{\partial\alpha}=constant$$
In the absence of better data, this constant can be approximated with $k=0.5$.
#### Elevator Angle to Trim
The three equations valid in the plane of symmetry are:
Transverse:
$$L_{W}+L_{T}=nW$$
Axial:
$$F=D$$
Pitch:
$$\begin{align*}
M_{ac}&= M_{0}+nWx\bar{c}-L_Tl_{T}\\
&= 0~~~~(\text{for equilibrium})
\end{align*}$$
To achieve longitudinal balance we need to satisfy the top and bottom equations above and then trim the aircraft to meet the following requirements:
a) Fly fast enough to produce the required lift
b) Achieve an angle of attack, related to the flight speed, to satisfy the conditions in the top equation; since the wing lift is dominant we tend to think of this as a requirement for wing $\alpha$ though it is not that simple, i.e. we need to consider the distribution of lift related to (c)
c) We need to achieve the pitch balance to satisfy the final equation by adjusting tail lift, noting that the adjustment of tail lift requires an equal and opposite change in the wing lift to keep the balance given by the first equation. We will use the elevator to change the tail lift and achieve the required balance.

Hence we will need to be able to calculate $\eta$ (required elevator deflection) for a given speed.
#### An Expression for the Elevator Angle $\eta$ 
Lets quickly list our variables and their states:
$$\begin{align*}
U&= \text{Fixed}\\
\alpha &= \text{Variable}\\
\eta&=\text{Variable}\\
i_{T}&= \text{Variable (tail setting angle)}
\end{align*}$$
Lets also consider the configuration (we will assume a conventional one):
![[Pasted image 20251024124331.png]]
Note that the tailplane is attached to the fuselage with a different basic incidence greater than the wing incidence by the setting angle $i_{T}$.
![[Pasted image 20251024124424.png|centre]]
Thus as illustrated on the previous slide, the effective angle of attack at the tail is:
$$\alpha_{T}=i_{T}+\alpha-\varepsilon$$
The downwash from the wing, which alters the angle of attack at the tail is proportional to $C_{L_{W}}$ and this in turn is proportional to $\alpha$ so we can say:
$$\varepsilon=\frac{\partial\varepsilon}{\partial\alpha}\alpha$$
Which implies that for $\varepsilon=0$ $\alpha=0$
Substituting this into the first equation:
$$\begin{align*}
\alpha_{T}&= i_{T}+\alpha\left(1-\frac{\partial\varepsilon}{\partial\alpha}\right)\\
&= i_{T}+\alpha(1-k)
\end{align*}$$
Where $k=\frac{\partial\varepsilon}{\partial\alpha}$.
>An approach in design could be to find/choose $i_{T}$ and then fic it and find $\eta$ for a new trim condition.

Then to involve the elevator explicitly we write the tail lift coefficient as:
$$\begin{align*}
C_{L_{T}}&= a_{1_{T}}\alpha_{T}+a_{2_{T}}\eta\\
C_{L_{T}}&= a_{1_{T}}(i_{T}+\alpha[1-k])+a_{2_{T}}\eta
\end{align*}$$
Which implies a symmetric section for the horizontal tailplane having $a_{0_{T}}=0$
We can now use the moment equation to solve for balance but we need to be careful to choose the correct reference point (a.c. vs c.g.)
#### Choice of Lift Coefficient $C_{L}$
We should really use the total $C_{L}$, with the consequence that:
$$\begin{align*}
C_{M_{ac}}&= M_{M_{0}}+xC_{L}\bar{V}-C_{L_{T}}\\
&= C_{M_{0}}+x\left[\frac{C_{L_{W}}+S_{T}}{S}C_{L_{T}}\right]-\bar{V}C_{L_{T}}\\
&= C_{M_{0}}+xC_{L_{W}}+\left(x\frac{S_{T}}{S}-\bar{V}\right)C_{T}
\end{align*} $$
And this makes both the $C_{L_{W}}$ and the $C_{L_{T}}$ terms dependent on $x$.
Lets then consider the factor:
$$\left(x\frac{S_{T}}{S}-\bar{V}\right)$$
Examples of the values of the two terms in this expression for a few civil aircraft are:
![[Pasted image 20251024143718.png|centre]]
The implication is that relative to $\bar{V}$, $x\frac{S_{T}}{S}$ can be ignored without great loss of accuracy due to it being much smaller than it.
#### Moment Balancing Using $\eta$ 
One of the advantages of simplifying the above equation is that we can write it as:
$$C_{M_{ac}}=C_{M_{0}}+xC_{L_{w}}-\bar{V}C_{L_{T}}$$
Which means we can take partial derivatives of the form:
$$\frac{\partial}{\partial\alpha}~~~\text{or}~~~\frac{\partial}{\partial C_{L}}$$
#### Elevator Angle to Trim Continued
We can then combine the lift acting on the tail and the moment balance:
$$C_{M_{0}}+xC_{L_{W}}-\bar{V}a_{1_{T}}(i_{T}+\alpha[1-k])-\bar{V}a_{2_{T}}\eta=0$$
However we have terms in $C_{L_{W}}$ and $\alpha$ that could be combined. We need to replace $\alpha$ with $\frac{C_{L_{W}}}{a_{1}}$ and gather terms in $C_{L_{W}}$ to obtain:
$$C_{M_{0}}-\bar{V}a_{1_{T}}-C_{L_W}\left[\bar{V}\frac{a_{1_{T}}}{a_{1}}(1-k)-x\right]-\bar{V}a_{2_{T}}\eta=0$$
And thus the elevator angle required to obtain this trim is:
$$\eta_{trim}=\frac{1}{\bar{V}a_{2_{T}}}\left(C_{M_{0}}-\bar{V}a_{1_{T}}i_{T}-C_{L_{W}}\left[\bar{V}\frac{a_{1_{T}}}{a_{1}}(1-k)-x\right]\right)$$
Which displays that the elevator angle to trim is a linear function of $C_{L_{W}}$.
#### Choosing $i_{T}$
Generally for a fixed tailplane, $i_T$ will be chosen to obtain trim in cruise without having to use the elevator.
Obviously changes in speed and c.g. position will alter the need for $\eta$, so at best the value of $i_{T}$ that required $\eta=0$ is only correct at one instantaneous condition.
For an adjustable horizontal tail, the whole cruise can be flown at $\eta=0$ while $i_{T}$ is adjusted continually. 