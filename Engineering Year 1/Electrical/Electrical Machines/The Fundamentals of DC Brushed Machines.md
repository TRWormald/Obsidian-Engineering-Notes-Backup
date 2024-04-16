We know that we can use Fleming's left hand rule to determine the direction of the [[Lorentz Force]], and that we can calculate the force using the equation:
$$F=Bil\sin\theta$$
Where $B$ is the magnetic field strength, $i$ is the current, $l$ is the length of wire in the magnetic field, and $\theta$ is the angle between the direction of the current and the magnetic field:
![[20.1-Force-on-conductor-1.avif|center]]
\
If we have a bundle of $N$ wires carrying $i$ amps then:
$$F=NBil\sin\theta=k_ei\sin\theta,~~~~~~\text{where } k_{e}=BlN $$
We also know that we can calculate the EMF induced in a wire moving through a magnetic field using the equation:
$$\epsilon=B\cdot l\cdot v$$
And can use [[Fleming's Left and Right Hand Rules|Fleming's Right Hand Rule]] rule to determine the direction of the induced current/voltage.
If we apply this to a bundle of $N$ wires moving together at $v$ m/s:
$$\epsilon=BlvN\sin\theta=k_{e}v\sin\theta,~~~~~~\text{where }k_{e}=BlN$$
Where $\theta$ is the angle between the wires and the magnetic field.
\
**These effects are not isolated, and frequently we get both at the same time.**
\
1) We apply a voltage to wires in a magnetic field, resulting in a current flowing in them
2) The wires in the magnetic field now experience a force, which results in an acceleration and hence the wires begin to move.
3) This results in an EMF in a direction that opposes the source voltage, and hence the current that caused the movement (back EMF)
4) This reduces the available voltage ($V_S-\epsilon$) for current so the current reduces and the force reduces
5) This reduces the acceleration of the wire
6) As the wire is still accelerating an EMF is still growing
7) At some point the source voltage minus the EMF from the moving wires results in a current that is just enough to overcome the friction force on the wires and the system settles into a steady state.
\
#### Types of Brushed Machines
There are two main types of brushed machines: Wound Field Machines (which use electromagnets for the stator) and Permanent Magnet Machines (which as you would imagine use permanent magnets as the stator).
The stator is what provides the magnetic field which work is done against to generate energy.
![[Screenshot 2024-03-26 115016.png|center]]
**For most questions we will be considering permanent magnet machines.**
#### Electromagnetic Torque 
In the following case (where the + indicates current into the page and the - indicates current out of the page), if we apply the left hand rule we can calculate that the resulting electromagnetic torque will be equal to:
$$\tau_{EM}=2\cdot F\cdot r$$
![[Pasted image 20240326115347.png|center]]
![[Pasted image 20240326115424.png|center|250]]
However this presents a problem if the coil continues to rotate then the torque will result in an oscillating motion, and as a result we have to invert the current direction. This is done using a commutator.
#### Increasing the number of Coils
As we increase the number of coils the total torque increases, but its AC component decreases and its DC component increases.
If we increase the number of coils the torque will increase:
$$\begin{align*}
\tau_{EM}&= 2\cdot2\cdot F\cdot r\\
&= 2\cdot 2\cdot B\cdot i \cdot l\cdot r
\end{align*}$$
The above equation is for two coils with a single loop of wire each, the equation can be generalised:
$$\tau_{EM}=2\cdot (B\cdot i\cdot l)\cdot r\cdot M\cdot N$$
Where $M$ is the number of coils $N$ is the number of loops per coil, $r$ is the radius of the coil, $l$ is the active length, $i$ is the current, and $B$ is the magnetic field strength provided by the stator.
\
From the equation above we can calculate the EMF that will be produced:
$$\epsilon_{EM}=2\cdot (B\cdot i\cdot l)\cdot r\cdot M\cdot N\cdot \omega_{r}$$
Where the components that relate the angular velocity and the EMF are called the electro-mechanical constant ($k_{e}$)

#### Loss Mechanisms in Electrical Machines
Electromechanical system losses always relate to useful mechanical or electrical energy being converted into unwanted heat energy.
##### Mechanical Losses
There are two main types of mechanical losses:
1) Frictional Losses (Brush Friction/Bearing Friction) - these are the resistances to rotational motion offered by contact between two solid moving parts. They are proportional to **the square of the angular velocity**
2) Windage - this is the resistance to rotational motion offered by air on any moving part. They are proportional to **the cube of the angular velocity**
\
Mechanical losses typically account for 15% of the total losses.
##### Electrical Losses
There are two main types of electrical losses:
1) Electrical Losses - These are due to the resistance to current flow in all current carrying components, these losses are typically greater than 50% of total losses
2) Magnetic Losses - These are caused by moving components constantly working against the magnetic field. They account for around 30% of total losses.
#### Efficiency of Electric Machines
If the mechanical input power is $W_{mech}$ and we get an electrical output power of $W_{elec}$ and we assume our system isn't 100% efficient:
$$W_{mech}-W_{elec}=L_{elec}+L_{mech}+L_{mag}$$
So to find the efficiency we can use the equation:
$$\eta=\frac{W_{elec}}{W_{mech}}=\frac{W_{mech}-L_{mech}-L_{elec}-L_{mag}}{W_{mech}}$$
(For mechanical to electrical systems)
And:
$$\eta=\frac{W_{mech}}{W_{elec}}=\frac{W_{mech}-L_{mech}-L_{elec}-L_{mag}}{W_{elec}}$$
(For electrical to mechanical systems)