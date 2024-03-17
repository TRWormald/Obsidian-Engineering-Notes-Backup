### Basics
We've so far looked at the impedance associated with a capacitor:
$$Z_C=\frac{1}{j\omega\cdot C}$$
Where $Z_C$ is the impedance of the capacitor, $\omega$ is the angular velocity, and $C$ is the capacitance.
And we know how it results in the current **leading** the voltage when excited by an AC power source.
#### Structure
Capacitors consist of two parallel metal plates with a dielectric in between them, when there is current electrons are deposited on one plate and removed from the other resulting in a difference in electrical charge and hence a electrical field is generated (this is how energy is stored).
#### Equation for Capacitance
*The capacitance is the ratio of charge on one plate of a capacitor to voltage difference between the two plates.*
So:
$$C=\frac{q}{V}$$
Where $q$ is the charge on the plate and $V$ is the potential difference between the plates.
Capacitance $C$ is measured in Farads $[F]$
#### How can we change Capacitance?
The capacitance of a capacitor can be changed by modifying:
- The overlapping plate area
- The distance between the plates
- The permittivity of the dielectric
This results in the equation:
$$C=\frac{\epsilon\cdot A}{d}=\frac{\epsilon\cdot w\cdot h}{d}$$
So capacitance is directly proportional to overlapping area and permittivity but inversely proportional to the distance between the plates.
**Permittivity**
We can calculate permittivity by comparing the permittivity of a material to the permittivity of free space. As such:
$$\epsilon = \epsilon_0 \cdot \epsilon_r$$
Where:
$\epsilon_0=8.854\times 10^{-12}$ which is the permittivity of free space
$\epsilon_r$ is the relative permittivity of a material.

### Electrical Behaviour
#### Fundamental Behaviour
If we look at the defining equation and re-arrange it:
$$q=C\cdot V$$
And knowing that current is the rate of change of charge with respect to time:
$$i=\frac{dq}{dt} \Rightarrow q=\int_0^t i \cdot dt$$
So:
$$q=\int_0^t i \cdot dt = C\cdot v_C$$
$$i_c=\frac{d}{dt}(C\cdot v_C)=C\frac{dv_c}{dt}+v_c\frac{dC}{dt}$$
Hence we have a differential equation with respect to time, which tells us how the current and voltage vary as a function of time. This is what is responsible for what occurs during the transient period (the dynamic response).
![[Pasted image 20240305103051.png|center]]
This is due to the fact that a capacitor's voltage cannot change instantly.
#### Energy Stored in a Capacitor
The power delivered by the current source to the capacitor is:
$$P_C = v_C\cdot I_C = v_C\cdot C \frac{dv_c}{dt}$$
With power being defined by:
$$W_C=\int_0^t P\cdot dt$$
So:
$$W_C=\int_0^tv_c\cdot C\cdot \frac{dv_C}{dt}\cdot dt$$

$$W_C=C\int_{v_C(0)}^{v_C(t)} v_c \cdot dv_C$$
$$W_C=\left[\frac{v_C^2}{2}\right]_{v_C(0)}^{v_C(t)}$$
So the energy stored in a capacitor that is being charged to $v_C$ volts from 0 volts is:
$$W_C=\frac{1}{2}C\cdot v_C^2$$
Or:
$$W_C=\frac{1}{2C}q^2$$
### Combining Capacitors in Parallel and Series
#### Combining capacitors in Parallel
Capacitors in parallel share the same voltage with current being split between them.
To combine you simply add the capacitances like you would for resistors in series.
#### Combining capacitors in Series
Capacitors in series will have the same current but the voltage will be split between them.
To combine you take the reciprocal of the sum of the reciprocals of the capacitances (like you would with resistors in parallel)
