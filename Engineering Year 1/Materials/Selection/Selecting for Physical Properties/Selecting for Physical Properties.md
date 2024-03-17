Often we need to choose materials based on their physical properties. This includes thermal, electrical, and optical properties.
### Electrical Properties
The resistivity $\rho$ of a material is the dimension normalised resistance of a material (i.e. it is a material property). The higher a resistivity the more power lost across that material if in a circuit.
Metals are typically good conductors and as such have low resistivities.
Note that precipitate strengthening/alloying can increase the resistivity of a material as the alloying elements get in the way of electrons. 
The best option for strengthening a material that needs to carry both current and load (like overhead power lines) is work hardening as dislocations have a very low impact on electron movements.
### Thermal Properties
Temperature is a measure of the average kinetic energy of atoms and molecules. 
Materials have minimum and maximum service temperatures, which are the limit for sustained, sage use of a material. This is typically constrained by things like oxidation, drops in strength, or changes in chemical structure.
Typically the maximum service temperature is much lower than the melting point as materials (metals especially) lose a lot of their strength when heated to a fraction of their melting point.
Many properties vary linearly with temperature:
![[Pasted image 20240309135403.png|center]]
#### Thermal Conductivity
Thermal conductivity is a measure of how quickly the material can move heat from areas of high temperature to low temperature. We measure this my measuring the heat flux $q$ through a surface required to maintain a temperature gradient between a hot side and a cold side over a plate of material of thickness x, resulting in the equation:
$$q=-\lambda \frac{\Delta T}{x}$$
![[Pasted image 20240309135700.png|center]]
Where $\lambda$ is the thermal conductivity.
#### Specific Heat Capacity and Thermal Diffusivity
We already know about [[Specific Heat Capacity at Constant Volume]] and [[Specific Heat Capacity at Constant Pressure]], however thermal diffusivity is a measure of how quickly a material changes temperature. A material with a low thermal diffusivity will change its temperature more slowly and a heat wave will take longer to pass through.
Diffusivity (a) can be calculated to be:
$$a = \frac{\lambda}{\rho C_p}$$
So it is related to the thermal conductivity of the material as well as its density and [[Specific Heat Capacity at Constant Pressure]].
\
Note that $\rho C_p$ is the energy absorbed by the wall per unit volume per degree.
#### Thermal Expansion Coefficient
Thermal expansion is a strain arising from the increased separation of atoms as temperature increases. The expansion is resisted by stiffness of the atomic bonds and a good approximation is:
$$\alpha=\frac{1}{L}\frac{dL}{dT}(K^{-1})$$
Where $L$ is some linear dimension of a body. 
![[Pasted image 20240309143127.png|center]]
If a material heats up then stresses can accumulate if expansion is constrained in some way, there are two common ways for this to happen:
1) Difference in expansion between two materials
If a structure is made up of two different materials that expand differently as temperature changes then stress can be created, take for example a small component with modulus $E_1$ and expansion coefficient $\alpha_1$ connected to a much larger one with expansion coefficient $\alpha_2$, the stress will be:
$$\sigma=E_1(\alpha_1-\alpha_2)\Delta T$$
So minimising differential stresses relies on choosing materials with similar expansion coefficients.
1) Thermal gradients
If heat is suddenly applied then a heat wave will move through the material and there will be a thermal strain/stress mismatch over that gradient (as some parts are expanding more than others).The stress is more extreme the greater the thermal gradient. Materials with high conductivity and low expansion coefficients reduce this strain. Typically materials with a high $\lambda/\alpha$ is predictive of better performance.
### The Material Index (M)
The material index is a method of telling us what material properties are impacting the result that we want. Take for example the following equation:
$$\frac{Q}{m}= \frac{\Delta T}{t^{2}} \frac{\lambda}{\rho}$$
The material index will equal:
$$M=\frac{\lambda}{\rho}$$ As all of the other variables do not impact the material that we are selecting. b