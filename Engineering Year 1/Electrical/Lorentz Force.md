When a charged particle moves through a magnetic field with a velocity it experiences a force. This often manifests as an interaction between a current carrying conductor and a magnet.
The Lorentz force is a force on a moving **positive** charge (the direction of the force is reversed for a negative charge).
$$\vec{F}=q(\vec{v}\times\vec{B})$$
Where $\vec{F}$ is the Lorentz force, $q$ is the charge, $\vec{v}$ is the charge velocity, and $\vec{B}$ is the external magnetic field density.
$\vec{F}$ is maximised when $\vec{v}$ and $\vec{B}$ are orthogonal, and the force is zero when they are parallel.
Applying the cross product we know that:
$$F=q(|v|\cdot|B|)sin\theta$$
Where $\theta$ is the angle between $v$ and $B$.
\
For a current carrying wire the force applied to it is:
$$F=B\cdot I\cdot l$$
Where $I$ is the current in the wire, and $l$ is the length of wire in the magnetic field.
We can use the left hand rule to determine the direction of the force:
![[Pasted image 20240322112638.png|center|500]]
Where the thumb represents the direction force, the first finger points the direction of the field, and the second finger points the direction of the current.

### Relating the Lorentz force to EMF
We know that using [[Induction#Faraday's Law of Induction|Faraday's Law]] we can calculate the EMF produced when a magnet moves within a coil of wire, and using the Lorentz force we can calculate the force on a wire from a magnetic field. Using these two facts we can calculate the EMF generated based on the velocity of a wire in a magnetic field.
![[Screenshot 2024-03-22 114915 1.png|center|500]]
In the above image there is a **potential difference** between the two rails, and there is a uniform magnetic field/flux density between them - which is into the page. There is a straight wire, length ($l$) which completes the circuit between the rails. Current ($I$) flows around the circuit due to the potential difference.
The Lorentz force ($F=B\cdot I\cdot l$) causes the straight wire to travel with velocity ($v$).
The wire moves from its initial position to a position $dx$ away in time $dt$, such that:
$$v=\frac{dx}{dt}$$
If we imagine the completed circuit as a single turn on a coil - as it increases in size the total area of the magnetic field it contains increases. The magnetic flux density is constant, but the magnetic flux $\phi$ increases, because it is a function of interaction area, so:
$$\phi=B\cdot A$$
$$d\phi=B\cdot dA=Bl\cdot dx$$
Therefore if we substitute this into Faraday's Law:
$$\epsilon=-N\frac{d\phi}{dt}=-B\cdot l \frac{dx}{dt}=-B\cdot l \cdot v$$
Where $N=1$ as we are only considering a single turn.
\
Hence the EMF induced in a wire of length $l$ moving through a magnetic field of strength $B$ with velocity $v$ is:
$$\epsilon=-B\cdot l \cdot v$$
