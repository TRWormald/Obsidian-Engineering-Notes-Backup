**An inductor** is a physical component whose principal behaviour is represented by inductance.
\
**Inductance** is a property/behaviour that can be present in a circuit and that links magnetic fields to current flowing in a component.
\
**Induction** is a physical effect where an electrically conductive component present in  magnetic fields that are changing with respect to each other results in a voltage induced in that component.
\
We know that the impedance associated with an inductor is:
$$Z_L=j\cdot \omega L$$
Where $Z_L$ is the impedance, $\omega$ is the angular velocity, and $L$ is the inductance.
Inductance results in the current **lagging** voltage when excited by an AC power source.
Inductance relates to a structure's ability to store energy as a magnetic field.

### Current Carrying Wire
Any wire that has a current passing through it has a magnetic field around it. The magnetic field is represented by closed flux lines perpendicular to the current flowing in the wire.
\
The magnetic field at a point in space has a magnitude $B$ and a direction - this is often referred to as flux density.
The units of the magnetic field (or flux density) are:
- Tesla $[T]$
- Webers/$m^2$ $[\frac{Wb}{m^{2}}]$ 
\
Magnetic flux $\Phi$ is the surface integral of flux density normal to an area:
$$\Phi = \iint B\cdot dS$$
\
Coils of current carrying wire are called solenoids:
![[Pasted image 20240312151319.png|center|400]]
Inductance is defined from an electrical perspective as:
"*The ratio of magnetic flux linkage from a coil to the current passing through that same coil.*"
So:
$$L=N \frac{\Phi}{I} ~~~[H]$$
Where inductance $L$ is measured in Henrys $[H]$, $\Phi$ is the magnetic flux, $N$ is the number of coils, and $I$ is the current through the wire.
Therefore:
$$L=\frac{N^2\mu A}{\ell}$$Where $\mu$ is the permeability of material around the coil $[\frac{H}{m}]$, $A$ is the cross sectional area of the coil normal to the flux, and $\ell$ is the mean length of the flux path.
Note that the mean path length is the *average* length of one of the flux lines:
![[Pasted image 20240312152132.png|center|400]]
The mean path is highlighted in blue in the image above.
\
The permeability can be split into two parts:
$$\mu=\mu_0\cdot\mu_r$$
Where $\mu$ is the permeability, $\mu_0$ is the permeability of free space ($4\pi\times 10^{-7}$), and $\mu_r$ is the relative permeability of the material.

### The Electrical Behaviour of Inductors
We have so far looked at the impedance associated with an inductor - this results from its fundamental behaviour.
Consider the following:
![[Screenshot 2024-03-14 101048.png|center|150]]
If we look at the definition of inductance and rearrange it:
$$L=\frac{N\Phi}{i_{L}},~~~~~~\Phi=\frac{L\cdot i_{L}}{N}$$
And as voltage is the rate of change of flux linkage with respect to time ($-\epsilon =v_L$):
$$\epsilon = -N \frac{d\Phi}{dt},~~~~~~v_{L}=N\frac{ d\Phi}{dt} $$
So if we apply this definition of EMF to the inductance equation:
$$v_{L}=\frac{d}{dt}(Li_{L})=\left(L \frac{di_{L}}{dt}+i_{L} \frac{dL}{dt}\right)$$
Normally the inductance is constant with respect to time hence the voltage drop across and inductance is related to the rate of change of current through it:
$$v_{L}=L\frac{di_{L}}{dt}$$
This is a differential equation with respect to time. It tells us how the current and voltage vary as a function of time, and it it responsible for what occurs during the transient period (the dynamic response). Once we have reached a steady state - in an AC circuit we will have a 90 degree chase difference (current lags voltage) whilst in a DC circuit an inductor looks like a short circuit.
#### Energy stored in an inductor
We can calculate the energy stored in an inductor to be:
$$E=\frac{1}{2}L\cdot i_{L}^{2}$$
#### Combining Inductors
##### Inductors in Series
If we connect a number of inductors in series then they will share the same current with voltage being split between them, this results in the total inductance being equal to the sum of the individual inductances:
$$L_{total}=\sum\limits^N_{i=1}L_i$$
##### Inductors in Parallel
If we connect a number of inductances in parallel then they will share the same voltage with current being split between them, this results in the total inductance being equal to the following:
$$L_{total}=\left(\sum\limits^{N}_{i=1}\left(\frac{1}{L_{i}}\right)\right)^{-1}$$
