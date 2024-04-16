### The Basics
When turning you need to have a resultant force to the side (towards the centre of the turn):
![[Pasted image 20240415121648.png|center|250]]
We could use the rudder to provide this **sideforce** - with the wings held horizontal in a **flat turn**.
This is very inefficient as the sideforce is small (resulting in a large turn radius) and the drag increase due to fuselage **sideslip** is significant.
\
It is far more efficient to **bank** or **roll** the aircraft so that part of the lift acts in the horizontal plane giving a **banked turn**:
![[Screenshot 2024-04-15 121920 1.png|center|300]]
This is advantageous as there is a large force available so tight turns are possible and the aerodynamic loads remain symmetrical (left to right in the aircraft frame of reference).
### Load Factor in a Steady Banked Turn
Consider an aircraft turning with a radius $R$ and at steady speed $V$:
![[Screenshot 2024-04-15 122939.png|center|300]]
The thrust and drag are balanced, and the correct **bank angle $\phi$** is set so there is no sideslip, note that $V$ is [[Level Flight#True Air Speed (TAS)|True Air Speed]].
If we resolve the forces vertically:
$$L\cos\phi = W$$
$$L=nW$$
Where $n$ is the load factor at any given point in time.
Therefore:
$$\boxed{\cos\phi=\frac{1}{n}}$$
Hence high load factors require large bank angles.
### Turn Radius
![[Screenshot 2024-04-15 122939 1.png|center|300]]
In the horizontal plane the lift component provides the horizontal resultant force, $F_{r}$, to maintain the curved flight path.
$$F_{r}=\sqrt{L^{2}-W^{2}}=W\sqrt{n^{2}-1}$$
$$F_{r}=m \frac{V^{2}}{R}=\frac{W}{g} \frac{V^{2}}{R}$$
Where the second equation is the equation for the [[Centripetal Force]].
Hence:
$$\boxed{R= \frac{V^{2}}{{g\sqrt{n^{2}-1}}}}$$
We can note that the radius decreases as $n$ (and $\phi$) increase, and that it also increases as $V$ increases.
The **minimum turn radius** $R_{min}$ occurs at maximum load factor $n_{max}$.
And for a given load factor $R_{min}$ occurs at $V_{min}$.

### Turn Rate
We can calculate the angular velocity of the plane using:
$$\boxed{\omega_{t}=\frac{V}{R}}$$
Combining this with the equation for turn radius above:
$$\boxed{\omega_{t}=\frac{g\sqrt{n^{2}-1}}{V}}$$
Hence the turn rate (the rate of change of heading) increases as $n$ increases, and decreases with $V$.
**Maximum turn rate** $\omega_{max}$ occurs at max load factor $n_{max}$
For a given load factor $\omega_{max}$ occurs at $V_{min}$
\
The time to turn through a given angle is also important, for example the time to reverse heading:
$$t_{180}=\frac{\pi}{\omega_{t}}= \frac{\pi R}{V}= {\frac{\pi V}{g\sqrt{n^{2}-1} }}$$
### Limits of Turn Performance
Whilst turning an aircraft is limited by its [[Manoeuvring Flight#Manoeuvre Envelope|Manoeuvre Envelope]] and by the amount of thrust it can produce.
Sustained (steady) turn performance is a function of $V$ and $n$, however note that the instantaneous turn rate might be higher.
There are several **physical constraints** that an aircraft faces, namely stall, load factor, and thrust.
#### Stall Limited Turn
On the stall boundary of the manoeuvre flight envelope $n$ is limited by $C_{L_{max}}$:
![[Pasted image 20240415130459.png|center||200]]
We know that in straight and level flight:
$$W=\frac{1}{2}\rho V_{S1}^{2}SC_{L_{max}}$$
And at load factor $n$:
$$nW=\frac{1}{2}\rho V^{2}SC_{L_{max}}$$
Where $n$ is equal to:
$$n=\left(\frac{V}{V_{S1}}\right)^{2}$$
So substituting into the turn performance equation:
$$R=\frac{V^{2}}{g\sqrt{\left(\frac{V}{V_{S1}}\right)^{4}-1 }}$$
Which can be rearranged to:
$$R=\frac{V_{S1}^{2}}{g}\left(1-\left(\frac{V_{S1}}{V}\right)^{4} \right)^{-\frac{1}{2}}$$
From this we can see that there is very little effect from $V$ on turn radius $R$, as $(V_{S1}/V)^{4}$ becomes very small.
The only exception to this is where $n$ is close to one (i.e. where $V\approx V_{S1}$). In which case the turn radius trends to zero.
The time to turn $t_{180}$ reduces significantly as speed increases:
$$t_{180}=\pi \frac{R}{V}=\pi \frac{V_{S1}}{g}\left(\frac{V_{S1}}{V}\right)\left(1-\left(\frac{v_{S1}}{V}\right)^4\right)^{-\frac{1}{2}}$$
#### Load Factor Limited Turn
We know that the maximum manoeuvrability is achieved at the [[Manoeuvring Flight#The Manoeuvre Point|Manoeuvre Point]], where the load factor reaches it maximum permissible value $n_{max}$ resulting in:
$$R=\frac{V^{2}}{g\sqrt{n_{max}^{2}-1}}$$
$$t_{180}=\pi \frac{R}{V}= \frac{\pi V}{g\sqrt{n_{max}^{2}-1}}$$
So radius $R$ increases rapidly with $V^{2}$, and time to turn $t_{180}$ increases with $V$. Hence the best turn performance is at the manoeuvre point on the manoeuvre flight envelope, which occurs at the corner speed, $V^{*}$.
The maximum bank angle is constant:
$$\cos\phi_{max}=\frac{1}{n_{max}}$$
##### Example
![[Pasted image 20240415160417.png|center]]
In this example we can see the stall and load factor limited turn radii, below $V^{*}$ the stall limit is what governs our turn radius, whilst above it its the load factor.
**Typically** at lower speeds we will be limited by stall, whilst at higher speeds we will be limited by load factor.
We can see a similar relationship in the time to turn:
![[Pasted image 20240415160616.png|center]]
#### Thrust Limited Turn
An increase in load factor leads to an increase in drag:
$$D=\underbracket{\frac{1}{2}\rho V^{2}SC_{D_{0}}}_{\text{independent of n}}+\underbracket{\frac{K(nW)^{2}}{\frac{1}{2}\rho V^{2}S}}_{\text{scales with }n^{2}}$$
And as a result our drag increment (for a given load factor $n$) will be:
$$\Delta D = \frac{KW^{2}}{\frac{1}{2}\rho V^{2}S}(n^{2}-1)=\Delta T $$
Where the change in drag is equal to the change in thrust the propulsion system will have to generate to maintain the turn.
\
We can get the following from the turn equation:
$$R=\frac{V^{2}}{g\sqrt{n^{2}-1}}\Rightarrow n^{2}-1 = \frac{V^{4}}{R^{2}g^{2}}$$
Hence:
$$\Delta D=\Delta T=\frac{KW^{2}}{\frac{1}{2}\rho S g^{2}} \frac{V^{2}}{R^{2}}$$
And as $\Delta P=\Delta T\times V$:
$$\Delta P=\frac{KW^{2}}{\frac{1}{2}\rho S g^{2}} \frac{V^{3}}{R^{2}}$$
So thrust or power required rise rapidly with increasing speed $V$ and/or reducing turn radius $R$.
We can see the impact of this in the plot below:
![[Pasted image 20240416090925.png|center]]
In it we can see the velocity at the manoeuvre point ($V^{*}$) has a very high drag and as a result it might not be optimum to try to turn at it if you don't have sufficient thrust.
Note that the blue stall boundary line is plotted against the TAS and varies with $n$. 
\
We see a similar behaviour with the graph showing power:
![[Pasted image 20240416091210.png|center]]
Although we see that the power required at the manoeuvre point is much closer to the minimum power than it was to the minimum drag in the original plot.
## Summary
![[Pasted image 20240416091531.png|center|300]]
For a turning aircraft:
$$\cos\phi=\frac{1}{n}$$
$$R=\frac{V^{2}}{g\sqrt{n^{2}-1}}$$
$$\omega_t=\frac{g\sqrt{n^{2}-1}}{V}$$ And turn performance is limited by:
- Stall onset
- Maximum load factor
- Power or Thrust available