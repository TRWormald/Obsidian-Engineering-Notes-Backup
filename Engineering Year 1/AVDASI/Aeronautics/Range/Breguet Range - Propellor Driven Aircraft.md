As a recap we know that the [[Breguet Range - Jet#The Breguet Range Equation|Breguet Range Equation for a jet is]]:
$$\frac{dW}{dt}=-fgT$$
However for propellor aircraft we use Power instead of Thrust, so:
$$\boxed{\frac{dW}{dt}=-fgP}$$
Where $f$ is the mass of fuel burnt per unit of power per second, $W$ is the weight of the aircraft, $g$ is the acceleration due to gravity, and $P$ is the power of the aircraft's engines.
### Calculating Endurance
So the power delivered by the propellor (where $\eta$ is the propellor efficiency):
$$\eta P=DV$$
Where $D$ is the drag on the aircraft, and $V$ is the velocity of the aircraft. This is required as for Jet aircraft we know that the drag is equal to the thrust, however there is an additional source of energy loss for propellor aircraft which is represented by the propellor efficiency.
So:
$$\frac{dW}{dt}=-fg \frac{DV}{\eta}~~~\Rightarrow~~~dt=- \frac{\eta}{fgV} \frac{C_{L}}{C_{D}} \frac{dW}{W}$$
Hence if we integrate we get (assuming that $C_{L}/C_{D}$ remain constant-the same as Jet [[Breguet Range - Jet#The Implications of our Assumptions|cruise climb]]):
$$\boxed{E_{prop}=t_{2}-t_{1}=t_{12}=\frac{\eta}{fg} \frac{1}{V} \frac{C_{L}}{C_{D}}\ln\left(\frac{W_{1}}{W_{2}}\right)}$$
#### Finding Maximum Endurance
For maximum endurance we require $\frac{\frac{C_{L}}{C_{D}}}{V}$ to be a maximum or $\frac{VC_{D}}{C_{L}}$ to be a minimum.
If we expand the above term:
$$V \frac{C_{D}}{C_{L}}=\frac{VD}{L}=\frac{VD}{W}$$
We know that $D\times V$ is the power required to overcome drag, and we want to minimise $\frac{VD}{W}$ so **maximum endurance is achieved at minimum power speed for propellor driven aircraft**.
Note that this is much much slower than for jet aircraft, and compares with glider performance.
So we need to maximise:
$$\frac{C_{L}^{\frac{2}{3}}}{C_{D}}$$
### Calculating Range
The increment in distance $dS$ at velocity $V$ is given by:
$$dS=Vdt=- \frac{\eta}{fg} \frac{C_{L}}{C_{D}} \frac{dW}{W}$$
We can then integrate from the start weight $W_{1}$ to end weight $W_{2}$ to obtain the range $R$:
$$\boxed{R_{prop}=S_{2}-S_{1}=\frac{\eta}{fg}\left(\frac{C_{L}}{C_{D}}\right)\ln\left(\frac{W_{1}}{W_{2}}\right)}$$
**Maximum range is achieved at minimum drag speed** for propellor-driven aircraft.
### Comparing the Range of Jets and Propellor Driven Aircraft
For a Jet:
![[Screenshot 2024-03-27 134755.png|center]]
For a Propellor Driven Aircraft:
![[Pasted image 20240327135009.png|center]]
Note that the max range for a prop is governed by the same ratio as the max endurance for a jet aircraft, showing that the max range of a propellor aircraft will always be lower than that of a jet (given that they are the same in all other aspects).

