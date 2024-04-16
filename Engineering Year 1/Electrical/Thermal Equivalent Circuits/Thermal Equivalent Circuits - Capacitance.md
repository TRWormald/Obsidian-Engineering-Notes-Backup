### Thermal System
**Consider the steady state condition** of an object before and after the addition of heat energy. The object has mass $m$ and specific heat capacity $c_{p}$. The temperature of the object rises from $T_{1}$ to $T_{2}$, so $\Delta T=T_{2}-T_{1}$. Hence:
$$Q=m\cdot c_{p}\cdot(T_{2}-T_{1})$$
As the mass and specific heat capacity are constant we can combine them into a single homogenous unit - the thermal capacitance $C_{t}$ - where:
$$C_{t}=m\cdot c_{p}~[J/K]$$
Note how this is now independent of mass.
Hence:
$$Q=C_{t}\cdot (T_{2}-T_{1})$$
**Consider the transient case where heat is being constantly added to the object at a rate $\dot{Q}$**
$$\dot{Q}=C_{t}\cdot\frac{d(T_{2}-T_{1})}{dt}$$
We know that $\frac{dT_{1}}{dt}=0$ as $T_{1}$ is the constant temperature of the ambient surroundings, hence:
$$\dot{Q}=C_{t}\cdot \frac{dT_{2}}{dt}$$
### Electrical Equivalence
Consider the following equivalent circuit, including a capacitor (of capacitance $C_{e}$) and a current source:
![[Pasted image 20240416102534.png|center|300]]
- $V_{1}$ is constant as it is connected to the ground
- Current flow ($I$) increases $V_{2}$ over time
Hence:
$$I=C_{e}\cdot \frac{d(V_{2}-V_{1})}{dt}$$
And again $\frac{dV_{1}}{dt}=0$ so:
$$I=C_{e}\cdot \frac{dV_{2}}{dt}$$
