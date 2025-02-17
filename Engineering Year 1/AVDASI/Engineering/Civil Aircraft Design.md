When designing any aircraft we need to consider the drivers for that design. In the civil sector those drivers are typically profitability, low maintenance costs, amount of crew training required, number of crew, etc.
These influence design choices - there are many of them but some of the most important are:
- Wing loading - depends on mass and wing area
- Cruise speed (driven by economics) and cruise lift coefficient
- Landing and low speed behaviours (landing and take off distance are linked to maximum lift coefficient)
- Speed
\
#### Why Transonic
**Turbofan** aircraft tend to be designed to maximise range, which depends on $speed \times L/D$ (from the Breguet range equation). 
$$R=\frac{V}{sfc}\frac{L}{D}log\left(\frac{W_o+W_f}{W_o}\right)$$
Where $V$ is the speed of the aircraft, $sfc$ is the specific fuel consumption, $L/D$ is the lift to drag ratio, $W_o$ is the mass of the aircraft, whilst $W_f$ is the weight of the fuel.
If we factor out the speed of sound, and only look at the aerodynamic part we get:
$$\frac{ML}{D}$$
Where $M$ is the Mach number.
If we plot this against Mach number we get a graph which peaks at transonic speeds.
\
#### Supersonics
The best L/D is roughly given by:
$$\frac{L}{D}=4(M+3)/M$$
So ML/D continues to grow with M, hence it is preferable for an aircraft to operate at its highest feasible Mach number, which can be determined by various factors like thrust or material constraints.
#### Low Speed Maximum Lift
We need to approach landing at low speeds to reduce the length of the runway required to land safely, this is also true of take-off.
In most aircraft the maximum coefficient of lift ($C_L$) is between two and three.
#### Wing Loading at Landing and Cruise
Wing loading is equal to the mass of the aircraft divided by its wing area. As wing loading will equal (or approximately equal) the lift generated by the aircraft (as it needs to stay in the air) we can equate them:
$$\frac{W}{S}=C_{L_{max}}\frac{1}{2}\gamma M^2p_{\infty_{land}}$$
Where $W$ is the weight of the aircraft, $S$ is the wing area, $\gamma$ is the ratio of the specific heats of air at constant pressure and volume (see the [[Isentropic Process]]), $M$ is the Mach number, and $p_{\infty_{land}}$ is the static pressure at landing conditions.
\
We can use this equation to determine the cruising altitude of an aircraft by calculating the pressure ratio:
$$\frac{p_{\infty_{cruise}}}{p_{\infty_{land}}}=\frac{\frac{W}{S}_{cruise}C_{L_{max}}M_{land^2}}{\frac{W}{S}_{land}C_{L_{cruise}}M^2_{cruise}}$$
By multiplying by $p_{\infty_{land}}$ we can then calculate the static pressure at cruise altitude and then use that to calculate the cruise altitude.
\
Note that if higher wing loading drops in cruise (i.e. through fuel burn) then cruise altitude will increase.
\
For **supersonic** aircraft not much changes (as wing loading is about the same and $C_{L_{max}}$ requirements are similar)
#### Wing, tailplane, and tail fin design
*Why are wings high aspect ratio?*
Induced drag is produced by lift, we can reduce it by increasing the aspect ratio.
*Why is the tailplane low aspect ratio?*
This is because it must be able to generate large forces, so it must have reasonable total area. Normally it only has a small lift coefficient so it produces very little induced drag.
#### Choosing Aircraft
When choosing an aircraft for a mission you want an aircraft that just meets requirements, because:
- Too much range implies excess structural weight
- Too little range implies stopovers
- Seats and frequency should match demand
- Fuel economy is traded against purchase price (it may be cheaper to buy a less expensive but more fuel hungry plane if the initial cost of the other aircraft is too high)
- Crew and maintenance commonality important in total cost
