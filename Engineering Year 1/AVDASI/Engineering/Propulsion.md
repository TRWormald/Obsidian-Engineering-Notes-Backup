What to burn? Lots of things burn, however they have differing energy density characteristics:
![[Pasted image 20240303162451.png|center]]
In aircraft we typically use hydrocarbons (seen in the red circle) as they have good (but not excellent) energy per unit volume and mass.
\
Issues with burning fuel:
We can burn fuel at atmospheric pressure - however this doesn't guarantee ideal combustion (as there may not be enough oxygen) resulting in inefficiency and by-product production.
We can increase the amount of air/oxygen available to the combustion process by compressing it (as this increases the air density)
Note that liquid rocket engines have no requirement for compression because they use oxidiser.

#### Specific Impulse
Specific impulse is a good measure of how efficient a fuel is. It is the amount of thrust produced per unit weight of fuel burn:
$$I_{sp} = \frac{Tt}{mg}=\frac{Thrust}{Weight rate of fuel burn}=\frac{T}{\dot{m}g}[s]$$
We can see how $I_{sp}$ changes with speed on the graph below:
![[Pasted image 20240303163502.png|center]]
But why does this happen?
If we assume that the total efficiency is one:
$$P=Tu_o$$
Where $P$ is the power of the engine, $T$ is the thrust produced, and $u_o$ is the speed of the aircraft.
By substituting this into the $I_{sp}$ equation:
$$I_{sp}=\frac{\frac{P}{u_o}}{\dot{m}g}=\frac{h}{u_o g}$$
Where $h$ is the amount of energy released by combustion of 1kg of fuel.
So we can see that specific impulse is inversely proportional to the speed of the aircraft.
#### Air-Breathing Propulsive Efficiencies
$$\eta_{total}=\eta_{thermal}\eta_{propulsive}=\frac{KE}{fuel~ power}\frac{propulsive ~power}{KE}=\frac{Tu_0}{\dot{m}_fh}$$
We can rewrite the propulsive efficiency as:
$$\eta_{propulsive}=\frac{2u_0}{u_e+u_o}=\frac{2}{1+\frac{u_e}{u_o}}$$
Matching the exhaust velocity to flight speed gives good propulsive efficiency - however we cannot match them exactly as then thrust would be zero.
![[Pasted image 20240303165021.png|center]]
#### Fuel Usage
If we consider the power produced by an engine:
$$P=\frac{1}{2}\rho A u_o(u_e^2-u_o^2)=\frac{1}{2}\rho A u_o (u_e+u_o)(u_e-u_o)=\frac{1}{2}T(u_e+u_o)$$
For an engine with high propulsive efficiency ($u_e=u_o$) then power is driven by the propulsive power ($P=Tu_o$).
If the propulsive efficiency is low ($u_e>>u_o$) then power is only dependant on thrust, so $P\approx\frac{Tu_e}{2}$ 
\
Neither case is 100% accurate, some engines operate more like one or the other, for example turbojets show mostly thrust specific fuel use whilst turboprops (or any other kind of propeller propulsion) show power specific fuel use.

#### Types of Gas Turbines
The main types of gas turbines are:
- Turbojets
- Turbofans
- Turboprops
- Turboshaft
- Power Generation
- Ships
- Tanks, Trains, Cars, Motorbikes
\
The Jet Engines:
##### Turboshaft/Turboprop
![[Pasted image 20240303170203.png|center|500]]
##### Turbojet
Axial Turbojet
![[Pasted image 20240303170224.png|center|500]]
Radial Turbojet
![[Pasted image 20240303170427.png|center|500]]
##### Turbofan
![[Pasted image 20240303170323.png|center|500]]
