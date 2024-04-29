Some basic definitions we will need for this section:
- Endurance - This is the time an aircraft can remain in flight
- Range - This is the horizontal distance that an aircraft can cover.
There are some other important variations on these definitions:
\
**Safe Range**
This is the maximum distance between two airfields for which an aircraft can fly a safe and reliably regular service with a specified payload
Calculating it requires a lengthy calculation of the full mission profile, including take-off/climb/cruise/descent/landing, headwinds, diversion allowance etc.
Therefore we use Still Air Range (SAR) as a simplification this is a scenario where the plane takes off with full fuel, climbs to cruise altitude, and then cruises until all fuel is expended
**Gross Still Air Range (GSAR)**
This is where a plane begins at a selected altitude with full fuel, cruises until all fuel is used.
The approximate factor between GSAR and Safe Range is known so we can use it to estimate the latter.

### The Breguet Range Equation
Originally derived by Coffin in the 1920s; it is a simple and compact way of calculating GSAR. The key assumption made is that *the rate at which fuel is burnt is equal to the rate at which the aircraft weight is reduced*.
We must define thrust specific fuel consumption (TSFC or $f$) as the mass of fuel burnt per unit of thrust per second. It has units of kilograms per newton second, however it is sometimes given in kilograms per newton hour.
For thrust $T$ and weight $W$ the basic Breguet equation is:
$$\frac{dW}{dt}=-fgT$$Which is a differential equation in units of $N/s$.
By rearranging and substituting $T=D$ and $W=L$:
$$dt=-\frac{dW}{fgT}$$
$$T=\frac{D}{L}W=\frac{C_{D}}{C_{L}}W$$
So:
$$dt=- \frac{1}{fg} \frac{C_{L}}{C_{D}} \frac{dW}{W}$$
#### Finding Endurance
We can assume that $C_{L}/C_{D}$ and $f$ remain constant, and therefore we can integrate from start weight $W_{1}$ to end weight $W_{2}$ to obtain the endurance $E$:
$$\begin{align*}
E=\int_{t_{1}}^{t_{2}}dt=t_2-t_1&=- \frac{1}{fg} \frac{C_{L}}{C_{D}}\int_{W_{1}}^{W_{2}} \frac{1}{W}\cdot dW\\
&= - \frac{1}{fg} \frac{C_{L}}{C_{D}}\ln\left(\frac{W_{2}}{W_{1}}\right)\\
&= \frac{1}{fg} \frac{C_{L}}{C_{D}}\ln\left(\frac{W_{1}}{W_{2}}\right)
\end{align*}$$
So:
$$\boxed{E=t_{2}-t_{1}=\frac{1}{fg} \frac{C_{L}}{C_{D}}\ln\left(\frac{W_{1}}{W_{2}}\right)}$$
Hence the maximum endurance occurs at maximum $C_{L}/C_{D}$:
$$C_{D_{max~E}}=2C_{D_{0}},~~~~~C_{L_{max~E}}=\sqrt{C_{D_{0}}/K}$$
Where $K=\frac{1}{\pi AR e}$, and $e$ is the Oswald efficiency factor.
#### Finding Range (Given constant airspeed)
We can say that an increment in distance $dS$ at velocity $V$ is given by:
$$\boxed{dS=Vdt=- \frac{V}{fg} \frac{C_{L}}{C_{D}} \frac{dW}{W}}$$
We can assume that the true air speed $V$ remains constant, and then integrate from start weight to end weight to obtain the range $R$:
$$\boxed{R=S_2-S_{1}=\frac{V}{fg} \frac{C_{L}}{C_{D}}\ln\left(\frac{W_{1}}{W_{2}}\right)}$$
#### The Implications of our Assumptions
We have assumed that $C_{L}/C_{D}$, $f$, and $V_{TAS}$ are constant, this is only true in a particular set of circumstances. As fuel is burnt the weight will decrease and hence the required lift $L$ reduces. If $V_{TAS}$ is held constant then either $C_{L}$ and/or $\sigma$ must reduce.
Since we've assumed constant $C_{L}/C_{D}$ our $C_{L}$ must be constant, therefore our only option is that $\sigma$ decreases and therefore **altitude must increase**.
Constant $C_{L}/C_{D}$ also implies constant $C_D$, therefore drag $D$ decreases in proportion to $\sigma$.
Since $T=D$, thrust must also decrease with altitude while constant SFC implies constant throttle setting.
**In order to create this maximum range scenario we have had to come up with a flight profile where altitude is constantly increasing whilst thrust is kept constant. This is called Cruise-Climb.**
Reviewing the equation for range:
$$\boxed{R=S_2-S_{1}=\frac{V}{fg} \frac{C_{L}}{C_{D}}\ln\left(\frac{W_{1}}{W_{2}}\right)}$$
We can make several interesting observations about it:
- $fg$ is a measure of thermodynamic efficiency - i.e. we want to minimise fuel consumption
- We want to maximise our speed $V$ as this results in a better fuel efficiency
- $C_{L}/C_{D}$ is a measure of aerodynamic efficiency - i.e. we want to minimise drag.
- $W_{1}/W_{2}$ is a measure of structural efficiency - i.e. we want to minimise the fixed weight $W_{2}$

