### The Units

| Basic Unit  | SI  | Imperial | Derived Units  | SI   | Imperial |
| ----------- | --- | -------- | -------------- | ---- | -------- |
| Mass        | kg  | slug     | Force          | N/kN | lbf      |
| Length      | m   | ft       | Pressure       | kPa  | psi      |
| Time        | s   | s        | Work or Energy | kJ   | ft lb    |
| Temperature | C/K | F/R      | Power          | kW   | hp       |
### Symbols
Mass Flow $\dot{m}$ (kg/s)
Thrust/Force $F$ (kN)
Absolute Velocity $C$ (m/s)
Relative Velocity $V$ (m/s)
Mach Number $M$
Total Temperature $T_{0}$ (C or K)
Static Temperature $T$ (C or K)
Total Pressure $P_{0}$ (kPa / bar)
Static Pressure $P$ (kPa / bar)
Work / Energy $W$ (kJ)
Power $P_{ow}$ (kW)
### Subscripts/Superscripts
$a$ - ambient
$'$ - ideal
$N$ - at nozzle throat
$N^{*}$ - static conditions @ nozzle throat
$c$ - bypass flow
$h$ - LP turbine exit flow
$j$ - mixed flow at jet exit

### Altitude vs Mach Number
![[Pasted image 20260119213441.png|centre]]
### Propulsion System Classification
![[Pasted image 20260119213516.png|centre]]
### Choice of Propulsion System
Why do we choose specific systems? We design for specific fuel consumption (i.e. fuel flow per unit thrust):
![[Pasted image 20260119213612.png|centre]]
### Thermodynamics?
Thermodynamics is important to the study of Gas turbines as it is the "interrelationship and the conversion of different forms of energy". And a gas turbine is fundamentally an energy converter (changing primarily chemical into thermal, and then kinetic energy).
### The Brayton Cycle for a Gas Turbine
![[Screenshot 2024-02-25 120154.png]]
The Brayton cycle is a simple thermodynamic cycle where energy is constantly generated. It consists of four stages:
- Isentropic compression (1-2)
- Isobaric heat addition $Q_{in}$ (2-3)
- Isentropic expansion (3-4)
- Isobaric heat rejection $Q_{out}$ (4-1)
The efficiency can be characterised as:
$$\eta=1-\left(\frac{1}{ p_{2}/p_{1}}\right)^{\gamma-1/\gamma}$$
### The Turbojet Cycle
This is a modification of the Brayton Cycle where a diffuser and nozzle are included at either end to generate thrust:
![[Screenshot 2024-03-01 131740.png]]
The heat exchanger between the compressor and the nozzle models the combustion chamber.

### The International Standard Atmosphere
A standard atmosphere is used so all aircraft and engine performance data can be compared on the same basis.
The ISA represents the average atmospheric conditions in North America and Europe and is based on the assumption that:
- Air is a perfect gas
- Air is dry
- Gravitational acceleration does not vary with altitude
- Hydrostatic equilibrium exists

It has the following sea level values:

| Variable                     | Symbol | Value                          |
| ---------------------------- | ------ | ------------------------------ |
| Pressure                     | $p$    | $101.325 kPa$                  |
| Temperature                  | $T$    | $15 ^o C~~ (288.15 K$)         |
| Density                      | $\rho$ | $1.2250 kg/m^3$                |
| Speed of Sound               | $a$    | $340.29 m/s$                   |
| Dynamic Viscosity            | $\mu$  | $1.7894\times 10^{-5} kg/(ms)$ |
| Gravitational Acceleration   | $g$    | $9.80665~ m/s^2$               |
| Specific Gas Constant of Air | $R$    | $287.05 J/(kg\cdot K)$         |
> It is convenient to assume that acceleration due to gravity is constant with position and altitude - this is due to the very small variance over massive distances.

#### Altitudes
There are a number of different altitudes that we can consider:
- Geometric height $Z$ - The actual height above mean-sea-level
- Geopotential height $H$ - The height in a uniform gravitational field ($g$ constant with altitude) which gives the same potential energy as exists in the actual, variable gravitational field:
$$h=\frac{R_{earth} Z}{R_{earth}+Z}$$
- Pressure height - Aircraft normally fly at altitudes defined by barometric means. The pressure height in any atmosphere is the geopotential height in an the standard atmosphere giving the same pressure.
### Hydrostatic Equilibrium of an Element of Air
If we consider the forces acting on an element of air in the atmosphere we obtain the following diagram:
![[Pasted image 20260120110806.png|centre|250]]
Which we can represent using an equation:
$$\frac{dP}{dh}=-\rho(h)g=-\frac{P}{RT(h)}g$$
As a result we need a model for the temperature variation with altitude to close the problem.
The international standard atmosphere is based on an idealised mean-annual, steady state model assuming a period of moderate solar activity and at a latitude of 45 degrees North.

In the troposphere $T=T_{SL}-Lh$ where $L=0.0065 \frac{K}{m}$ which is the "Lapse Rate". So we can calculate the temperature at any altitude up to ~10km using the sea level temperature, a constant, and the altitude. (In the Stratosphere the temperature is approximately constant $T=T_{10}$ i.e. it is the same as the temperature at 10km)

So we have:
$$\frac{dP}{dh}=-\rho(h)g=-\frac{P}{RT(h)}g$$
$$T=T_{SL}-Lh$$
Which we can combine to obtain:
$$\frac{dP}{dh}=-\frac{P}{R(T_{SL}-Lh)}g$$
$$\int_{P_{SL}}^{P} \frac{dP}{P}=-\frac{g}{R}\int_{0}^{h}\frac{dh}{T_{SL}-Lh}$$
And finally we can obtain the ratio of the pressures at a given altitude above sea level:
$$\frac{P}{{P_{SL}}}=\left(1-\frac{Lh}{T_{SL}}\right)^{-\frac{g}{RL}}$$

![[Pasted image 20260120112151.png|centre|500]]


