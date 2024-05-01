## Gliding Flight
#### Forces in Gliding and Glide Angle
When gliding $T=0$ however $D\neq0$, as a result you cannot maintain equilibrium in straight and level flight.
Therefore the aircraft descends at **glide angle** $\theta$
The component of weight along the flight path replaces thrust:
![[Aircraft Gliding Diagram.png|center|500]]
We can then calculate the **force balance**:
$$\boxed{L=W~cos\theta}$$
$$\boxed{D=W~sin\theta}$$
Therefore:
$$\boxed{tan\theta = \frac{1}{L/D}=\frac{1}{C_L/C_D}}$$
The glide angle depends solely on the aerodynamic characteristics, with weight only affecting the **speed** at which a particular $C_L/C_D$ is achieved.
The best (shallowest) glide angle occurs at maximum $L/D$.
$\Rightarrow$ Minimum glide angle occurs at minimum drag speed (See [[Level Flight#Minimum Drag Speed]])
The minimum glide angle creates the best glide ratio (which is equal to the distance forward/the distance down) which is equal to the lift to drag ratio.
#### Speed for Minimum Glide Angle
We know that minimum glide angle occurs at the minimum drag condition, resulting in the maximum distance from a given start height. However the speed depends on glide angle:
$$V=\sqrt{\frac{L}{\frac{1}{2}\rho S C_L}}=\sqrt{\frac{W~cos\theta}{\frac{1}{2}\rho S C_L}}=\sqrt{\frac{W}{\frac{1}{2}\rho S C_L}}\sqrt{cos\theta}$$
So for a given $C_L$, speed is less than that of level flight by the factor $\sqrt{cos\theta}$.
But if we use a small angle approximation then for any glide angle less than 10 degrees the error is less than 1%.
Hence we can say that:
$$L\approx W~~~\Rightarrow~~~V_{min~\theta}\approx V_{MD}=\left(\frac{2W}{\rho S}\right)^{\frac{1}{2}}\left(\frac{K}{C_{D_0}}\right)^{\frac{1}{4}}$$
Which is the same result as in [[Level Flight#Minimum Drag Speed]].
#### Speed for Minimum Sink Rate
The sink rate $v$ is  the vertical component of the flight speed $V$:
$$\boxed{v=V~sin\theta}$$
If we again make our small angle approximation such that $L\approx W$:
$$v=V\frac{D}{W}\approx V\frac{D}{L}=V\frac{C_D}{C_L}$$
So:
$$\boxed{v=\sqrt{\frac{2L}{\rho S C_L}}\frac{C_D}{C_L}\approx\sqrt{\frac{2W}{\rho S}}\frac{C_D}{C_L^{3/2}}}$$
Which is the same as the minimum power condition from [[Power#Minimum Power Required]]:
$$\boxed{V_{min~sink}\approx V_{MP}=\left(\frac{2W}{\rho S}\right)^{\frac{1}{2}}\left(\frac{K}{3C_{D_0}}\right)^{\frac{1}{4}}}$$
#### Glider Polar Diagram
Glider performance is represented by the graph of sink speed $v$ vs forward speed $V$. The gradient indicates the variation of $D/L$ with speed.
![[Glide Polar (Sink Speed vs Airspeed).png|center|400]]


### Climbing Flight
In climbing flight $T>D$, so the aircraft cannot maintain equilibrium in straight and level flight, hence the aircraft ascends at climb angle $\theta$.
The horizontal component of the weight opposes thrust:
![[Aircraft Climbing Flight Diagram.png|center|500]]
#### Force Balance in a Climb
If we resolve forces parallel and perpendicular to the aircraft we get:
$$\boxed{L=W~cos\theta}$$
$$\boxed{T-D=W~sin\theta}$$
Hence the climb angle is equal to:
$$\boxed{sin\theta=\frac{T-D}{W}}$$
And the rate of climb $v$ is then:
$$\boxed{v=V~sin\theta=\frac{V(T-D)}{W}}$$
Which when rearranged gives us:
$$\boxed{Wv=TV-DV}$$
Where $Wv$ is the rate of increase of potential energy, $TV$ is the available power, and $DV$ is the power required. This makes sense as if $TV=DV$ then there is no increase in potential energy.
#### Climb Performance
There are several important takeaways:
- Maximum angle of climb requires maximum excess thrust ($T-D$)
- Maximum rate of climb requires maximum excess power.
- These do not occur together, they depend on the thrust/power characteristics:
![[Pasted image 20240308161259.png|center]]
(as seen above the best angle will allow you to gain altitude in the shortest horizontal distance, however it will not necessarily be the greatest altitude you could have achieved in an equal amount of time)
- We can also not make small angle assumptions so we have to calculate numerically.
### Impact of Propulsion type on available thrust and power
In simple terms:
**Jet Aircraft**
- Thrust remains constant with speed
- Power increases linearly with speed ($P=TV$)
![[Thrust and Power Variation with TAS (Jet).png|center|300]]
**Propeller Aircraft**
- Thrust reduces with speed ($T=P/V$)
- Power output remains constant with speed.
![[Thrust and Power Variation with TAS (Propeller).png|center|300]]
#### Climb Angle for a Jet
![[Jet Climb Excess Thrust (Climb Angle) Polar.png|center]]
#### Rate of Climb for a Jet
![[Jet Climb Excess Power (Climb Rate) Polar.png|center]]
#### Climb Angle for a Prop Powered Aircraft
![[Prop Aircraft Climb Excess Thrust (Climb Angle) Polar.png|center]]
#### Rate of Climb for a Prop Powered Aircraft
![[Prop Aircraft Climb Excess Power (Climb Rate) Polar.png|center]]
### Climb Performance Summary
![[Pasted image 20240308161435.png|center]]