##### A more common notation for commercial aircraft is:
$$\boxed{R=\frac{a}{fg}\left(M \frac{L}{D}\right)\ln\left(\frac{W_{1}}{W_{2}}\right)}$$
Where $a$ is the speed of sound $M$ is the Mach number, and $M(L/D)$ becomes the important aerodynamic parameter for range.
#### Range at Constant Altitude
If we assume altitude is constant ($\rho$ must be constant) and that $C_{L}$ is held constant **we must not have constant speed**, so:
$$V=\sqrt{\frac{W}{\frac{1}{2}\rho SC_{L}}}$$
Which when substituted into our range equation gives:
$$dS=- \frac{1}{fg}\sqrt{\frac{2}{\rho S}} \frac{C_{L}^{\frac{1}{2}}}{C_{D}} \frac{dW}{W^{\frac{1}{2}}}$$
And then integrating:
$$\boxed{R=\sqrt{\frac{8}{\rho S}} \frac{1}{fg} \frac{C_{L}^{\frac{1}{2}}}{C_{D}}\left(W_{1}^{\frac{1}{2}}-W_{2}^{\frac{1}{2}}\right)}$$
A constant altitude means that as we burn fuel we must reduce the throttle resulting in some variation in SFC.
#### Maximum Range - Cruise-Climb
If we specify a start altitude defined by $\sigma_1$ and let thrust vary as required, to maximise range we will therefore have to maximise $V(C_{L}/C_{D})$ and since $\sigma$ isn't a variable we can substitute the speed equation for $V$:
$$V \frac{C_{L}}{C_{D}}=\sqrt{\frac{W_{1}}{\frac{1}{2}\sigma_1\rho_{0}S}} \frac{C_{L}^{\frac{1}{2}}}{C_{D}}$$
Therefore we need to find the maximum of $C_{L}^\frac{1}{2}/C_D$ or the minimum of $C_{D}/C_{L}^{\frac{1}{2}}$.
We know that $C_{D}=C_{D_{0}}+KC_{L}^{2}$ hence:
$$\frac{C_{D}}{C_{L}^{\frac{1}{2}}}=\frac{C_{D_0}}{C_{L}^{\frac{1}{2}}}+KC_{L}^{\frac{3}{2}}$$
Differentiating:
$$\frac{d(C_{D}/C_{L}^{\frac{1}{2}})}{dC_{L}}=-\frac{1}{2}\frac{C_{D_0}}{C_L^{\frac{3}{2}}}+\frac{3}{2}KC_L^{\frac{1}{2}}$$
So at the maximum point:
$$\boxed{C_{D_{max~R}}=\frac{4}{3}C_{D_0},~~~C_{L_{max~R}}=\sqrt{C_{D_{0}}/3K}}$$
We can then substitute these values, along with $W_1$ and $\sigma_1$ in to the Breguet Equation to find range. 
#### Jet Cruise-Climb Range
The following plot shows how the range varies with $C_L$ based on the starting altitude of cruise:
![[Pasted image 20240314183735.png|center|500]]
It is interesting to note that the maximum range occurs at a $C_{L}$ much lower than that which gives the minimum drag and minimum power.
#### Maximum Range - Constant Altitude
We know range at constant altitude can be given by:
$$\boxed{R=\sqrt{\frac{8}{\rho S}} \frac{1}{fg} \frac{C_{L}^{\frac{1}{2}}}{C_{D}}\left(W_{1}^{\frac{1}{2}}-W_{2}^{\frac{1}{2}}\right)}$$
For maximum range we need $C_{D}/C_{L}^{\frac{1}{2}}$ to be minimum, just like in cruise-climb.
So we will once again have:
$$\boxed{C_{D_{max~R}}=\frac{4}{3}C_{D_0},~~~C_{L_{max~R}}=\sqrt{C_{D_{0}}/3K}}$$
Which we will substitute into our range equation along with the atmospheric density $\rho$.