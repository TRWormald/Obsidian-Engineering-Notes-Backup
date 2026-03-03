### Introduction to Turbomachinery
In turbomachinery the **compressor** raises the pressure of the air before combustion, whilst the **turbine** extracts work from the hot high pressure combustion products to drive the compressor.
![[Pasted image 20260303110127.png|centre]]
In the compressor, each "stage" consists of a row of blades followed by a row of stator blades. These are often preceded by an inlet guide vane,

In the turbine, each stage consists of a nozzle guide vanes which direct the gas onto the rotor blade.
#### A Comparison of Compressor and Turbine Blades
![[Pasted image 20260303110305.png|671]]
Note that rotor blades spin, and stator blades are static and mounted to the housing.
### Isentropic & Polytropic Efficiency
#### Polytropic (Small Stage) Efficiency
The isentropic efficiency of an elemental stage, such that it is constant throughout the whole process:
$$\text{For Compression:}~~~\eta_{pol}=\frac{dT_{o}'}{dT_{o}}=\text{Constant}$$
$$\text{For an Isentropic Process:}~~~~\frac{T_{o}}{p_{o}^{\gamma-1/\gamma}}=\text{Constant}$$
$$\text{The Differential form being:}~~~~\frac{dT_{o}'}{T_{o}}=\frac{\gamma}{\gamma-1}\frac{dp_{o}}{p_{o}}$$
If we substitute for $dT_{o}'$ we obtain:
$$\eta_{pol}\frac{dT_{o}}{T_{o}}=\frac{\gamma}{\gamma-1}\frac{dp_{o}}{p_{o}}$$
Which we can integrate from 1 to 2 to obtain:
$$\frac{T_{O2}}{T_{O1}}=\left(\frac{p_{O2}}{p_{01}}\right)^\frac{\gamma-1}{\gamma\eta_{pol}}$$
This is representative of aerodynamic quality and "technology level".
#### Isentropic Efficiency
$$\eta_{isen}=\frac{T_{O2}'-T_{O1}}{T_{O2}-T_{O1}}$$
The Overall Efficiency of compressors of identical aerodynamic quality reduces as overall pressure ratio increases. In a multi-stage axial compressor of equal aerodynamic quality, i.e. a similar $\Delta T_{O}$ per stage, the pressure ratio per stage decreases.
![[Pasted image 20260303111340.png|centre]]
#### Using Polytropic Efficiency
The polytropic efficiency removes the penalty from higher pressure ratios and allows compressors of differing aerodynamic quality and pressure ratio to be compared.
![[Pasted image 20260303111622.png]]
### The Euler Work Equation
This is applicable to both compressors and turbines.
Consider the rotor stage below:
![[Pasted image 20260303111814.png|246]]
If we consider an elemental mass $\delta\dot{m}$ entering the rotor in steady flow conditions. In time $\delta t$ an equal mass must leave.

The moment of momentum of the entering fluid at $r_{1}$ about the axis of rotation is:
$$M_{1}=\delta \dot{{m}}\cdot r_{1}\cdot C_{w1}$$
The corresponding moment of momentum of the leaving fluid at $r_2$:
$$M_{2}=\delta\dot{m}\cdot r_{2}\cdot C_{w2}$$
Since torque is the rate of change of the moment of momentum then:
$$T=\dot{m}(r_{2}\cdot C_{w2}-r_{2}\cdot C_{w1})$$
Where $C$ is the velocity of the fluid.

**Power** is then given by the Euler Equation:
$$P_{ow}=T\cdot \omega~~~~\&~~~~U=r\cdot\omega$$
So then:
$$P_{ow}=T\cdot\omega=\dot{m}(U_{2}\cdot C_{w2}-U_{1}\cdot C_{w1})$$
Where $U_1$ and $U_2$ are the speed of the blade row at inlet & outlet.

The work input per unit mass is equal to the change in stagnation enthalpy per unit mass:
$$\Delta h_{0}=C_{p}(T_{02}-T_{01})=U_{2}\cdot C_{w2}-U_{1}\cdot C_{w1}$$
In most cases we can assume that $r_{1}=r_{2}$ and hence $U_{1}=U_{2}=U$:
$$\Delta h_{0}=U(Cw_{2}-Cw_{1})$$
### Typical Axial Compressor Layout
![[Pasted image 20260303112455.png]]
### Pressure & Velocity Changes Through an Axial Compressor
![[Pasted image 20260303112603.png]]
### T-s Diagram for a Single Stage
![[Pasted image 20260303112710.png|centre]]
### Velocity Triangles
**This is the most important plot to understand how a compressor works**
![[Pasted image 20260303113309.png]]
![[Pasted image 20260303113329.png]]
#### Simple Blading Analysis
From the velocity triangles:
$$U/C_{a}=(\tan\beta_{1}+\tan\alpha_{1})=(\tan\beta_{2}+\tan\alpha_{2})$$
By consideration of Angular Momentum (see the Euler Equation) it can be shown that:
$$P_{ow}=\dot{m}\cdot U\cdot (C_{w2}-C_{w1})$$
In terms of Axial Velocity and Air Angles:
$$P_{ow}=\dot{m} \cdot U \cdot C_{a}(\tan\alpha_{2}-\tan\alpha_1)$$
Or in terms of $\beta_1$:
$$P_{ow}=\dot{m} \cdot U \cdot C_{a}(\tan\beta_{1}-\tan\beta_{2}) $$
The input energy will be absorbed in raising pressure and overcoming frictional losses. Regardless of efficiency, power input must equal the raise in stagnation temperature of the stage.
![[Pasted image 20260303114259.png|centre]]
### Factors Effecting Stage Pressure Ratio
![[Pasted image 20260303114322.png|centre]]
### Compressor Reaction
The Reaction, R, is defined as:
$$R=\frac{\text{Static Enthalpy Rise in Rotor}}{\text{Static Enthalpy Rise in Stage}}=\frac{\Delta h_{rotor}}{\Delta h_{stage}}=\frac{\Delta T_{rotor}}{\Delta T_{stage}}$$
Because at $$\Delta T_{stage}=\Delta T_{0}= T_{03}-T_{01}=T_{02}-T_{01}$$
If we assume $C1=C3$, so:
$$R=\frac{\Delta T_{rotor}}{\Delta T_{0}}$$
And, from previously:
$$\Delta T_{0}=\frac{U\cdot C_a}{C_{p}}(\tan\beta_{1}-\tan\beta_{2})$$
$$\Delta T_{rotor}=\Delta T_{0}-\frac{1}{2C_{p}}(C_{2}^{2}-C_{1}^{2})$$
With reference to the velocity triangles and use of trig:
$$R=\frac{C_{a}}{2U}(\tan\beta_{1}+\tan\beta_{2})$$
**If the reaction is >50% then the majority of the static pressure rise is being done in the rotor**.
**If the reaction <50% then the majority of the static pressure rise is being done in the stator.**

### Blade Spacing and Blockage
![[Pasted image 20260303115101.png|centre]]
### Dimensional Relationships
![[Pasted image 20260303115304.png|centre]]
