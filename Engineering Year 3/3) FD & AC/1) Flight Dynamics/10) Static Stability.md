### The Neutral Point and Static Margin
The **neutral point** is the rearmost position of the c.g. before an unstable condition occurs.
The **static margin** is a measure of the distance remaining through which the c.g. could be moved rearward before the aircraft displays neutral static stability.
### Static Stability
We can consider the static stability in terms of stiffness of the system.
![[Pasted image 20251027123858.png|centre|300]]
If we consider the system above, the force $F$ results in a displacement of $x$. Which gives us a positive slope $k$.
The spring also exerts an opposite but equal force, which is the force required to achieve equilibrium.
Stability deals with the tendency of a system to return to its previous condition after a perturbation. For a system to be stable the force it produces in response to a perturbation must tend to restore it to its unperturbed state.
![[Pasted image 20251027124401.png|centre]]
The flight mechanics case follows this sign convention and displays the displacement/force characteristics given earlier. Our study of stability will consider the pitching moment $\Delta M$ produced when there is a departure $\Delta\alpha$ away from the equilibrium flight altitude.
![[Pasted image 20251027124544.png|centre]]
The system is the pitch response of an aircraft, the input is a pitch displacement, and the output is the consequent pitching moment.
For stable flight we need $\Delta M\lt 0$ for $\Delta \alpha \gt0$ so that there will be a restoring action. This can be seen graphically below:
![[Pasted image 20251027124702.png|centre]]
If we consider a perturbation away from a trimmed, straight and level operating point what is more desirable? A +ve or -ve slope?
**Negative** as otherwise the aircraft is not stable.

>The static stability of an aircraft is commonly interpreted to describe its tendency to converge on the initial equilibrium condition following a small disturbance from trim. Dynamic stability, on the other hand, describes the transient motion involved in the process of recovering equilibrium following disturbances.

