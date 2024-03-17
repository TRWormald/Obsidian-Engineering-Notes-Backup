As aerospace engineers the atmosphere and its various zones are quite an important facet of our knowledge.
The zones are based the temperature profile and are (in increasing altitude): The Troposphere, Stratosphere, Mesosphere, Thermosphere.
The diagram below shows these:
\
![[Pasted image 20240223110454.png]]
\
Most aircraft equipped with air-breathing engines operate within the lowest two zones (at altitude less than 20km)
\
In the **troposphere** temperature decreases with altitude.
The lowest part of the **stratosphere** is Isothermal.
**Tropopause** is the separating boundary between zones.

#### The International Standard Atmosphere
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
##### ISA Values
\
ISA tables can give absolute values or the variables are often stated as ratios of sea level (SL) values:
\
Absolute temperature ratio: $\theta = \frac{T}{T_{SL}}$
\
Static pressure ratio: $\delta =\frac{p}{p_{SL}}$
\
Density ratio: $\sigma = \frac{\rho}{\rho_{SL}}$
\
If we apply [[The Ideal Gas Law]], at a given altitude:
\
$$\frac{p}{p_{Sl}}=\frac{\rho}{\rho_{SL}}\frac{T}{T_{SL}} ~~~~or~~~~ \delta=\sigma\cdot\theta$$


##### ISA Temperature
The **Troposphere** is defined as altitudes between 0 and 11 kilometres, with a linear temperature lapse rate of $-6.5~^o C/km$ 
**Tropopause** occurs at 11km, where $T=-56~^oC$ ($216.65~K$)
The lowest part of the **Stratosphere** (11-20 km) is isothermal.
\
![[Screenshot 2024-02-23 112603.png]]
##### ISA Pressure
The pressure can be determined in the following way:
![[Screenshot 2024-02-23 112908.png]]

##### ISA Density
With temperature and pressure known, we can use the equation of state to determine density:
\
![[Screenshot 2024-02-23 113020.png]]
\
We can also approximate density in the following way:
\
$$\sigma =\frac{\rho}{\rho_{SL}}\approx \frac{20-H}{20+H}$$
Where $H$ is the altitude in kilometres
##### ISA Speed of Sound
The speed of sound ($a$) is related to temperature:
\
$$a=\sqrt{\gamma R T}$$
Where $\gamma$ is the Ratio of Specific Heats for air and is equal to 1.4.
We can also calculate it in terms of the temperature ratio:
\
$$ a=a_{SL}\theta^{~0.5}$$
\
![[Pasted image 20240223113636.png|300]]
##### ISA Viscosity
Dynamic Viscosity ($\mu$) can be estimated from temperature using Sutherland's Equation:
\
$$\frac{\mu}{\mu_{SL}}=\left(\frac{T}{T_{SL}}\right)^{3/2}\cdot\frac{T_{SL}+T_S}{T+T_S}$$
\
Where $T_S$ is the Sutherland constant, $T_S = 110K$ 
Or alternatively:
\
$$\frac{\mu}{\mu_{SL}}=\frac{1.383}{\theta +0.383}\cdot\theta^{3/2}$$
\
![[Pasted image 20240223114216.png|300]]
