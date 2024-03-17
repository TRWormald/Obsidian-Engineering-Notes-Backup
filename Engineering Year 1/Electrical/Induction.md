### Electromotive Force
EMF is a potential difference generated along a length of wire by a non-electrical source. In other words it is the amount of work done to charge carriers per unit charge.
It has units of volts $[V]$ or joules per coulomb $[J/C]$
\
It is not unique to mechanical to electrical energy conversion - batteries generate EMF in a closed circuit via a chemical to electrical energy conversion.
\
In electromagnetism the EMF is the potential difference generated along a length of wire by a permanent magnetic field.
### Electromagnetic Induction
Induction uses a permanent magnetic field to generate EMF around a closed loop.
Closed loops of wire can have any number ($N$) of complete loops. The EMF $[V]$ is measured across the ends of the loop of wire. However the magnetic field is not enough to generate an EMF alone, mechanical work is essential. This is because EMF is only generated when there is a change in magnetic flux.
\
The motion can be linear or rotational, magnetic flux $\Phi$ imposed on the wire loop changes as the magnet moves - this generated an EMF due to the flow of electrons around the circuit. If we reverse the direction of the motion we reverse the EMF.
### Faraday's Law of Induction
Faraday noted that the magnitude of current flow induced is proportional to the number of coils, and the relative velocity of the magnet.
His ideas were then refined by Lenz who formulated them into an equation:
$$I_{coil}=-\frac{N}{R_{coil}} \frac{d\Phi}{dt}$$
Where:
$I_{coil}$ is the induced current $[A]$
$N$ is the number of turns in the coil
$R_{coil}$ is the coil resistance $[\Omega]$ 
$\Phi$ is the magnetic flux $[Wb]$
$t$ is the time $[s]$
\
However what Lenz noticed was that the current induced is directed to oppose the change in magnetic flux.
In other words it is trying to generate a magnetic field in the opposite direction to keep the magnet where it is, which work is then done against to generate the induced current/power.
**Note that this is not a perfect explanation but it succinctly explains why you are not generating power from nothing.**
\
We can also use [[Ohm's Law]] to calculate the EMF generated:
$$\begin{align*}
\epsilon_{coil}&= I_{coil}\cdot R_{coil}\\
&= -N \frac{d\Phi}{dt}\\
\end{align*}$$
Where $\epsilon_{coil}$ is the EMF generated in volts $[V]$
### Transformers
Transformers leverage electromagnetic induction to step up or step down the voltage of an alternating current.
A transformer consists of a laminated metal core with two coils of wire wound around its sides:
![[Pasted image 20240312160459.png|center|400]]
The alternating current in the primary coil induces an alternating magnetic flux around the core. The alternating magnetic flux induces an alternating current, at a different voltage in the secondary coil. Note that the frequency of the current is unchanged.
This results in the following equation linking the ratios of turns, voltage and current.
$$\frac{n_1}{n_{2}}=\frac{V_1}{V_{2}}=\frac{I_2}{I_{1}}=Turns~Ratio$$
Where:
$n_1$ is the number of turns on the primary coil, whilst $n_2$ is the number of turns on the secondary coil.
$V_1$ is the voltage across the primary coil, and $V_2$ is the voltage across the secondary coil.
$I_1$ is the current in the primary coil, whilst $I_2$ is the current in the secondary coil.