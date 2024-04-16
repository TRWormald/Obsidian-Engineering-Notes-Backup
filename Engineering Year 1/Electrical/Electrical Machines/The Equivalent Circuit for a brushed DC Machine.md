We have the following circuit:
![[Screenshot 2024-03-26 125353.png|center|450]]
We have the input voltage $V_{a}$ across the motor terminals, this voltage results in a current, $i_{a}$ in the rotor that flows through electric coils that have:
- Rotor Resistance, $R_{a}$
- Rotor Self Inductance, $L_{a}$
(**Note that there is positive rotation when the arm is moving anticlockwise**)
\
Lets also remind ourselves that $k_{e}$ is the electro-mechanical constant and that it is equal to:
$$\boxed{k_{e}=2\cdot (B\cdot i\cdot l)\cdot r\cdot M\cdot N}$$
Where $B$ is the stator's magnetic field strength, $i$ is the current, $l$ is the active length, $r$ is the radius of the windings, $M$ is the number of coils, and $N$ is the number of turns per coil.
\
The current results in a torque on the rotor $\tau_{EM}$ that causes an angular acceleration.
The rotating coil on the rotor results in an EMF $\varepsilon$, that opposes the source voltage/input voltage.
\
Based on the circuit we can see that:
$$V_{a}=i_{a}R_{a}+L_{a} \frac{di_{a}}{dt}+\varepsilon$$
If we consider what this means - the source voltage is divided over the resistance caused by the windings, the inductance caused by the windings and the EMF opposing it.
If we consider the above relationship in the steady-state (i.e. when $\frac{d}{dt}$ terms are zero):
$$\boxed{V_{a}= i_{a}R_{a}+\varepsilon}$$
Which can be rewritten as:
$$V_{a}-\varepsilon=i_{a}R_{a}$$
Using this equation we can determine whether we are motoring (using the input voltage to generate torque), or generating (creating an EMF using torque):
\
We are **motoring** if the EMF is in the opposite direction to the current flow - this happens when $\varepsilon<V_{a}$
We are **generating** if the current flow is in the same direction as the EMF - this happens when $\varepsilon>V_{a}$
Hence there are four combinations of EMF and current direction:
![[Pasted image 20240326131019.png|center]]
###  Torque-Speed Envelope
Electrical motors provide maximum torque when not rotating, and maximum speed when they generate no torque. This can be seen in the following equations derived below:
$$\tau_{EM}=k_{e}i_{a},~~~~~~\varepsilon=k_{e}\omega_{r}$$
Substituting these into the equation from the equivalent circuit results in:
$$V_{a}=\frac{\tau_{EM}R_{a}}{k_{e}}+k_{e}\omega_{r}$$
Which we can then rearrange to solve for the torque and the angular velocity:
$$\tau_{EM}=\frac{k_{e}V_{a}}{R_{a}}- \frac{k_{e}^{2}\omega_{r}}{R_{a}},~~~~~~\omega_{r}= \frac{V_{a}}{k_{e}}- \frac{\tau_{EM}R_{a}}{k^{2}_{e}}$$
The latter halves of both of these equations only reduce the torque/angular velocity, so we want to minimise them, the only way we can do this is by setting the angular velocity/torque respectively to zero.
So:
$$\tau_{EM_{max}}=\frac{k_{e}V_{a}}{R_{a}}~~~~~ \text{When }\omega_{r}=0 $$
$$\omega_{r_{max}}=\frac{V_{a}}{R_{a}}~~~~~~\text{When } \tau_{EM}=0$$
We call $\tau_{EM_{max}}$ the stall torque $\tau_{stall}$, and $\omega_{r_{max}}$ the no load speed $\omega_{0}$.
### The Impact of the Mechanical Structure of the Rotor on the Machine
If we consider a solid cylinder with length $l$, radius $r$, density $\rho$ and mass $M$ we can calculate the Mass moment of inertia:
$$J_{xx}=\frac{1}{2}Mr^{2}=\frac{1}{2}\times\rho\times\pi r^{2}\times l \times r^{2}=\frac{1}{2}\rho\pi l r^{4}$$
For a rotating cylinder:
$$\dot{\omega_{r}}=\frac{\tau_{EM}}{J_{xx}}=\frac{\tau_{iner}}{J_{xx}}$$
So systems that need to accelerate quickly should be long and have a low radius.
However if we need to maintain constant speeds in face of torque ripple you should have a large radius and short length.
![[Pasted image 20240326153812.png]]
![[Pasted image 20240326153831.png]]
![[Pasted image 20240326153844.png]]