### The Neutral Point and Static Margin
![[Pasted image 20251027125044.png|centre]]
Note that our earlier use of c.g. position $x$ is replaced here by an alternative measure $h$ from the leading edge of the MAC ($x=h -\frac{1}{4}$)
### Static Stability - Definitions
If the coefficient form $\frac{\partial C_{M}}{\partial \alpha}$ is negative the aircraft will be stable. Remembering that $\alpha$ is $\alpha_{wing}$ and that we can put $\alpha_{wing}=C_{L_{W}}/a_{1}$, and hence there is only a constant factor that would distinguish between $\frac{\partial C_{M}}{\partial \alpha}$ and $\frac{\partial C_{M}}{\partial C_{L}}$. And as a result if the latter is negative then the aircraft will be stable.
![[Pasted image 20251027125431.png|centre|400]]
The image above shows stability reversal at high lift coefficients.
### The Pitching Moment Equation
#### Derivatives of the Pitching Moment Equation
We have previously found that:
![[Pasted image 20251027125537.png|centre|400]]
Now for trimmed flight $C_{M}=0$. Lets consider a disturbance in pitch $\Delta\alpha$, perhaps caused by an upward gust, resulting in an increase in the $C_{L}$.
This means that there will be a commensurate change in the pitching moment. From what we have seen earlier it should be clear that:
$$\Delta C_{M}>0 \text{ is adverse}\Rightarrow\text{the aircraft is unstable}$$
$$\Delta C_{M}<0 \text{ is restoring}\Rightarrow\text{the aircraft is stable}$$
And thus in general:
![[Pasted image 20251027125843.png|centre|400]]
### The Case For a Fixed Elevator
We will assume that the elevator is heled fixed by the pilot or that there is a control fixed condition imposed by the hydraulics when control demands remain constant.
With the stick free case there can be a small difference in the pitch stability if the elevator position is allowed to drift. Under such conditions, the nominal value $\eta=\eta_{trim}$ is not retained when the pitch attitude is disturbed.
![[Pasted image 20251028172821.png|centre]]
### Static Stability
If we consider:
![[Pasted image 20251027125537.png|centre|400|centre]]
and recall that:
$$C_{L}=C_{L_{W}}+\frac{S_{T}}{S}C_{L_{T}}$$
and that $\frac{S_{T}}{S}$ can be neglected. Then for the case where the elevator is locked and $\eta$ is constant we have, for static stability:
$$\frac{1}{a_{1}}\frac{\partial C_{M}}{\partial \alpha}=\frac{\partial C_{M}}{\partial C_{L}}=-\left[\bar{V}\frac{a_{1_{T}}}{a_{1}}(1-k)-x\right]<0$$
For $k$ of order 1/2 and with the c.g. behind the primary lift by a small distance (i.e. $x$ is small and positive), the terms in the brackets lead to a positive value. This will remain so, as the c.g. moves forward and passes the primary lift to make x<0. However, clearly $x$ could become sufficiently large and positive for the terms inside the brackets to become negative and then the aircraft would become unstable.
#### An Alternative Criterion For Pitch Stability
Another way of looking at the longitudinal stability is to use a logical argument which relates the lift coefficient and the $\eta_{trim}$ as follows for balanced flight:
1) If flight is to be at a faster speed, it must also be at a lower $C_{L}$ i.e. $\Delta C_{L}<0$
2) Therefore to obtain a lower $C_{L}$ we must push the nose down to obtain lower incidence
3) This lower incidence is obtained by a larger upward force at the tail via a more positive $\eta$ i.e. $\Delta \eta>0$, even if $\eta<0$
### Elevator Angle to Trim
We therefore obtain the elevator trim angle:
$$\eta_{trim}=\frac{1}{\bar V a_{2_{T}}}\left(C_{M_{0}}-\bar{V}a_{1_{T}}i_{T}-C_{L_{W}}\left[\bar{V}\frac{a_{1_{T}}}{a_{1}}(1-k)-x\right]\right)$$
### Static Stability
Thus in flight we should expect to have the change in elevator trim angle as positive as speed is increased whilst the change in lift coefficient becomes negative, and thus:
$$\frac{\partial \eta_{trim}}{\partial C_{L}}<0$$
Indeed a differentiation of the expression for $\eta_{trim}$ will show that this leads to:
$$\frac{\partial \eta_{trim}}{\partial C_{L}}=-\frac{1}{\bar V a_{2_{T}}}\left[\bar{V}\frac{a_{1_{T}}}{a_{1}}(1-k)-x\right]$$Clearly the right hand side will be negative if the bracketed expression is again positive.
![[Pasted image 20251028174658.png|centre|400]]
Because the bracketed terms in the equations above are the same the boundary between stable and unstable flight is shown by a zero value for that term and thus a horizontal line for the $\eta_{trim}$ vs $C_{L}$ graph.
### Lateral Static Stability
> Lateral static stability is concerned with the ability of the aircraft to maintain wings level equilibrium in the roll sense.

Thus the condition for an aircraft to be laterally stable is that the rolling moment resulting from a positive disturbance in roll attitude must be negative.
### Directional Static Stability
>Directional static stability is concerned with the ability of the aircraft to yaw or weathercock into the wind in order to maintain directional equilibrium.

![[Pasted image 20251028174943.png|centre|400]]
![[Pasted image 20251028175004.png|centre|400]]
### The Neutral Point and Static Margin
![[Pasted image 20251028175356.png|centre]]
Note that our earlier use of c.g. position $x$ is replaced here by an alternative measure $h$ from the MAC.
#### The Neutral Point
Stability becomes neutral when the c.g. moves back to the neutral point where:
$$h=h_{n},~~~~~~~~x=h_{n}- \frac{1}{4}$$
The stick fixed neutral point can be found by setting to zero the derivative that we saw earlier:
![[Pasted image 20251028175551.png|centre|400]]
![[Pasted image 20251028175609.png|centre|500]]
And this defines the stick fixed neutral point relative to the MAC, i.e. ...
#### Static Margin
The static margin is a measure of the distance remaining through which the c.g. could move rearward before the aircraft displays neutral static stability.
It is defined as the remaining distance divided by $\bar c$, so it is a chord-fraction and is given by:
$$h_{n}-h =H_{n}$$
Static margin is positive if the aircraft is still stable. Note that if in the large equation above if we insert $x=\frac{1}{4}$ we have:
![[Pasted image 20251028180012.png|centre|300]]
But from the equation for $h_{n}$ this is just:
![[Pasted image 20251028180054.png|centre|300]]
Which means that:
$$\frac{\partial C_{M}}{\partial C_{L}}=-H_{n}$$
Which shows that the static margin must be positive for positive static stability.